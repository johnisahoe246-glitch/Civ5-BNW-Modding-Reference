''This page is a part of the [[Lua and UI Reference (Civ5)|Lua and UI Reference]].''


= Firaxis Hungarian notation =
=== What is it? ===
Firaxis used a naming convention categorized as [http://en.wikipedia.org/wiki/Hungarian_notation Hungarian Notation]. The prefixes provide informations regarding the type.
* '''s''', '''sz''' and '''str''' mean a string. 
::Example: '''sName''' expects something like "Genghis Khan".
* '''b''' means boolean. 
::Example: '''bHide''' expects true or false.
* '''f''' means floating-point, a number. 
::Example: '''fScale''' expects a scale factor, may be 0.5, 1.0, 2.0, etc.
* '''i''' means integer, a number. Sometimes it may be one of the identifiers listed on the main page. 
::Example: '''iPlayer''' expects a {{Type5|PlayerID}} while '''iWidth''' expects a width in pixels (50, 200, etc).
* '''e''' means an identifier (integer) taken from a Lua enumeration. 
::Example: '''eBuilding''' expects a {{Type5|BuildingType}}. You could assign it with 10 or <code>GameInfoTypes.BUILDING_SEAPORT </code>, both are equivalent.
* '''p''' means an API object (p means pointer but pointer is a C term with no relevance in Lua). 
::Example: '''pPlayer''' expects a {{Type5|Player}} object.


=== Should you use the same notation? ===
* Pro: it's widely used in the community and your code will harmonize with the one from Firaxis.
* Pro: you always now the type of a variable by looking at its name, which is useful since ModBuddy does not inform us about the type.
* Con: it adds some clutter and it's not really necessary because most of the time a consistent naming is enough to know the type of a variable: for example playerID for a {{Type5|PlayerID}} and player for a {{Type5|Player}}.


[[Category:Civ5 API]]