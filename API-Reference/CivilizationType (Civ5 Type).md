{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|ID.png|The <code>CivilizationType</code> pseudo-type is actually a regular '''integer'''. Pseudo-types do not exist in Lua, they only serve a documentation purpose on the wiki!
* {{DB}} Integers labeled as <code>CivilizationType</code> corresponds to the ''ID'' column of the {{Table5|Civilizations|CIV5Civilizations}} XML table.
}}


= XML: the Civilizations table =
Here are the ''ID'' and ''Type'' columns found in this table.
<code>
{|
|-
!align="left" |ID
!
!align="left" |Type
|-
|align="right"|0
|
|CIVILIZATION_AMERICA
|-
|align="right"|0
|
|CIVILIZATION_AUSTRIA
|-
|align="right"|1
|
|CIVILIZATION_ARABIA
|-
|align="right"|1
|
|CIVILIZATION_BYZANTIUM
|-
|align="right"|2
|
|CIVILIZATION_AZTEC
|-
|align="right"|2
|
|CIVILIZATION_CARTHAGE
|-
|align="right"|3
|
|CIVILIZATION_CHINA
|-
|align="right"|3
|
|CIVILIZATION_CELTS
|-
|align="right"|4
|
|CIVILIZATION_EGYPT
|-
|align="right"|4
|
|CIVILIZATION_ETHIOPIA
|-
|align="right"|5
|
|CIVILIZATION_ENGLAND
|-
|align="right"|5
|
|CIVILIZATION_HUNS
|-
|align="right"|6
|
|CIVILIZATION_FRANCE
|-
|align="right"|6
|
|CIVILIZATION_MAYA
|-
|align="right"|7
|
|CIVILIZATION_GERMANY
|-
|align="right"|7
|
|CIVILIZATION_NETHERLANDS
|-
|align="right"|8
|
|CIVILIZATION_GREECE
|-
|align="right"|8
|
|CIVILIZATION_SWEDEN
|-
|align="right"|9
|
|CIVILIZATION_INDIA
|-
|align="right"|10
|
|CIVILIZATION_IROQUOIS
|-
|align="right"|11
|
|CIVILIZATION_JAPAN
|-
|align="right"|12
|
|CIVILIZATION_OTTOMAN
|-
|align="right"|13
|
|CIVILIZATION_PERSIA
|-
|align="right"|14
|
|CIVILIZATION_ROME
|-
|align="right"|15
|
|CIVILIZATION_RUSSIA
|-
|align="right"|16
|
|CIVILIZATION_SIAM
|-
|align="right"|17
|
|CIVILIZATION_SONGHAI
|-
|align="right"|18
|
|CIVILIZATION_MINOR
|-
|align="right"|19
|
|CIVILIZATION_BARBARIAN
|}</code>


= Examples =
Here are different ways to query the database to retrieve the ''ID'' from the ''type''. Those examples will return and assign the integer value 0. See also {{Type5|GameInfo}}.
<syntaxhighlight lang="lua" class="civ5-example">
local id = GameInfo.Civilizations.CIVILIZATION_AUSTRIA.ID
local id = GameInfo["Civilizations"].["CIVILIZATION_AUSTRIA"].ID
local id = GameInfo.Civilizations{Type="CIVILIZATION_AUSTRIA"}().ID
</syntaxhighlight>
Alternatively you could use the ''ID'' or the ''type'' to retrieve the value of the ''Description'' column. Those examples will return and assign the value TXT_KEY_CIV_AUSTRIA_DESC.
<syntaxhighlight lang="lua" class="civ5-example">
local description = GameInfo.Civilizations[0].Description
local description = GameInfo["Civilizations"][0]["Description"]
local description = GameInfo.Civilizations{ID=0}().Description
</syntaxhighlight>


=Used by=
{|cellspacing="4" cellpadding="0" width="100%" style="background-color:#F0F0F0"
<!-- 
GETCIVILIZATIONTYPE
-->
|-
|align="right" width="200" |<code>{{Type5|CivilizationType}}</code>
|style="padding-left:6px" |<code>{{Type5|City}}:{{Func5|City|GetCivilizationType}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ADDPLAYER
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Game}}.{{Func5|Game|AddPlayer}}<b>(</b>{{Type5|PlayerID}} newPlayer, {{Type5|LeaderType}} leader, {{Type5|CivilizationType}} civ<b>)</b></code>
<!-- 
GETACTIVECIVILIZATIONTYPE
-->
|-
|align="right" width="200" |<code>{{Type5|CivilizationType}}</code>
|style="padding-left:6px" |<code>{{Type5|Game}}.{{Func5|Game|GetActiveCivilizationType}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ISCIVEVERACTIVE
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|Game}}.{{Func5|Game|IsCivEverActive}}<b>(</b>{{Type5|CivilizationType}} civilization<b>)</b></code>
<!-- 
GETCIVILIZATIONTYPE
-->
|-
|align="right" width="200" |<code>{{Type5|CivilizationType}}</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|GetCivilizationType}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETCIVILIZATION
-->
|-
|align="right" width="200" |<code>{{Type5|CivilizationType}}</code>
|style="padding-left:6px" |<code>{{Type5|PreGame}}.{{Func5|PreGame|GetCivilization}}<b>(</b>{{Type5|PlayerID}} i = nil<b>)</b></code>
<!-- 
SETCIVILIZATION
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|PreGame}}.{{Func5|PreGame|SetCivilization}}<b>(</b>{{Type5|PlayerID}} player, {{Type5|CivilizationType}} civ = nil<b>)</b></code>
<!-- 
GETHALLOFFAMEDATA
-->
|-
|align="right" width="200" |<code>table('''unknown''' => '''table''')</code>
|style="padding-left:6px" |<code>{{Type5|UI}}.{{Func5|UI|GetHallofFameData}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETCAPTUREUNITTYPE
-->
|-
|align="right" width="200" |<code>{{Type5|UnitType}}</code>
|style="padding-left:6px" |<code>{{Type5|Unit}}:{{Func5|Unit|GetCaptureUnitType}}<b>(</b>{{Type5|CivilizationType}} civilization<b>)</b></code>
<!-- 
GETCIVILIZATIONTYPE
-->
|-
|align="right" width="200" |<code>{{Type5|CivilizationType}}</code>
|style="padding-left:6px" |<code>{{Type5|Unit}}:{{Func5|Unit|GetCivilizationType}}<b>(</b><!-- No arguments --><b>)</b></code>
|}




{{Civ5 API Footer}}
[[Category:Civ5 Types|CivilizationType]]