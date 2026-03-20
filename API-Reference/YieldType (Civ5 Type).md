{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|ID.png|The <code>YieldType</code> pseudo-type is actually a regular '''integer'''. Pseudo-types do not exist in Lua, they only serve a documentation purpose on the wiki!
* {{DB}} Integers labeled as <code>YieldType</code> corresponds to the ''ID'' column of the {{Table5|Yields|CIV5Yields}} XML table.
* {{Lua}} The standard (unmodded) values in the ''ID'' and ''Type'' columns are also stored in the '''YieldTypes''' Lua enumeration.
}}


= Lua: the YieldTypes enumeration =
Firaxis provides a Lua enumeration named <code>YieldTypes</code>. This is just a regular global table. Its keys are the constants' names and the pairs the corresponding values.
* This specific enumeration contains data from the {{Table5|Yields|CIV5Yields}} data table.<br/>
* They are stored as key/value pairs: the keys are the strings from the ''Type'' column and the values are the integers from the ''ID'' column.<br/>
{{Warning}} Be careful: this enumeration do '''not''' reflect the changes, additions and deletions made by mods. As a result it is advised to rely on {{Type5|GameInfo}} instead.<br/>

<br/>Below are the values found in this enumeration.
<code>
{|
|-
!align="left" |Key
!
!align="left" |Value 
|-
|align="left" |"NO_YIELD"
|
|align="right" |-1
|-
|align="left" |"YIELD_FOOD"
|
|align="right" |0
|-
|align="left" |"YIELD_PRODUCTION"
|
|align="right" |1
|-
|align="left" |"YIELD_GOLD"
|
|align="right" |2
|-
|align="left" |"YIELD_SCIENCE"
|
|align="right" |3
|-
|align="left" |"YIELD_CULTURE"
|
|align="right" |4
|-
|align="left" |"YIELD_FAITH"
|
|align="right" |5
|-
|align="left" |"NUM_YIELD_TYPES"
|
|align="right" |6
|}</code>


= XML: the Yields table =
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
|YIELD_FOOD
|-
|align="right"|1
|
|YIELD_PRODUCTION
|-
|align="right"|2
|
|YIELD_GOLD
|-
|align="right"|3
|
|YIELD_SCIENCE
|-
|align="right"|4
|
|YIELD_CULTURE
|-
|align="right"|5
|
|YIELD_FAITH
|}</code>


= Examples =
Here is how to use the LUA enumeration to retrieve the ''ID'' from the ''type''. Those examples will return and assign the integer value 0.
<syntaxhighlight lang="lua" class="civ5-example">
local id = YieldTypes.YIELD_FOOD
local id = YieldTypes["YIELD_FOOD"]
</syntaxhighlight>


