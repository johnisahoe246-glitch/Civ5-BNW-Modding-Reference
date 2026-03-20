{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|ID.png|The <code>VictoryType</code> pseudo-type is actually a regular '''integer'''. Pseudo-types do not exist in Lua, they only serve a documentation purpose on the wiki!
* {{DB}} Integers labeled as <code>VictoryType</code> corresponds to the ''ID'' column of the {{Table5|Victories|CIV5Victories}} XML table.
}}


= XML: the Victories table =
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
|VICTORY_TIME
|-
|align="right"|1
|
|VICTORY_SPACE_RACE
|-
|align="right"|2
|
|VICTORY_DOMINATION
|-
|align="right"|3
|
|VICTORY_CULTURAL
|-
|align="right"|4
|
|VICTORY_DIPLOMATIC
|}</code>


= Examples =
Here are different ways to query the database to retrieve the ''ID'' from the ''type''. Those examples will return and assign the integer value 0. See also {{Type5|GameInfo}}.
<syntaxhighlight lang="lua" class="civ5-example">
local id = GameInfo.Victories.VICTORY_TIME.ID
local id = GameInfo["Victories"].["VICTORY_TIME"].ID
local id = GameInfo.Victories{Type="VICTORY_TIME"}().ID
</syntaxhighlight>
Alternatively you could use the ''ID'' or the ''type'' to retrieve the value of the ''Description'' column. Those examples will return and assign the value TXT_KEY_VICTORY_TIME.
<syntaxhighlight lang="lua" class="civ5-example">
local description = GameInfo.Victories[0].Description
local description = GameInfo["Victories"][0]["Description"]
local description = GameInfo.Victories{ID=0}().Description
</syntaxhighlight>


=Used by=
{|cellspacing="4" cellpadding="0" width="100%" style="background-color:#F0F0F0"
<!-- 
GETADJUSTEDLANDPERCENT
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Game}}.{{Func5|Game|GetAdjustedLandPercent}}<b>(</b>{{Type5|VictoryType}} victory<b>)</b></code>
<!-- 
GETADJUSTEDPOPULATIONPERCENT
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Game}}.{{Func5|Game|GetAdjustedPopulationPercent}}<b>(</b>{{Type5|VictoryType}} victory<b>)</b></code>
<!-- 
GETVICTORY
-->
|-
|align="right" width="200" |<code>{{Type5|VictoryType}}</code>
|style="padding-left:6px" |<code>{{Type5|Game}}.{{Func5|Game|GetVictory}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ISVICTORYVALID
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|Game}}.{{Func5|Game|IsVictoryValid}}<b>(</b>{{Type5|VictoryType}} index<b>)</b></code>
<!-- 
SETVICTORYVALID
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Game}}.{{Func5|Game|SetVictoryValid}}<b>(</b>{{Type5|VictoryType}} arg0, '''bool''' arg1<b>)</b></code>
<!-- 
SETWINNER
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Game}}.{{Func5|Game|SetWinner}}<b>(</b>{{Type5|TeamID}} newWinner, {{Type5|VictoryType}} newVictory<b>)</b></code>
<!-- 
VICTORYDELAY
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Game}}.{{Func5|Game|VictoryDelay}}<b>(</b>{{Type5|VictoryType}} victory<b>)</b></code>
<!-- 
SETVICTORY
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|PreGame}}.{{Func5|PreGame|SetVictory}}<b>(</b>{{Type5|VictoryType}} arg0, '''bool''' check<b>)</b></code>
<!-- 
CANLAUNCH
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|Team}}:{{Func5|Team|CanLaunch}}<b>(</b>{{Type5|VictoryType}} victory<b>)</b></code>
<!-- 
GETVICTORYCOUNTDOWN
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Team}}:{{Func5|Team|GetVictoryCountdown}}<b>(</b>{{Type5|VictoryType}} victory<b>)</b></code>
<!-- 
GETVICTORYDELAY
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Team}}:{{Func5|Team|GetVictoryDelay}}<b>(</b>{{Type5|VictoryType}} victory<b>)</b></code>
<!-- 
GETHALLOFFAMEDATA
-->
|-
|align="right" width="200" |<code>table('''unknown''' => '''table''')</code>
|style="padding-left:6px" |<code>{{Type5|UI}}.{{Func5|UI|GetHallofFameData}}<b>(</b><!-- No arguments --><b>)</b></code>
|}




{{Civ5 API Footer}}
[[Category:Civ5 Types|VictoryType]]