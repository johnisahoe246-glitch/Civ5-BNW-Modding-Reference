''This page is a part of the [[Lua and UI Reference (Civ5)|Lua and UI Reference]].''


This article explains how to store data that are persisted when the user saves his game, or at anytime for mods settings.

= Opening or creating a storage space =

Mods can store data in the following containers:
* Global storage spaces accessible at any time. To store mods settings for example.
* One local storage space embedded in savegames. A zombie mod could for example use it to store the locations where units died in case they should be resurrected later.


=== Global storage spaces ===
You create/open such a space by using: <code>{{Type5|ModData}} Modding.{{Func5|Modding|OpenUserData}}('''string''' name, '''int''' version)<code>.
* Many modders specify their mod's GUID as a name. However this is not mandatory and it is not necessary the best practice for the end-user since it produces undecipherable files names. We suggest you just make sure to provide a unique name to avoid conflicts between mods.
* This storage space will be stored under a file in <code>My Games/Sid Meier's Civilization V/ModUserData/</code>. The file name will be the name you provided with the ".db" extension.
* Mods can use the same space if they share common settings for example. However it cannot be used as a communication channel it is not possible to listen for changes.
* One mod can create as much spaces as it wants.


=== Savegame's storage space ===
You can create/open the savegame's storage space by using: <code>{{Type5|ModData}} Modding.{{Func5|Modding|OpenSaveData}}()</code>.
* This space is shared by all mods, so beware of keys names conflicts: when saving a property try to prepend its name with a unique prefix for your mod "IGE_" for In-game editor, "RED_" for R.E.D., etc.
* The content of this space is written directly in the savegame file whenever the user saves his game.


= Using the storage space =
=== Get or set value ===
Once you retrieve a {{Type5|ModData}} instance, this one exposes the following methods:
* <code>{{Func5|ModData|SetValue}}('''string''' name, '''variant''' data)</code>
* <code>'''variant''' {{Func5|ModData|GetValue}}('''string''' name)</code>
A few remarks:
* Data can be '''nil''', '''bool''', '''number''' or '''string'''.
* If you query a value never assigned before, it will be nil.


=== Dealing with default values ===
Since it is not possible to know whether the value you just did read already existed before, you need to deal with the default nil values you will encounter. Here are some examples:
<div class="civ5-example"><syntaxhighlight lang="lua">
local db = Modding.OpenSaveData()
local trueByDefault = db.GetValue("trueByDefault") ~= "false"  -- False if "false", true otherwise
local falseByDefault = db.GetValue("falseByDefault") == "true" -- True if "true", false otherwise
local oneByDefault = db.GetValue("oneByDefault") or 1          -- 1 if nil or false, the value otherwise
</syntaxhighlight></div>


= Addressing performances problems =
The {{Type5|ModData}} you get is implemented through a database table. This means that every value read/write will generate a request string, this one will have to be parsed, etc. If you frequently read or write values, this can greatly hinder the game's performances. 

=== Using a local cache ===
Dealing with the reads is pretty easy, we only need to create a local copy of the properties, as demonstrated in the G&K scenarios. Instead of calling {{Func5|ModData|GetValue}} and {{Func5|ModData|SetValue}} directly, we will use the following wrappers:
<div class="civ5-example"><syntaxhighlight lang="lua">
g_SaveData = Modding.OpenSaveData()
g_Properties = {}

function GetPersistentProperty(name)
    if not g_Properties[name] then
        g_Properties[name] = g_SaveData.GetValue(name)
    end
    return g_Properties[name]
end

function SetPersistentProperty(name, value)
    if GetPersistentProperty(name) == value then return end
    g_SaveData.SetValue(name, value)
    g_Properties[name] = value
end
</syntaxhighlight></div>


