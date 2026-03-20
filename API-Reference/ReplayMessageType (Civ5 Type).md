{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|ID.png|The <code>ReplayMessageType</code> pseudo-type is actually a regular '''integer'''. Pseudo-types do not exist in Lua, they only serve a documentation purpose on the wiki!
* {{DB}} Integers labeled as <code>ReplayMessageType</code> corresponds to the ''ID'' column of the {{Table5|ReplayDataSets|CIV5Replays}} XML table.
}}


= XML: the ReplayDataSets table =
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
|REPLAYDATASET_SCORE
|-
|align="right"|1
|
|REPLAYDATASET_PRODUCTIONPERTURN
|-
|align="right"|2
|
|REPLAYDATASET_TOTALGOLD
|-
|align="right"|3
|
|REPLAYDATASET_GOLDPERTURN
|-
|align="right"|4
|
|REPLAYDATASET_CITYCOUNT
|-
|align="right"|5
|
|REPLAYDATASET_TECHSKNOWN
|-
|align="right"|6
|
|REPLAYDATASET_SCIENCEPERTURN
|-
|align="right"|7
|
|REPLAYDATASET_TOTALCULTURE
|-
|align="right"|8
|
|REPLAYDATASET_CULTUREPERTURN
|-
|align="right"|9
|
|REPLAYDATASET_EXCESSHAPINESS
|-
|align="right"|10
|
|REPLAYDATASET_HAPPINESS
|-
|align="right"|11
|
|REPLAYDATASET_UNHAPPINESS
|-
|align="right"|12
|
|REPLAYDATASET_GOLDENAGETURNS
|-
|align="right"|13
|
|REPLAYDATASET_POPULATION
|-
|align="right"|14
|
|REPLAYDATASET_FOODPERTURN
|-
|align="right"|15
|
|REPLAYDATASET_TOTALLAND
|-
|align="right"|16
|
|REPLAYDATASET_GPTCITYCONNECTIONS
|-
|align="right"|17
|
|REPLAYDATASET_GPTDEALS
|-
|align="right"|18
|
|REPLAYDATASET_UNITMAINTENANCE
|-
|align="right"|19
|
|REPLAYDATASET_BUILDINGMAINTENANCE
|-
|align="right"|20
|
|REPLAYDATASET_IMPROVEMENTMAINTENANCE
|-
|align="right"|21
|
|REPLAYDATASET_NUMBEROFPOLICIES
|-
|align="right"|22
|
|REPLAYDATASET_NUMBEROFWORKERS
|-
|align="right"|23
|
|REPLAYDATASET_IMPROVEDTILES
|-
|align="right"|24
|
|REPLAYDATASET_WORKEDTILES
|-
|align="right"|25
|
|REPLAYDATASET_MILITARYMIGHT
|}</code>


= Examples =
Here are different ways to query the database to retrieve the ''ID'' from the ''type''. Those examples will return and assign the integer value -1. See also {{Type5|GameInfo}}.
<syntaxhighlight lang="lua" class="civ5-example">
local id = GameInfo.ReplayDataSets.REPLAYDATASET_SCORE.ID
local id = GameInfo["ReplayDataSets"].["REPLAYDATASET_SCORE"].ID
local id = GameInfo.ReplayDataSets{Type="REPLAYDATASET_SCORE"}().ID
</syntaxhighlight>
Alternatively you could use the ''ID'' or the ''type'' to retrieve the value of the ''Description'' column. Those examples will return and assign the value TXT_KEY_REPLAY_VIEWER_GRAPHBY_SCORE.
<syntaxhighlight lang="lua" class="civ5-example">
local description = GameInfo.ReplayDataSets[-1].Description
local description = GameInfo["ReplayDataSets"][-1]["Description"]
local description = GameInfo.ReplayDataSets{ID=-1}().Description
</syntaxhighlight>


=Used by=
{|cellspacing="4" cellpadding="0" width="100%" style="background-color:#F0F0F0"
<!-- 
GETREPLAYMESSAGETYPE
-->
|-
|align="right" width="200" |<code>{{Type5|ReplayMessageType}}</code>
|style="padding-left:6px" |<code>{{Type5|Game}}.{{Func5|Game|GetReplayMessageType}}<b>(</b>{{Type5|ReplayMessageType}} i<b>)</b></code>
|}




{{Civ5 API Footer}}
[[Category:Civ5 Types|ReplayMessageType]]