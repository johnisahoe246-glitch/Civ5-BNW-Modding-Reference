''This page is a part of the [[Civ5 Modding Tutorials]].''

= Checklist =
* Did you correctly import to the [[VFS (Civ5)|VFS]] the files that need to be?
* Did you correctly set up the actions and content tab in your project?
* Did you restart civ5 after you added new files?


= XML Debugging =
[[File:SQLiteManager.png|frame|View of the snapshot using SQLiteManager]]
=== Checking the logs ===
If you correctly set up your [[#Configuration]], whenever you start a game, Civ5 saves some logs under <code>My Games/Sid Medier's Civilization V/cache/Civ5DebugDatabase.db</code>.
* If there were errors with the XML formatting of your data files (wrong column names for example), they will logged in XML.log. Some of those errors may be fatal: in such a case no mod is loaded!
:<pre>[6904.323] Tag (TXT_KEYMODDING_SHOWDLCMODS) does not start with 'TXT_KEY_'</pre>
* If there were errors with the data integrity (missing foreign keys for example - types that reference rows from other tables), they will logged in database.log.
:<pre>[6903.917] Invalid Reference on Leader_Flavors.LeaderType - "LEADER_HARALD" does not exist in Leaders</pre>


=== Using the snapshots ===
If you correctly set up your [[#Configuration]], whenever you start a game, Civ5 saves a snapshot of the database under <code>My Games/Sid Medier's Civilization V/cache/Civ5DebugDatabase.db</code>
* This allows you to check how your XML and SQL files have been merged with the standard game data.


= Lua Debugging =
=== Using the Firetuner console ===
If you correctly set up your [[#Configuration]], Civ5 will send all the Lua output to the Firetuner (and also to the <code>Lua.log</code> file). This includes all the debugging output but also any error that may arise, with their calls stack traces. 
<pre>
 Runtime Error: [string "C:\Users\Boss\Documents\My Games\Sid Meier'..."]:41: attempt to concatenate local 'name' (a nil value)
stack traceback:
	[string "C:\Users\Boss\Documents\My Games\Sid Meier'..."]:41: in function 'dumpObj'
	[string "C:\Users\Boss\Documents\My Games\Sid Meier'..."]:95: in function 'ScanAll'
	[string "C:\Users\Boss\Documents\My Games\Sid Meier'..."]:188: in main chunk
	[C]: ?
</pre>
Here we can see that a C/C++ code (the game engine) ran the main chunk called (the Lua file), which then called the function ''ScanAll'' on line 188, which then called ''dumpObj'' on line 95. And this one caused an error on line 41.


Note that paths are truncated in the provided example, which makes debugging harder sometimes. This happens when the file is in a {{Type5|context}} registered by the project's ''content'' tab. Here are the workarounds:
* Provide a custom stack trace, as explained in a further section.
* Register only a minimalist context, that will load additional contexts (through the UI LuaContext markup). Do not initiate any action from the root context, let the children context handle everything.
* Modifying your system paths is not recommended as it can cause incompatibilities with a few applications (old or badly written).


=== Print, assert and error ===
<code>print('''...''')</code> can be used to print anything to the Firetuner output. This allows you to check the flow of a program, or the values of variables. Print calls '''tostring''' on every argument and displays them all on a single line with tabulations as separators between them. Nil values are not displayed, so it is advised you provide expressions such as: <code>(expr or 'nil')</code>


<code>error('''string''' message, '''int''' level = 1)</code> throws an error with the specified message. The execution is then halted and the hand returned to the game engine (or the current protected call if you did use '''pcall''' or '''xpcall'''). The level parameter controls the error position that will be reported. 1 for the line where error is located, 2 for the function call that contained an error, etc. 0 for no position.


<code>assert('''variant''' condition, '''string''' message = "assertion failed")</code> can be used to assert the provided condition is neither nil nor false (everything else is evaluated to true in Lua). Otherwise, an error with the specified message is thrown. You can use them punctually, as a debugging technique. But they may also be used as a defensive programming technique similar to [http://en.wikipedia.org/wiki/Design_by_contract design-by-contract]: the idea is that whenever your program's correctness relies on an assumption, you should explicitly check it. For example, if a function takes an array as an argument and assumes that it is not empty, you should add two conditions at the beginning: <code>assert(type(t) == "table")</code> and <code>assert(#t > 0)</code>. This makes the code more self-explanatory (implicit assumptions are now explicitly stated) and it allows you to catch bugs as soon as possible, which typically makes them easier to understand and fix.


=== The end users' feedback ===
Most of the time, when one of your user encounters an error with your mod, he just stops using it. A fraction of them will do the effort of reporting bugs but too often the informations they provide is unusable (from "it doesn't work" to wrong reproduction steps "play until turn 173 and wait for Mars being aligned with Venus"). The best way to increase the number of reports and their usefulness is to let your mod tell them the info it needs, as illustrated below.

[[File:IGE-Error.png|none|frame|[http://forums.civfanatics.com/showthread.php?t=436912 In-game editor] tells its users what they must report, even including a calls stack trace when available. The user only needs to make a screenshot that will then land on his Steam profile (provided he didn't change the Steam settings). Reporting made easy!]]


The [[Lua introduction for confirmed developers]] describes a number of techniques you can use to achieve similar results. Here we present an implementation you can use to handle errors in the most dangerous parts of your code in order to present them to the user. The message will even include a full stack trace when available (you can provide your users a link to the [[#Configuration]] section and ask them to modify their config.ini).
<div class="civ5-example"><syntaxhighlight lang="lua">
-- Returns an array of strings, one for each call level. 
-- We could use debug.traceback instead but this ones truncates path and we cannot easily ignore the topmost levels.
function getStackTrace()
    -- Level 1 is getStackTrace, 2 is its caller
    local level = 2 
    local trace = {}
    while true do
        -- Gets that level's informations: function name, source file and line.
        local info = debug.getinfo(level, "nSl") 
        if not info then break end

        -- C code or Lua code?
        if info.what == "C" then
            table.insert(trace, "C function");
        else   
            local userStr = Path.GetFileName(info.source)..": "..info.currentline;
            if info.name and string.len(info.name) then
                userStr = userStr.." ("..info.name..")";
            end
            table.insert(trace, userStr);
        end
        level = level + 1
    end
    return trace;
end

-- Gets a nicely formatted string of the error. 
-- The second parameter is the number of levels to ignore in the calls stack (formatError excluded). Defaults to 0.
function formatError(err, levelsToIgnoreBelow)
    print(err);

    -- We do not want to include formatError in the stack trace, hence the +1
    levelsToIgnoreBelow = (levelsToIgnoreBelow or 0) + 1;

    -- 'err' is like: [string "C:\Users\Boss\Documents\My Games\Sid Meier'..."]:41: attempt to concatenate local 'name' (a nil value)
    -- We retrieve important positions in this string. Remember: not all paths are truncated.
    local elipsisIndex = string.find(err, "...", 1, true) or -5;
    local lineIndex = elipsisIndex + 6	
    local msgIndex = string.find(err, ":", lineIndex, true) + 1

    -- Can we append the stack trace?
    local result = ""
    if debug and debug.getinfo then
        result = string.sub(err, msgIndex)

        local trace = getStackTrace()
        for i, v in ipairs(trace) do
            print(v)
            if (i > levelsToIgnoreBelow) then
                result = result.."[NEWLINE]"..v;
            end
        end
    -- Otherwise just report the line and message, and the source file when not truncated.
    else
        result = "line "..string.sub(err, elipsisIndex)
    end

    return result
end

-- The error handler to provide to xpcall
local function errorHandler(err)
    -- The stack trace at this point is:
    -- 1: this error handler (must not be reported), 
    -- 2: C function calling the handler (kept for security)
    -- 3: the error source
    err = formatError(err, 1);

    -- Show a popup to the user
    local str = L("Oops, an error occured:").."[NEWLINE][ICON_PIRATE] "..err;
    Events.SerialEventGameMessagePopup( { Type = ButtonPopupTypes.BUTTONPOPUP_TEXT, Data1 = 800, Option1 = true, Text = str } );

    -- Restore things up here when needed. Beware to not cause any error as it would cause an infinite recursive call up to the stack overflow!
    return false
end

-- Calls someDangerousFunction with the given error handler
xpcall(someDangerousFunction, errorHandler)
</syntaxhighlight></div>


= Troubleshooting =
The [[Civ5 Useful Programs]] page presents you a number of tools you can use to inspect or modify the game. This is especially useful if you want to quickly reproduce a bug or test something, or to understand what is happening.
* Let's say your mod adds a tech but you do not see in the techs panel. There is a FireTuner panel you can use to see a flat list of all the techs in-game.
* Let's say your mod adds a unit or a wonder, the IGE mod allows you to quickly create an unit or build that wonder (including the splash screen).
* Let's say your mod modifies the yields when the player acquire a specific tech. Once again IGE allows you to grant you that tech and see how the yields are modified.


= Configuration =
Look for the following files under <code>My Documents/My Games/Sid Meiers' Civilization V</code> and open them in a text editor like the notepad (not in a word processor).
* '''config.ini'''
** Set <code>EnableTuner</code> to 1. Civ5 will duplicate the Lua output to FireTuner this one is when present.
** Set <code>LoggingEnabled</code> to 1. Civ5 will write log files under the <code>Logs</code> folder.
** Set <code>EnableLuaDebugLibrary</code> to 1. Civ5 will display stack traces on Lua errors and you will be able to use the [http://www.lua.org/manual/5.1/manual.html#pdf-debug.debug debug] object.
** Set <code>DebugPanel</code> to 1. By pressing the '''²''' key (may be '''ù''' or something else depending on your computer's language) during a game, Civ5 will display a debug panel.
* '''usersettings.ini'''
** Set <code>DebugMode</code> to 1. Needed to enable other features previously mentioned.


[[Category:Civ5 Tutorials]]