=== Persisting tables ===
A convenient and fast solution is to save tables, by exploiting the [http://www.lua.org/manual/5.1/manual.html#pdf-loadstring loadstring] table. The following implementation is a simple and naive one with the following limitations:
* Strings cannot contain the "]]" sequence.
* Can only save nils, booleans, numbers, strings, and tables. No functions or API Objects like {{Type5|Player}}.
* No identity preservation: if a sub-table is stored twice in the provided table, it will be deserialized as two different tables.
* It has not been tested, there may be errors.
<div class="civ5-example"><syntaxhighlight lang="lua">
function ToLuaCode(item)
   if type(item) == "nil" then return "nil" end
   if type(item) == "bool" then return tostring(item) end
   if type(item) == "number" then return tostring(item) end
   if type(item) == "string" then return "[[" .. item .. "]]" end
   if type(item) ~= "table" then error("could not serialize an element") end
   
   local str = "{"
   for k, v in pairs(item) do
       str = str .. "[" .. ToLuaCode(k) .. "] = " .. ToLuaCode(v) .. ", "
   end
   return str.."}"
end

function SetPersistentTable(name, t)
    g_SaveData.SetValue(name, ToLuaCode(t))
    g_Properties[name] = t
end

function GetPersistentTable(name)
    if not g_Properties[name] then
        local code = g_SaveData.GetValue(name)
        g_Properties[name] = loadstring(code)()
    end
    return g_Properties[name]
end
</syntaxhighlight></div>

=== Just-in-time writes ===
The previous tricks unfortunately do not address the problem entirely if you need frequent writes (for example anytime a unit moves). A good idea in theory would be to detect when the user is going to save his game so that you only write data at this point. Unfortunately there is no event for this circumstance and while it is possible to hijack the "quicksave" hotkey and the "save" menu, '''this creates a whole bunch of incompatibilities with other mods'''. Use it in last resort. If you want to see an implementation example, look at the R.E.D. WWII mod.

Another alternative is to use custom tables, as described in the next section.


= Alternatives =

=== Using the script data (mostly deprecated) ===
Every {{Type5|Player}}, {{Type5|Plot}} and {{Type5|Unit}} can hold one string.
* Strings are set through Player:{{Func5|Player|SetScriptData}}, Plot:{{Func5|Plot|SetScriptData}}, and Unit:{{Func5|Unit|SetScriptData}}
* Strings are retrieved through Player:{{Func5|Player|GetScriptData}}, Plot:{{Func5|Plot|GetScriptData}}, and Unit:{{Func5|Unit|GetScriptData}}
* Those data are shared between mods so this is a frequent cause of conflicts.
* There were more of those "SetScriptData" methods in the past, on other objects, but they have been removed on May 2012 by Firaxis. It is possible that Firaxis also removes the last three ones at a later point.
* Users interested in this solution should give a look at the [http://forums.civfanatics.com/showthread.php?t=392958 SaveUtils] library from Whys.


=== Using a custom table ===
If you want you may use a custom data table, although it has few advantages. It's not very convenient and if you were using it to store one row at once, you would encounter the same performances problems as {{Type5|ModData}}. However writing one or thousands of values at once in a data table makes small difference in the execution time so you could use it for batch updates and get good results. This can be an alternative to the table persistence method explained before. This can be done through <code>DB.{{Func5|DB|Query}}('''variant''' data)</code>. Users interested in this solution should also give a look at the [http://forums.civfanatics.com/showthread.php?t=442249 TableSaverLoader] library from Pazyryk.

Here is an example where we store magic points for some units (untested):
<div class="civ5-example"><syntaxhighlight lang="lua">
-- Create table if not already done on mod loading
if not GetPersistentProperty("MyMod_initialized") then 
   DB.Query("CREATE TABLE UnitsMagic( id INTEGER PRIMARY KEY UNIQUE, value INTEGER);")
   SetPersistentProperty("MyMod_initialized", true)
end

-- SaveAll takes a table[playerID][unitID] = value
function SaveAll(magicPoints)
    local query = ""
    for playerID, playerTable in ipairs(magicPoints) do
        for unitID, magicPoints in ipairs(playerTable) do
            -- Units' ID are player-specific only, so we compute a global unique identifier from the player's and unit's identifiers.
            local ID = playerID * 10000 + unitID
            query = query.."REPLACE INTO UnitsMagic (id, value) VALUES ("..ID..", "..magicPoints..");\n"
        end
    end
    DB.Query(query)
end
</syntaxhighlight></div>


[[Category:Civ5 API]]
[[Category:Civ5 Tutorials]]