=Used by=
{|cellspacing="4" cellpadding="0" width="100%" style="background-color:#F0F0F0"
<!-- 
GETYIELDTOOLTIP
-->
|-
|align="right" width="200" |<code>'''string'''</code>
|style="padding-left:6px" |<code>{{Func5|GetYieldTooltip}}<b>(</b>{{Type5|City}} city, {{Type5|YieldType}} yieldType, '''int''' base, '''int''' total, '''string''' iconString, '''string''' modifiersString<b>)</b></code>
<!-- 
GETYIELDTOOLTIPHELPER
-->
|-
|align="right" width="200" |<code>'''string'''</code>
|style="padding-left:6px" |<code>{{Func5|GetYieldTooltipHelper}}<b>(</b>{{Type5|City}} city, {{Type5|YieldType}} yieldType, '''string''' icon<b>)</b></code>
<!-- 
GETYIELDRATEMODIFIER
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Area}}:{{Func5|Area|GetYieldRateModifier}}<b>(</b>{{Type5|PlayerID}} index1, {{Type5|YieldType}} index2<b>)</b></code>
<!-- 
FINDBASEYIELDRATERANK
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|City}}:{{Func5|City|FindBaseYieldRateRank}}<b>(</b>{{Type5|YieldType}} yield<b>)</b></code>
<!-- 
FINDYIELDRATERANK
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|City}}:{{Func5|City|FindYieldRateRank}}<b>(</b>{{Type5|YieldType}} yield<b>)</b></code>
<!-- 
GETBASEYIELDRATE
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|City}}:{{Func5|City|GetBaseYieldRate}}<b>(</b>{{Type5|YieldType}} index<b>)</b></code>
<!-- 
GETBASEYIELDRATEFROMBUILDINGS
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|City}}:{{Func5|City|GetBaseYieldRateFromBuildings}}<b>(</b>{{Type5|YieldType}} yieldType<b>)</b></code>
<!-- 
GETBASEYIELDRATEFROMMISC
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|City}}:{{Func5|City|GetBaseYieldRateFromMisc}}<b>(</b>{{Type5|YieldType}} yieldType<b>)</b></code>
<!-- 
GETBASEYIELDRATEFROMRELIGION
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|City}}:{{Func5|City|GetBaseYieldRateFromReligion}}<b>(</b>{{Type5|YieldType}} yieldType<b>)</b></code>
<!-- 
GETBASEYIELDRATEFROMSPECIALISTS
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|City}}:{{Func5|City|GetBaseYieldRateFromSpecialists}}<b>(</b>{{Type5|YieldType}} yieldType<b>)</b></code>
<!-- 
GETBASEYIELDRATEFROMTERRAIN
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|City}}:{{Func5|City|GetBaseYieldRateFromTerrain}}<b>(</b>{{Type5|YieldType}} yieldType<b>)</b></code>
<!-- 
GETBASEYIELDRATEMODIFIER
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|City}}:{{Func5|City|GetBaseYieldRateModifier}}<b>(</b>{{Type5|YieldType}} index, '''int''' extra = 0<b>)</b></code>
<!-- 
GETBUILDINGYIELDCHANGE
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|City}}:{{Func5|City|GetBuildingYieldChange}}<b>(</b>{{Type5|BuildingClassType}} buildingClass, {{Type5|YieldType}} yield<b>)</b></code>
<!-- 
GETEXTRASPECIALISTYIELD
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|City}}:{{Func5|City|GetExtraSpecialistYield}}<b>(</b>{{Type5|YieldType}} index<b>)</b></code>
<!-- 
GETEXTRASPECIALISTYIELDOFTYPE
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|City}}:{{Func5|City|GetExtraSpecialistYieldOfType}}<b>(</b>{{Type5|YieldType}} index, {{Type5|SpecialistType}} specialist<b>)</b></code>
<!-- 
GETLAKEPLOTYIELD
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|City}}:{{Func5|City|GetLakePlotYield}}<b>(</b>{{Type5|YieldType}} index<b>)</b></code>
<!-- 
GETRELIGIONBUILDINGCLASSYIELDCHANGE
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|City}}:{{Func5|City|GetReligionBuildingClassYieldChange}}<b>(</b>{{Type5|BuildingClassType}} buildingClass, {{Type5|YieldType}} arg1<b>)</b></code>
<!-- 
GETRESOURCEYIELDRATEMODIFIER
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|City}}:{{Func5|City|GetResourceYieldRateModifier}}<b>(</b>{{Type5|YieldType}} index, {{Type5|ResourceType}} resource<b>)</b></code>
<!-- 
GETRIVERPLOTYIELD
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|City}}:{{Func5|City|GetRiverPlotYield}}<b>(</b>{{Type5|YieldType}} index<b>)</b></code>
<!-- 
GETSEAPLOTYIELD
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|City}}:{{Func5|City|GetSeaPlotYield}}<b>(</b>{{Type5|YieldType}} index<b>)</b></code>
<!-- 
GETSPECIALISTYIELD
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|City}}:{{Func5|City|GetSpecialistYield}}<b>(</b>{{Type5|SpecialistType}} specialist, {{Type5|YieldType}} yield<b>)</b></code>
<!-- 
GETYIELDMODIFIERTOOLTIP
-->
|-
|align="right" width="200" |<code>'''string'''</code>
|style="padding-left:6px" |<code>{{Type5|City}}:{{Func5|City|GetYieldModifierTooltip}}<b>(</b>{{Type5|YieldType}} yieldType<b>)</b></code>
<!-- 
GETYIELDPERPOPTIMES100
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|City}}:{{Func5|City|GetYieldPerPopTimes100}}<b>(</b>{{Type5|YieldType}} yieldType<b>)</b></code>
<!-- 
GETYIELDRATE
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|City}}:{{Func5|City|GetYieldRate}}<b>(</b>{{Type5|YieldType}} index<b>)</b></code>
<!-- 
GETYIELDRATEMODIFIER
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|City}}:{{Func5|City|GetYieldRateModifier}}<b>(</b>{{Type5|YieldType}} index<b>)</b></code>
<!-- 
GETYIELDRATETIMES100
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|City}}:{{Func5|City|GetYieldRateTimes100}}<b>(</b>{{Type5|YieldType}} index<b>)</b></code>
<!-- 
ISCANPURCHASE
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|City}}:{{Func5|City|IsCanPurchase}}<b>(</b>{{Type5|UnitType}} unitType, '''int''' buildingType, '''int''' projectType, '''int''' projectID, '''int''' projectID = nil, {{Type5|YieldType}} yield = nil<b>)</b></code>
<!-- 
SETBUILDINGYIELDCHANGE
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|City}}:{{Func5|City|SetBuildingYieldChange}}<b>(</b>{{Type5|BuildingClassType}} buildingClass, {{Type5|YieldType}} yield, '''int''' change<b>)</b></code>
<!-- 
GETBUILDINGYIELDCHANGE
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Game}}.{{Func5|Game|GetBuildingYieldChange}}<b>(</b>{{Type5|BuildingType}} building, {{Type5|YieldType}} arg1<b>)</b></code>
<!-- 
GETBUILDINGYIELDMODIFIER
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Game}}.{{Func5|Game|GetBuildingYieldModifier}}<b>(</b>{{Type5|BuildingType}} building, {{Type5|YieldType}} arg1<b>)</b></code>
<!-- 
SETPLOTEXTRAYIELD
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Game}}.{{Func5|Game|SetPlotExtraYield}}<b>(</b>'''int''' x, '''int''' y, {{Type5|YieldType}} yield, '''int''' extraYield<b>)</b></code>
<!-- 
CALCULATETOTALYIELD
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|CalculateTotalYield}}<b>(</b>{{Type5|YieldType}} yield<b>)</b></code>
<!-- 
GETCAPITALYIELDRATEMODIFIER
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|GetCapitalYieldRateModifier}}<b>(</b>{{Type5|YieldType}} index<b>)</b></code>
<!-- 
GETEXTRAYIELDTHRESHOLD
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|GetExtraYieldThreshold}}<b>(</b>{{Type5|YieldType}} index<b>)</b></code>
<!-- 
GETPLAYERBUILDINGCLASSYIELDCHANGE
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|GetPlayerBuildingClassYieldChange}}<b>(</b>{{Type5|BuildingClassType}} buildingClass, {{Type5|YieldType}} arg1<b>)</b></code>
<!-- 
GETPOLICYBUILDINGCLASSYIELDCHANGE
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|GetPolicyBuildingClassYieldChange}}<b>(</b>{{Type5|BuildingClassType}} buildingClass, {{Type5|YieldType}} arg1<b>)</b></code>
<!-- 
GETPOLICYBUILDINGCLASSYIELDMODIFIER
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|GetPolicyBuildingClassYieldModifier}}<b>(</b>{{Type5|BuildingClassType}} buildingClass, {{Type5|YieldType}} arg1<b>)</b></code>
<!-- 
GETSEAPLOTYIELD
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|GetSeaPlotYield}}<b>(</b>{{Type5|YieldType}} index<b>)</b></code>
<!-- 
GETSPECIALISTEXTRAYIELD
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|GetSpecialistExtraYield}}<b>(</b>{{Type5|SpecialistType}} index1, {{Type5|YieldType}} index2<b>)</b></code>
<!-- 
GETYIELDRATEMODIFIER
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|GetYieldRateModifier}}<b>(</b>{{Type5|YieldType}} index<b>)</b></code>
<!-- 
ISCANPURCHASEANYCITY
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|IsCanPurchaseAnyCity}}<b>(</b>'''bool''' arg0, '''bool''' arg1, {{Type5|UnitType}} arg2, {{Type5|BuildingType}} arg3, {{Type5|YieldType}} arg4<b>)</b></code>
<!-- 
SPECIALISTYIELD
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|SpecialistYield}}<b>(</b>{{Type5|SpecialistType}} specialist, {{Type5|YieldType}} yield<b>)</b></code>
<!-- 
CALCULATEBESTNATUREYIELD
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Plot}}:{{Func5|Plot|CalculateBestNatureYield}}<b>(</b>{{Type5|YieldType}} index, {{Type5|TeamID}} team<b>)</b></code>
<!-- 
CALCULATEIMPROVEMENTYIELDCHANGE
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Plot}}:{{Func5|Plot|CalculateImprovementYieldChange}}<b>(</b>{{Type5|ImprovementType}} improvement, {{Type5|YieldType}} yield, {{Type5|PlayerID}} player, '''bool''' optimal, {{Type5|RouteType}} assumeThisRoute<b>)</b></code>
<!-- 
CALCULATENATUREYIELD
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Plot}}:{{Func5|Plot|CalculateNatureYield}}<b>(</b>{{Type5|YieldType}} index, {{Type5|TeamID}} team, '''bool''' ignoreFeature = false<b>)</b></code>
<!-- 
CALCULATEYIELD
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Plot}}:{{Func5|Plot|CalculateYield}}<b>(</b>{{Type5|YieldType}} index, '''bool''' display<b>)</b></code>
<!-- 
GETYIELD
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Plot}}:{{Func5|Plot|GetYield}}<b>(</b>{{Type5|YieldType}} index<b>)</b></code>
<!-- 
GETYIELDWITHBUILD
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Plot}}:{{Func5|Plot|GetYieldWithBuild}}<b>(</b>{{Type5|BuildActionType}} build, {{Type5|YieldType}} yield, '''bool''' arg2, {{Type5|PlayerID}} activePlayer<b>)</b></code>
<!-- 
HASYIELD
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|Plot}}:{{Func5|Plot|HasYield}}<b>(</b>{{Type5|YieldType}} yield<b>)</b></code>
<!-- 
CHANGEIMPROVEMENTYIELDCHANGE
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Team}}:{{Func5|Team|ChangeImprovementYieldChange}}<b>(</b>{{Type5|ImprovementType}} index1, {{Type5|YieldType}} index2, '''int''' change<b>)</b></code>
<!-- 
GETIMPROVEMENTYIELDCHANGE
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Team}}:{{Func5|Team|GetImprovementYieldChange}}<b>(</b>{{Type5|ImprovementType}} index, {{Type5|YieldType}} index2<b>)</b></code>
|}




{{Civ5 API Footer}}
[[Category:Civ5 Types|YieldType]]