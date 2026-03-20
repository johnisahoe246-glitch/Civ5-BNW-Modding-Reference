''This page is a part of the [[Lua and UI Reference (Civ5)|Lua and UI Reference]].''


The Civ5 implementation is based on Lua 5.1.4. However it has been modified, mainly for sandboxing purposes.

= Missing elements =
Those items do not exist in the Civ5 implmentation of Lua. See [http://www.lua.org/manual/5.1/#index Lua Reference#Index] if you want to learn what they are for.

====Missing globals====
* '''__G'''


====Missing functions====
Use '''include''' instead of the '''load*''', '''module''' and '''require''' functions. See the next section for more informations.
* '''getfenv'''
* '''load'''
* '''loadfile'''
* '''loadstring'''
* '''module'''
* '''require'''
* '''setfenv'''
* '''setfenv'''


====Missing objects====
For I/O, use the methods from {{Type5|UI}} and {{Type5|Modding}} instead.
* '''file'''
* '''io'''
* '''package'''
* '''os''': it still exists but only contains the '''clock''', '''date''', '''time''' and '''difftime''' functions.
* <s>debug</s>: fortunately it has been added by Firaxis in May 2012. See [[Lua Debugging (Civ5)]]


= Include =
Instead of the usual functions for loading and requiring a Lua file from another, Civ5 provides a custom function to do so: '''include'''.

====Usage====
<code>table('''int''' => '''string''') include('''string''' file, '''bool''' useRegex = false)</code>
* '''file''': the name of the file, with or without extension. It can also be a local path starting from "Assets\UI" (see examples). Finally, if useRegex is true, it can be a regular expression where the '''%''' character is used instead of '''\'''.
* '''useRegex''': when true, the file argument will be treated as a [http://en.wikipedia.org/wiki/Regular_expression regular expression].
* '''returned value:''' an array that contains all the loaded files (a single one usually, many files if you did use a regular expression).

<div class="civ5-example"><syntaxhighlight lang="lua">
include("CityBannerManager")
include("CityBannerManager.lua")
include("Ingame\\CityBannerManager.lua") -- loads Assets/UI/Ingame/CityBannerManager.lua
include("CityBanner%w+.lua", true) -- loads all files starting with "CityBanner" and ending with ".lua".

-- Loads all "*Popup.lua" files in Assets/UI/Ingame/PopupsGeneric. 
-- Then we print a statement for each one of the included files.
local files = include("InGame\\PopupsGeneric\\%w+Popup.lua", true);
for i, v in ipairs(files) do
    print("Loaded Popup - "..v);
end
</syntaxhighlight></div>


====Restrictions====
* Only the files that have been imported into the [[VFS (Civ5)|VFS]] may be included.
* Usually only the first eight characters are checked. This is likely only true if you do not specify the path. This means that if you registered two files named ''MapScannerA.lua'' and ''MapScannerB.lua'', using <code>include("MapScannerA")</code> could either load the A file or the B file!
* When called in reaction to an UI event, include can silently fail. For example if you use it inside a function and this function is called in reaction to a click on a button, include will report it has been successful but the globals declared in the included file will not be included. This does not happen if you call this function after a Context update or at the time the mod is loaded.


[[Category:Civ5 API]]
[[Category:Civ5 Tutorials]]