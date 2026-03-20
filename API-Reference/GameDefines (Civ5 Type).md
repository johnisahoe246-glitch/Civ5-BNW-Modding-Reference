{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



= Purpose =
This object exposes all the constants defined in the [[Civ5 GlobalDefines|GlobalDefines.xml]] and [[GlobalAIDefines|GlobalAIDefines.xml]] files. Example:
<syntaxhighlight lang="lua" class="civ5-example">
local startYear = GameDefines["START_YEAR"]
local startYear = GameDefines.START_YEAR
</syntaxhighlight>

This tables ''does'' reflect the changes made by mods.


= Built-in fields =
Besides of the constants defined in the datatables, there are also a few built-in constants.

===Players counts===
'''MAX_PLAYERS'''
:The maximum number of players in a game. 64 by default. See {{Type5|PlayerID}} for more informations.
'''MAX_CIV_PLAYERS'''
:The maximum number of non-barbarian players in a game. 63 by default. See {{Type5|PlayerID}} for more informations.
'''MAX_MAJOR_CIVS'''
:The maximum number of major civilizations in a game. 22 by default. See {{Type5|PlayerID}} for more informations.
'''MAX_MINOR_CIVS'''
:The maximum number of city states in a game. 41 by default. See {{Type5|PlayerID}} for more informations.


===Teams counts===
'''MAX_PLAYERS'''
:The maximum number of teams in a game. 64 by default. See {{Type5|TeamID}} for more informations.
'''MAX_CIV_PLAYERS'''
:The maximum number of non-barbarian teams in a game. 63 by default. See {{Type5|TeamID}} for more informations.


===Tutorial index===
'''Tutorial'''
:When zero, no tutorial is active. Otherwise, it is an index code for the active tutorial. 
:*1 movement and exploration
:*2 founding cities
:*3 improving cities
:*4 combat and conquest
:*5 diplomacy




{{Civ5 API Footer}}
[[Category:Civ5 Types|GameDefines]]