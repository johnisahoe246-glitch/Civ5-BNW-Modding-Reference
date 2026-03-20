{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|ID.png|The <code>ImprovementType</code> pseudo-type is actually a regular '''integer'''. Pseudo-types do not exist in Lua, they only serve a documentation purpose on the wiki!
* {{DB}} Integers labeled as <code>ImprovementType</code> corresponds to the ''ID'' column of the {{Table5|Improvements|CIV5Improvements}} XML table.
}}


= XML: the Improvements table =
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
|IMPROVEMENT_CITY_RUINS
|-
|align="right"|0
|
|IMPROVEMENT_HOLY_SITE
|-
|align="right"|1
|
|IMPROVEMENT_BARBARIAN_CAMP
|-
|align="right"|1
|
|IMPROVEMENT_POLDER
|-
|align="right"|2
|
|IMPROVEMENT_GOODY_HUT
|-
|align="right"|3
|
|IMPROVEMENT_FARM
|-
|align="right"|4
|
|IMPROVEMENT_MINE
|-
|align="right"|5
|
|IMPROVEMENT_QUARRY
|-
|align="right"|6
|
|IMPROVEMENT_TRADING_POST
|-
|align="right"|7
|
|IMPROVEMENT_LUMBERMILL
|-
|align="right"|8
|
|IMPROVEMENT_PASTURE
|-
|align="right"|9
|
|IMPROVEMENT_FISHING_BOATS
|-
|align="right"|10
|
|IMPROVEMENT_PLANTATION
|-
|align="right"|11
|
|IMPROVEMENT_CAMP
|-
|align="right"|12
|
|IMPROVEMENT_WELL
|-
|align="right"|13
|
|IMPROVEMENT_OFFSHORE_PLATFORM
|-
|align="right"|14
|
|IMPROVEMENT_FORT
|-
|align="right"|15
|
|IMPROVEMENT_LANDMARK
|-
|align="right"|16
|
|IMPROVEMENT_ACADEMY
|-
|align="right"|17
|
|IMPROVEMENT_CUSTOMS_HOUSE
|-
|align="right"|18
|
|IMPROVEMENT_MANUFACTORY
|-
|align="right"|19
|
|IMPROVEMENT_CITADEL
|}</code>


= Examples =
Here are different ways to query the database to retrieve the ''ID'' from the ''type''. Those examples will return and assign the integer value 0. See also {{Type5|GameInfo}}.
<syntaxhighlight lang="lua" class="civ5-example">
local id = GameInfo.Improvements.IMPROVEMENT_HOLY_SITE.ID
local id = GameInfo["Improvements"].["IMPROVEMENT_HOLY_SITE"].ID
local id = GameInfo.Improvements{Type="IMPROVEMENT_HOLY_SITE"}().ID
</syntaxhighlight>
Alternatively you could use the ''ID'' or the ''type'' to retrieve the value of the ''Description'' column. Those examples will return and assign the value TXT_KEY_IMPROVEMENT_HOLY_SITE.
<syntaxhighlight lang="lua" class="civ5-example">
local description = GameInfo.Improvements[0].Description
local description = GameInfo["Improvements"][0]["Description"]
local description = GameInfo.Improvements{ID=0}().Description
</syntaxhighlight>


=Used by=
{|cellspacing="4" cellpadding="0" width="100%" style="background-color:#F0F0F0"
<!-- 
CANPLACEGOODYAT
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Func5|CanPlaceGoodyAt}}<b>(</b>{{Type5|ImprovementType}} improvement, {{Type5|Plot}} plot<b>)</b></code>
<!-- 
GETHELPTEXTFORIMPROVEMENT
-->
|-
|align="right" width="200" |<code>'''string'''</code>
|style="padding-left:6px" |<code>{{Func5|GetHelpTextForImprovement}}<b>(</b>{{Type5|ImprovementType}} improvement, '''bool''' excludeName, '''bool''' excludeHeader, '''bool''' noMaintenance<b>)</b></code>
<!-- 
GETNUMIMPROVEMENTS
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Area}}:{{Func5|Area|GetNumImprovements}}<b>(</b>{{Type5|ImprovementType}} improvement<b>)</b></code>
<!-- 
GOTOPEDIAHOMEPAGE
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Events}}.{{Func5|Events|GoToPediaHomePage}}<b>(</b>{{Type5|ImprovementType}} homePage<b>)</b></code>
<!-- 
SERIALEVENTIMPROVEMENTCREATED
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Events}}.{{Func5|Events|SerialEventImprovementCreated}}<b>(</b>'''float''' hexX, '''int''' hexY, {{Type5|ArtStyleType}} continent1, {{Type5|ArtStyleType}} continent2, {{Type5|PlayerID}} player, '''int''' createImprovementType, {{Type5|ImprovementType}} createImprovementRRType, '''int''' createImprovementEra, '''int''' createImprovementState, '''unknown''' ImprovementEra = nil<b>)</b></code>
<!-- 
GETIMPROVEMENTUPGRADETIME
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Game}}.{{Func5|Game|GetImprovementUpgradeTime}}<b>(</b>{{Type5|ImprovementType}} improvement, {{Type5|Plot}} plot<b>)</b></code>
<!-- 
GETADVANCEDSTARTIMPROVEMENTCOST
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|GetAdvancedStartImprovementCost}}<b>(</b>{{Type5|ImprovementType}} improvement, '''bool''' add, {{Type5|Plot}} plot<b>)</b></code>
<!-- 
GETIMPROVEMENTCOUNT
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|GetImprovementCount}}<b>(</b>{{Type5|ImprovementType}} improvement<b>)</b></code>
<!-- 
CALCULATEIMPROVEMENTYIELDCHANGE
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Plot}}:{{Func5|Plot|CalculateImprovementYieldChange}}<b>(</b>{{Type5|ImprovementType}} improvement, {{Type5|YieldType}} yield, {{Type5|PlayerID}} player, '''bool''' optimal, {{Type5|RouteType}} assumeThisRoute<b>)</b></code>
<!-- 
CANHAVEIMPROVEMENT
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|Plot}}:{{Func5|Plot|CanHaveImprovement}}<b>(</b>{{Type5|ImprovementType}} improvement, {{Type5|TeamID}} team, '''bool''' potential<b>)</b></code>
<!-- 
GETIMPROVEMENTTYPE
-->
|-
|align="right" width="200" |<code>{{Type5|ImprovementType}}</code>
|style="padding-left:6px" |<code>{{Type5|Plot}}:{{Func5|Plot|GetImprovementType}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETREVEALEDIMPROVEMENTTYPE
-->
|-
|align="right" width="200" |<code>{{Type5|ImprovementType}}</code>
|style="padding-left:6px" |<code>{{Type5|Plot}}:{{Func5|Plot|GetRevealedImprovementType}}<b>(</b>{{Type5|TeamID}} team, '''bool''' debug<b>)</b></code>
<!-- 
GETUPGRADETIMELEFT
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Plot}}:{{Func5|Plot|GetUpgradeTimeLeft}}<b>(</b>{{Type5|ImprovementType}} improvement, {{Type5|PlayerID}} player<b>)</b></code>
<!-- 
ISRESOURCECONNECTEDBYIMPROVEMENT
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|Plot}}:{{Func5|Plot|IsResourceConnectedByImprovement}}<b>(</b>{{Type5|ImprovementType}} improvement<b>)</b></code>
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
[[Category:Civ5 Types|ImprovementType]]