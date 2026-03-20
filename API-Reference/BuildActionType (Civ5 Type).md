{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|ID.png|The <code>BuildActionType</code> pseudo-type is actually a regular '''integer'''. Pseudo-types do not exist in Lua, they only serve a documentation purpose on the wiki!
* {{DB}} Integers labeled as <code>BuildActionType</code> corresponds to the ''ID'' column of the {{Table5|Builds|CIV5Builds}} XML table.
}}


= XML: the Builds table =
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
|BUILD_ROAD
|-
|align="right"|0
|
|BUILD_HOLY_SITE
|-
|align="right"|1
|
|BUILD_RAILROAD
|-
|align="right"|1
|
|BUILD_POLDER
|-
|align="right"|2
|
|BUILD_FARM
|-
|align="right"|3
|
|BUILD_MINE
|-
|align="right"|4
|
|BUILD_TRADING_POST
|-
|align="right"|5
|
|BUILD_LUMBERMILL
|-
|align="right"|6
|
|BUILD_PASTURE
|-
|align="right"|7
|
|BUILD_CAMP
|-
|align="right"|8
|
|BUILD_PLANTATION
|-
|align="right"|9
|
|BUILD_QUARRY
|-
|align="right"|10
|
|BUILD_WELL
|-
|align="right"|11
|
|BUILD_OFFSHORE_PLATFORM
|-
|align="right"|12
|
|BUILD_FISHING_BOATS
|-
|align="right"|13
|
|BUILD_FORT
|-
|align="right"|14
|
|BUILD_REMOVE_JUNGLE
|-
|align="right"|15
|
|BUILD_REMOVE_FOREST
|-
|align="right"|16
|
|BUILD_REMOVE_MARSH
|-
|align="right"|17
|
|BUILD_SCRUB_FALLOUT
|-
|align="right"|18
|
|BUILD_REPAIR
|-
|align="right"|19
|
|BUILD_REMOVE_ROUTE
|-
|align="right"|20
|
|BUILD_LANDMARK
|-
|align="right"|21
|
|BUILD_ACADEMY
|-
|align="right"|22
|
|BUILD_CUSTOMS_HOUSE
|-
|align="right"|23
|
|BUILD_MANUFACTORY
|-
|align="right"|24
|
|BUILD_CITADEL
|}</code>


= Examples =
Here are different ways to query the database to retrieve the ''ID'' from the ''type''. Those examples will return and assign the integer value 0. See also {{Type5|GameInfo}}.
<syntaxhighlight lang="lua" class="civ5-example">
local id = GameInfo.Builds.BUILD_HOLY_SITE.ID
local id = GameInfo["Builds"].["BUILD_HOLY_SITE"].ID
local id = GameInfo.Builds{Type="BUILD_HOLY_SITE"}().ID
</syntaxhighlight>
Alternatively you could use the ''ID'' or the ''type'' to retrieve the value of the ''Description'' column. Those examples will return and assign the value TXT_KEY_BUILD_HOLY_SITE.
<syntaxhighlight lang="lua" class="civ5-example">
local description = GameInfo.Builds[0].Description
local description = GameInfo["Builds"][0]["Description"]
local description = GameInfo.Builds{ID=0}().Description
</syntaxhighlight>


=Used by=
{|cellspacing="4" cellpadding="0" width="100%" style="background-color:#F0F0F0"
<!-- 
SELECTIONLISTGAMENETMESSAGE
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Game}}.{{Func5|Game|SelectionListGameNetMessage}}<b>(</b>{{Type5|GameMessageType}} message, '''int''' data2 = -1, {{Type5|BuildActionType}} data3 = -1, {{Type5|UnitID}} data4 = -1, '''int''' flags = 0, '''bool''' alt = false, '''bool''' shift = false<b>)</b></code>
<!-- 
CANBUILD
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|CanBuild}}<b>(</b>{{Type5|Plot}} plot, {{Type5|BuildActionType}} build, '''bool''' testEra = false, '''bool''' testVisible = false, '''bool''' testGold = false<b>)</b></code>
<!-- 
ISBUILDBLOCKEDBYFEATURE
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|IsBuildBlockedByFeature}}<b>(</b>{{Type5|BuildActionType}} build, {{Type5|FeatureType}} feature<b>)</b></code>
<!-- 
CANBUILD
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|Plot}}:{{Func5|Plot|CanBuild}}<b>(</b>{{Type5|BuildActionType}} build, {{Type5|PlayerID}} player, '''bool''' testVisible<b>)</b></code>
<!-- 
CHANGEBUILDPROGRESS
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|Plot}}:{{Func5|Plot|ChangeBuildProgress}}<b>(</b>{{Type5|BuildActionType}} build, '''int''' change, {{Type5|TeamID}} team<b>)</b></code>
<!-- 
GETBUILDPROGRESS
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Plot}}:{{Func5|Plot|GetBuildProgress}}<b>(</b>{{Type5|BuildActionType}} build<b>)</b></code>
<!-- 
GETBUILDTIME
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Plot}}:{{Func5|Plot|GetBuildTime}}<b>(</b>{{Type5|BuildActionType}} build<b>)</b></code>
<!-- 
GETBUILDTURNSLEFT
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Plot}}:{{Func5|Plot|GetBuildTurnsLeft}}<b>(</b>{{Type5|BuildActionType}} build, '''int''' nowExtra, '''int''' thenExtra<b>)</b></code>
<!-- 
GETBUILDTURNSTOTAL
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Plot}}:{{Func5|Plot|GetBuildTurnsTotal}}<b>(</b>{{Type5|BuildActionType}} build<b>)</b></code>
<!-- 
GETFEATUREPRODUCTION
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Plot}}:{{Func5|Plot|GetFeatureProduction}}<b>(</b>{{Type5|BuildActionType}} build, {{Type5|TeamID}} team, {{Type5|City}} city<b>)</b></code>
<!-- 
GETYIELDWITHBUILD
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Plot}}:{{Func5|Plot|GetYieldWithBuild}}<b>(</b>{{Type5|BuildActionType}} build, {{Type5|YieldType}} yield, '''bool''' arg2, {{Type5|PlayerID}} activePlayer<b>)</b></code>
<!-- 
ISBUILDREMOVESFEATURE
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|Plot}}:{{Func5|Plot|IsBuildRemovesFeature}}<b>(</b>{{Type5|BuildActionType}} build<b>)</b></code>
<!-- 
CANBUILD
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|Unit}}:{{Func5|Unit|CanBuild}}<b>(</b>{{Type5|Plot}} plot, {{Type5|BuildActionType}} build, '''bool''' testVisible = false, '''bool''' testGold = true<b>)</b></code>
<!-- 
GETBUILDTYPE
-->
|-
|align="right" width="200" |<code>{{Type5|BuildActionType}}</code>
|style="padding-left:6px" |<code>{{Type5|Unit}}:{{Func5|Unit|GetBuildType}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
WORKRATE
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Unit}}:{{Func5|Unit|WorkRate}}<b>(</b>'''bool''' max, {{Type5|BuildActionType}} build = nil<b>)</b></code>
|}




{{Civ5 API Footer}}
[[Category:Civ5 Types|BuildActionType]]