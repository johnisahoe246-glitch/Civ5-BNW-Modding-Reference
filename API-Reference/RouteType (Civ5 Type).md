{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|ID.png|The <code>RouteType</code> pseudo-type is actually a regular '''integer'''. Pseudo-types do not exist in Lua, they only serve a documentation purpose on the wiki!
* {{DB}} Integers labeled as <code>RouteType</code> corresponds to the ''ID'' column of the {{Table5|Routes|CIV5Routes}} XML table.
}}


= XML: the Routes table =
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
|ROUTE_ROAD
|-
|align="right"|1
|
|ROUTE_RAILROAD
|}</code>


= Examples =
Here are different ways to query the database to retrieve the ''ID'' from the ''type''. Those examples will return and assign the integer value 0. See also {{Type5|GameInfo}}.
<syntaxhighlight lang="lua" class="civ5-example">
local id = GameInfo.Routes.ROUTE_ROAD.ID
local id = GameInfo["Routes"].["ROUTE_ROAD"].ID
local id = GameInfo.Routes{Type="ROUTE_ROAD"}().ID
</syntaxhighlight>
Alternatively you could use the ''ID'' or the ''type'' to retrieve the value of the ''Description'' column. Those examples will return and assign the value TXT_KEY_ROUTE_ROAD.
<syntaxhighlight lang="lua" class="civ5-example">
local description = GameInfo.Routes[0].Description
local description = GameInfo["Routes"][0]["Description"]
local description = GameInfo.Routes{ID=0}().Description
</syntaxhighlight>


=Used by=
{|cellspacing="4" cellpadding="0" width="100%" style="background-color:#F0F0F0"
<!-- 
GETADVANCEDSTARTROUTECOST
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|GetAdvancedStartRouteCost}}<b>(</b>{{Type5|RouteType}} route, '''bool''' add, {{Type5|Plot}} plot<b>)</b></code>
<!-- 
CALCULATEIMPROVEMENTYIELDCHANGE
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Plot}}:{{Func5|Plot|CalculateImprovementYieldChange}}<b>(</b>{{Type5|ImprovementType}} improvement, {{Type5|YieldType}} yield, {{Type5|PlayerID}} player, '''bool''' optimal, {{Type5|RouteType}} assumeThisRoute<b>)</b></code>
<!-- 
GETREVEALEDROUTETYPE
-->
|-
|align="right" width="200" |<code>{{Type5|RouteType}}</code>
|style="padding-left:6px" |<code>{{Type5|Plot}}:{{Func5|Plot|GetRevealedRouteType}}<b>(</b>{{Type5|TeamID}} team, '''bool''' debug<b>)</b></code>
<!-- 
GETROUTETYPE
-->
|-
|align="right" width="200" |<code>{{Type5|RouteType}}</code>
|style="padding-left:6px" |<code>{{Type5|Plot}}:{{Func5|Plot|GetRouteType}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
CHANGEROUTECHANGE
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Team}}:{{Func5|Team|ChangeRouteChange}}<b>(</b>{{Type5|RouteType}} index, '''int''' change<b>)</b></code>
<!-- 
GETROUTECHANGE
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Team}}:{{Func5|Team|GetRouteChange}}<b>(</b>{{Type5|RouteType}} index<b>)</b></code>
|}




{{Civ5 API Footer}}
[[Category:Civ5 Types|RouteType]]