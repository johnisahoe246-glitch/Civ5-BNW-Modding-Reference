{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>

Plots apparently have an equality operator handler, i.e. two variables of plot type can be compared directly without having to compare both their X and Y coordinates.

=Instance Methods=
Methods are functions that belong to an object. Instance methods are invoked through a '''colon''', as in <code>caller:SomeMethod(&lt;args&gt;)</code>, where ''caller'' is an instance of Plot.<br/>
A colon implictly passes the caller object as the first argument. That is, the former call is equivalent to this one: <code>caller.SomeMethod(caller, &lt;args&gt;)</code>
==A==
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
ADDFEATUREDUMMYMODEL
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Plot|AddFeatureDummyModel}}<b>(</b>'''string''' dummyTag, '''string''' modelTag<b>)</b></code>
<!-- 
AREA
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>{{Type5|Area}}</code>
|width="100%" |<code>{{FuncLabel5|Plot|Area}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
AT
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Plot|At}}<b>(</b>'''int''' x, '''int''' y<b>)</b></code>
|}

==C==
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
CALCULATEBESTNATUREYIELD
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Plot|CalculateBestNatureYield}}<b>(</b>{{Type5|YieldType}} index, {{Type5|TeamID}} team<b>)</b></code>
<!-- 
CALCULATEIMPROVEMENTYIELDCHANGE
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Plot|CalculateImprovementYieldChange}}<b>(</b>{{Type5|ImprovementType}} improvement, {{Type5|YieldType}} yield, {{Type5|PlayerID}} player, '''bool''' optimal, {{Type5|RouteType}} assumeThisRoute<b>)</b></code>
<!-- 
CALCULATENATUREYIELD
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Plot|CalculateNatureYield}}<b>(</b>{{Type5|YieldType}} index, {{Type5|TeamID}} team, '''bool''' ignoreFeature = false<b>)</b></code>
<!-- 
CALCULATETOTALBESTNATUREYIELD
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Plot|CalculateTotalBestNatureYield}}<b>(</b>{{Type5|TeamID}} team<b>)</b></code>
<!-- 
CALCULATEYIELD
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Plot|CalculateYield}}<b>(</b>{{Type5|YieldType}} index, '''bool''' display<b>)</b></code>
<!-- 
CANBUILD
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Plot|CanBuild}}<b>(</b>{{Type5|BuildActionType}} build, {{Type5|PlayerID}} player, '''bool''' testVisible<b>)</b></code>
<!-- 
CANHAVEFEATURE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Plot|CanHaveFeature}}<b>(</b>{{Type5|FeatureType}} featureForest<b>)</b></code>
<!-- 
CANHAVEIMPROVEMENT
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Plot|CanHaveImprovement}}<b>(</b>{{Type5|ImprovementType}} improvement, {{Type5|TeamID}} team, '''bool''' potential<b>)</b></code>
<!-- 
CANHAVERESOURCE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Plot|CanHaveResource}}<b>(</b>{{Type5|ResourceType}} resource, '''bool''' ignoreLatitude<b>)</b></code>
<!-- 
CANSEEPLOT
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Plot|CanSeePlot}}<b>(</b>{{Type5|Plot}} target, {{Type5|TeamID}} team, '''int''' range<b>)</b></code>
<!-- 
CHANGEBUILDPROGRESS
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Plot|ChangeBuildProgress}}<b>(</b>{{Type5|BuildActionType}} build, '''int''' change, {{Type5|TeamID}} team<b>)</b></code>
<!-- 
CHANGEEXTRAMOVEPATHCOST
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Plot|ChangeExtraMovePathCost}}<b>(</b>'''int''' change<b>)</b></code>
<!-- 
CHANGEIMPROVEMENTDURATION
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Plot|ChangeImprovementDuration}}<b>(</b>'''int''' change<b>)</b></code>
<!-- 
CHANGEINVISIBLEVISIBILITYCOUNT
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Plot|ChangeInvisibleVisibilityCount}}<b>(</b>{{Type5|TeamID}} team, {{Type5|InvisibilityScopeType}} invisible, '''int''' change<b>)</b></code>
<!-- 
CHANGENUMRESOURCE
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Plot|ChangeNumResource}}<b>(</b>'''int''' change<b>)</b></code>
<!-- 
CHANGEOWNERSHIPDURATION
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Plot|ChangeOwnershipDuration}}<b>(</b>'''int''' change<b>)</b></code>
<!-- 
CHANGEUPGRADEPROGRESS
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Plot|ChangeUpgradeProgress}}<b>(</b>'''int''' change<b>)</b></code>
<!-- 
CHANGEVISIBILITYCOUNT
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Plot|ChangeVisibilityCount}}<b>(</b>{{Type5|TeamID}} team, '''int''' change, {{Type5|InvisibilityScopeType}} seeInvisibleType, '''bool''' informExplorationTracking, '''bool''' alwaysSeeInvisible<b>)</b></code>
<!-- 
COUNTNUMAIRUNITS
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Plot|CountNumAirUnits}}<b>(</b>{{Type5|PlayerID}} player<b>)</b></code>
|}

==D==
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
DEFENSEMODIFIER
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Plot|DefenseModifier}}<b>(</b>{{Type5|TeamID}} defendTeam, '''bool''' ignoreBuilding, '''bool''' help<b>)</b></code>
|}

==E==
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
ERASE
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>{{UnknownSignature5}}</code>
|width="100%" |<code>{{FuncLabel5|Plot|Erase}}<!-- No arguments --></code>
|}

==G==
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
GETACTIVEFOGOFWARMODE
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>{{UnknownSignature5}}</code>
|width="100%" |<code>{{FuncLabel5|Plot|GetActiveFogOfWarMode}}<!-- No arguments --></code>
<!-- 
GETAREA
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>{{Type5|AreaID}}</code>
|width="100%" |<code>{{FuncLabel5|Plot|GetArea}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETBESTDEFENDER
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''unknown'''</code>
|width="100%" |<code>{{FuncLabel5|Plot|GetBestDefender}}<b>(</b>{{Type5|PlayerID}} owner, {{Type5|PlayerID}} attackingPlayer, {{Type5|Unit}} attacker, '''bool''' testAtWar, '''bool''' testPotentialEnemy, '''bool''' testCanMove<b>)</b></code>
<!-- 
GETBUILDPROGRESS
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Plot|GetBuildProgress}}<b>(</b>{{Type5|BuildActionType}} build<b>)</b></code>
<!-- 
GETBUILDTIME
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Plot|GetBuildTime}}<b>(</b>{{Type5|BuildActionType}} build<b>)</b></code>
<!-- 
GETBUILDTURNSLEFT
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Plot|GetBuildTurnsLeft}}<b>(</b>{{Type5|BuildActionType}} build, '''int''' nowExtra, '''int''' thenExtra<b>)</b></code>
<!-- 
GETBUILDTURNSTOTAL
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Plot|GetBuildTurnsTotal}}<b>(</b>{{Type5|BuildActionType}} build<b>)</b></code>
<!-- 
GETCITYRADIUSCOUNT
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Plot|GetCityRadiusCount}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETCONTINENTARTTYPE
-->
|-
{{FuncInfos5|yes  |yes  |yes|Determines continent for plot type.}}
|align="right"  |<code>{{Type5|ArtStyleType}}</code>
|width="100%" |<code>{{FuncLabel5|Plot|GetContinentArtType}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETCULTURE
-->
|-
{{FuncInfos5|yes  |no   |yes|Determines the amount of culture yielded by working the plot.}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Plot|GetCulture}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETEXTRAMOVEPATHCOST
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Plot|GetExtraMovePathCost}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETFEATUREPRODUCTION
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Plot|GetFeatureProduction}}<b>(</b>{{Type5|BuildActionType}} build, {{Type5|TeamID}} team, {{Type5|City}} city<b>)</b></code>
<!-- 
GETFEATURETYPE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>{{Type5|FeatureType}}</code>
|width="100%" |<code>{{FuncLabel5|Plot|GetFeatureType}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETFEATUREVARIETY
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Plot|GetFeatureVariety}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETFOUNDVALUE
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Plot|GetFoundValue}}<b>(</b>{{Type5|PlayerID}} index<b>)</b></code>
<!-- 
GETIMPROVEMENTDURATION
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Plot|GetImprovementDuration}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETIMPROVEMENTTYPE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>{{Type5|ImprovementType}}</code>
|width="100%" |<code>{{FuncLabel5|Plot|GetImprovementType}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETINLANDCORNER
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>{{Type5|Plot}}</code>
|width="100%" |<code>{{FuncLabel5|Plot|GetInlandCorner}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETINVISIBLEVISIBILITYCOUNT
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Plot|GetInvisibleVisibilityCount}}<b>(</b>{{Type5|TeamID}} team, {{Type5|InvisibilityScopeType}} invisible<b>)</b></code>
<!-- 
GETLATITUDE
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Plot|GetLatitude}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETNEARESTLANDAREA
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>{{Type5|AreaID}}</code>
|width="100%" |<code>{{FuncLabel5|Plot|GetNearestLandArea}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETNEARESTLANDPLOT
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>{{Type5|Plot}}</code>
|width="100%" |<code>{{FuncLabel5|Plot|GetNearestLandPlot}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETNONOBSOLETERESOURCETYPE
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>{{Type5|ResourceType}}</code>
|width="100%" |<code>{{FuncLabel5|Plot|GetNonObsoleteResourceType}}<b>(</b>{{Type5|TeamID}} team<b>)</b></code>
<!-- 
GETNUMDEFENDERS
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Plot|GetNumDefenders}}<b>(</b>{{Type5|PlayerID}} player<b>)</b></code>
<!-- 
GETNUMFRIENDLYUNITSOFTYPE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Plot|GetNumFriendlyUnitsOfType}}<b>(</b>{{Type5|Unit}} unit<b>)</b></code>
<!-- 
GETNUMRESOURCE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Plot|GetNumResource}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETNUMUNITS
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Plot|GetNumUnits}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETNUMVISIBLEENEMYDEFENDERS
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Plot|GetNumVisibleEnemyDefenders}}<b>(</b>{{Type5|Unit}} unit<b>)</b></code>
<!-- 
GETNUMVISIBLEPOTENTIALENEMYDEFENDERS
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Plot|GetNumVisiblePotentialEnemyDefenders}}<b>(</b>{{Type5|Unit}} unit<b>)</b></code>
<!-- 
GETOWNER
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>{{Type5|PlayerID}}</code>
|width="100%" |<code>{{FuncLabel5|Plot|GetOwner}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETOWNERSHIPDURATION
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Plot|GetOwnershipDuration}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETPLAYERCITYRADIUSCOUNT
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Plot|GetPlayerCityRadiusCount}}<b>(</b>{{Type5|PlayerID}} index<b>)</b></code>
<!-- 
GETPLOTCITY
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Plot|GetPlotCity}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETPLOTTYPE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>{{Type5|PlotType}}</code>
|width="100%" |<code>{{FuncLabel5|Plot|GetPlotType}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETRECONCOUNT
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Plot|GetReconCount}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETRESOURCETYPE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>{{Type5|ResourceType}}</code>
|width="100%" |<code>{{FuncLabel5|Plot|GetResourceType}}<b>(</b>{{Type5|TeamID}} team<b>)</b></code>
<!-- 
GETREVEALEDIMPROVEMENTTYPE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>{{Type5|ImprovementType}}</code>
|width="100%" |<code>{{FuncLabel5|Plot|GetRevealedImprovementType}}<b>(</b>{{Type5|TeamID}} team, '''bool''' debug<b>)</b></code>
<!-- 
GETREVEALEDOWNER
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>{{Type5|PlayerID}}</code>
|width="100%" |<code>{{FuncLabel5|Plot|GetRevealedOwner}}<b>(</b>{{Type5|TeamID}} team, '''bool''' debug<b>)</b></code>
<!-- 
GETREVEALEDROUTETYPE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>{{Type5|RouteType}}</code>
|width="100%" |<code>{{FuncLabel5|Plot|GetRevealedRouteType}}<b>(</b>{{Type5|TeamID}} team, '''bool''' debug<b>)</b></code>
<!-- 
GETREVEALEDTEAM
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>{{Type5|TeamID}}</code>
|width="100%" |<code>{{FuncLabel5|Plot|GetRevealedTeam}}<b>(</b>{{Type5|TeamID}} team, '''bool''' debug<b>)</b></code>
<!-- 
GETRIVERCROSSINGCOUNT
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Plot|GetRiverCrossingCount}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETRIVEREFLOWDIRECTION
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>{{Type5|FlowDirectionType}}</code>
|width="100%" |<code>{{FuncLabel5|Plot|GetRiverEFlowDirection}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETRIVERSEFLOWDIRECTION
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>{{Type5|FlowDirectionType}}</code>
|width="100%" |<code>{{FuncLabel5|Plot|GetRiverSEFlowDirection}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETRIVERSWFLOWDIRECTION
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>{{Type5|FlowDirectionType}}</code>
|width="100%" |<code>{{FuncLabel5|Plot|GetRiverSWFlowDirection}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETROUTETYPE
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>{{Type5|RouteType}}</code>
|width="100%" |<code>{{FuncLabel5|Plot|GetRouteType}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETSCRIPTDATA
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''string'''</code>
|width="100%" |<code>{{FuncLabel5|Plot|GetScriptData}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETSELECTEDUNIT
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''unknown'''</code>
|width="100%" |<code>{{FuncLabel5|Plot|GetSelectedUnit}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETTEAM
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>{{Type5|TeamID}}</code>
|width="100%" |<code>{{FuncLabel5|Plot|GetTeam}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETTERRAINTYPE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>{{Type5|TerrainType}}</code>
|width="100%" |<code>{{FuncLabel5|Plot|GetTerrainType}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETUNIT
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>{{Type5|Unit}}</code>
|width="100%" |<code>{{FuncLabel5|Plot|GetUnit}}<b>(</b>{{Type5|UnitID}} id<b>)</b></code>
<!-- 
GETUNITPOWER
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Plot|GetUnitPower}}<b>(</b>{{Type5|PlayerID}} owner<b>)</b></code>
<!-- 
GETUPGRADEPROGRESS
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Plot|GetUpgradeProgress}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETUPGRADETIMELEFT
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Plot|GetUpgradeTimeLeft}}<b>(</b>{{Type5|ImprovementType}} improvement, {{Type5|PlayerID}} player<b>)</b></code>
<!-- 
GETVISIBILITYCOUNT
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Plot|GetVisibilityCount}}<b>(</b>{{Type5|TeamID}} team<b>)</b></code>
<!-- 
GETWORKINGCITY
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>{{Type5|City}}</code>
|width="100%" |<code>{{FuncLabel5|Plot|GetWorkingCity}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETWORKINGCITYOVERRIDE
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''unknown'''</code>
|width="100%" |<code>{{FuncLabel5|Plot|GetWorkingCityOverride}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETX
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Plot|GetX}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETY
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Plot|GetY}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETYIELD
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Plot|GetYield}}<b>(</b>{{Type5|YieldType}} index<b>)</b></code>
<!-- 
GETYIELDWITHBUILD
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Plot|GetYieldWithBuild}}<b>(</b>{{Type5|BuildActionType}} build, {{Type5|YieldType}} yield, '''bool''' arg2, {{Type5|PlayerID}} activePlayer<b>)</b></code>
|}

==H==
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
HASBARBARIANCAMP
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Plot|HasBarbarianCamp}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
HASYIELD
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Plot|HasYield}}<b>(</b>{{Type5|YieldType}} yield<b>)</b></code>
|}

==I==
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
ISACTIVEVISIBLE
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Plot|IsActiveVisible}}<b>(</b>'''bool''' debug<b>)</b></code>
<!-- 
ISADJACENTNONREVEALED
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Plot|IsAdjacentNonrevealed}}<b>(</b>{{Type5|TeamID}} team<b>)</b></code>
<!-- 
ISADJACENTNONVISIBLE
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Plot|IsAdjacentNonvisible}}<b>(</b>{{Type5|TeamID}} team<b>)</b></code>
<!-- 
ISADJACENTOWNED
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Plot|IsAdjacentOwned}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ISADJACENTPLAYER
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Plot|IsAdjacentPlayer}}<b>(</b>{{Type5|PlayerID}} player, '''bool''' landOnly<b>)</b></code>
<!-- 
ISADJACENTREVEALED
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Plot|IsAdjacentRevealed}}<b>(</b>{{Type5|TeamID}} team<b>)</b></code>
<!-- 
ISADJACENTTEAM
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Plot|IsAdjacentTeam}}<b>(</b>{{Type5|TeamID}} team, '''bool''' landOnly<b>)</b></code>
<!-- 
ISADJACENTTOAREA
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Plot|IsAdjacentToArea}}<b>(</b>{{Type5|Area}} area<b>)</b></code>
<!-- 
ISADJACENTTOLAND
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Plot|IsAdjacentToLand}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ISADJACENTTOSHALLOWWATER
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Plot|IsAdjacentToShallowWater}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ISADJACENTVISIBLE
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Plot|IsAdjacentVisible}}<b>(</b>{{Type5|TeamID}} team, '''bool''' debug<b>)</b></code>
<!-- 
ISBARBARIAN
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Plot|IsBarbarian}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ISBEINGWORKED
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Plot|IsBeingWorked}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ISBESTADJACENTFOUND
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Plot|IsBestAdjacentFound}}<b>(</b>{{Type5|PlayerID}} index<b>)</b></code>
<!-- 
ISBUILDREMOVESFEATURE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Plot|IsBuildRemovesFeature}}<b>(</b>{{Type5|BuildActionType}} build<b>)</b></code>
<!-- 
ISCITY
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Plot|IsCity}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ISCITYRADIUS
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Plot|IsCityRadius}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ISCOASTALLAND
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Plot|IsCoastalLand}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ISENEMYCITY
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Plot|IsEnemyCity}}<b>(</b>{{Type5|Unit}} unit<b>)</b></code>
<!-- 
ISFIGHTING
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Plot|IsFighting}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ISFLATLANDS
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Plot|IsFlatlands}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ISFRESHWATER
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Plot|IsFreshWater}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ISFRIENDLYCITY
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Plot|IsFriendlyCity}}<b>(</b>{{Type5|Unit}} unit, '''bool''' checkImprovement<b>)</b></code>
<!-- 
ISFRIENDLYTERRITORY
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Plot|IsFriendlyTerritory}}<b>(</b>{{Type5|PlayerID}} player<b>)</b></code>
<!-- 
ISGOODY
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Plot|IsGoody}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ISHILLS
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Plot|IsHills}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ISIMPASSABLE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Plot|IsImpassable}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ISIMPROVEMENTPILLAGED
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Plot|IsImprovementPillaged}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ISINVISIBLEVISIBLE
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Plot|IsInvisibleVisible}}<b>(</b>{{Type5|TeamID}} team, {{Type5|InvisibilityScopeType}} invisible<b>)</b></code>
<!-- 
ISLAKE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Plot|IsLake}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ISMOUNTAIN
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Plot|IsMountain}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ISNEOFRIVER
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Plot|IsNEOfRiver}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ISNONE
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Plot|IsNone}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ISNWOFRIVER
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Plot|IsNWOfRiver}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ISOPENGROUND
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Plot|IsOpenGround}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ISOWNED
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Plot|IsOwned}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ISOWNERSHIPSCORE
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Plot|IsOwnershipScore}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ISPLAYERCITYRADIUS
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Plot|IsPlayerCityRadius}}<b>(</b>{{Type5|PlayerID}} index<b>)</b></code>
<!-- 
ISPOTENTIALCITYWORK
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Plot|IsPotentialCityWork}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ISPOTENTIALCITYWORKFORAREA
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Plot|IsPotentialCityWorkForArea}}<b>(</b>{{Type5|Area}} area<b>)</b></code>
<!-- 
ISRESOURCECONNECTEDBYIMPROVEMENT
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Plot|IsResourceConnectedByImprovement}}<b>(</b>{{Type5|ImprovementType}} improvement<b>)</b></code>
<!-- 
ISREVEALED
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Plot|IsRevealed}}<b>(</b>{{Type5|TeamID}} team, '''bool''' debug<b>)</b></code>
<!-- 
ISREVEALEDBARBARIAN
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Plot|IsRevealedBarbarian}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ISREVEALEDGOODY
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Plot|IsRevealedGoody}}<b>(</b>{{Type5|TeamID}} team<b>)</b></code>
<!-- 
ISRIVER
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Plot|IsRiver}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ISRIVERCONNECTION
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Plot|IsRiverConnection}}<b>(</b>{{Type5|DirectionType}} direction<b>)</b></code>
<!-- 
ISRIVERCROSSING
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Plot|IsRiverCrossing}}<b>(</b>{{Type5|DirectionType}} index<b>)</b></code>
<!-- 
ISRIVERCROSSINGFLOWCLOCKWISE
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Plot|IsRiverCrossingFlowClockwise}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ISRIVERCROSSINGTOPLOT
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Plot|IsRiverCrossingToPlot}}<b>(</b>{{Type5|DirectionType}} index<b>)</b></code>
<!-- 
ISRIVERSIDE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Plot|IsRiverSide}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ISROUGHGROUND
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Plot|IsRoughGround}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ISROUTE
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Plot|IsRoute}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ISROUTEPILLAGED
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Plot|IsRoutePillaged}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ISSTARTINGPLOT
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Plot|IsStartingPlot}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ISTRADEROUTE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Plot|IsTradeRoute}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ISUNIT
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Plot|IsUnit}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ISVALIDDOMAINFORACTION
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Plot|IsValidDomainForAction}}<b>(</b>{{Type5|Unit}} unit<b>)</b></code>
<!-- 
ISVALIDDOMAINFORLOCATION
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Plot|IsValidDomainForLocation}}<b>(</b>{{Type5|Unit}} unit<b>)</b></code>
<!-- 
ISVISIBLE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Plot|IsVisible}}<b>(</b>{{Type5|TeamID}} team, '''bool''' debug<b>)</b></code>
<!-- 
ISVISIBLEENEMYDEFENDER
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Plot|IsVisibleEnemyDefender}}<b>(</b>{{Type5|Unit}} unit<b>)</b></code>
<!-- 
ISVISIBLEENEMYUNIT
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Plot|IsVisibleEnemyUnit}}<b>(</b>{{Type5|PlayerID}} player<b>)</b></code>
<!-- 
ISVISIBLEOTHERUNIT
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Plot|IsVisibleOtherUnit}}<b>(</b>{{Type5|PlayerID}} player<b>)</b></code>
<!-- 
ISVISIBLETOWATCHINGHUMAN
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Plot|IsVisibleToWatchingHuman}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ISWATER
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Plot|IsWater}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ISWITHINTEAMCITYRADIUS
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Plot|IsWithinTeamCityRadius}}<b>(</b>{{Type5|TeamID}} team, {{Type5|PlayerID}} ignorePlayer<b>)</b></code>
<!-- 
ISWOFRIVER
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Plot|IsWOfRiver}}<b>(</b><!-- No arguments --><b>)</b></code>
|}

==M==
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
MOVEMENTCOST
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Plot|MovementCost}}<b>(</b>{{Type5|Unit}} unit, {{Type5|Plot}} fromPlot<b>)</b></code>
|}

==N==
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
NUKEEXPLOSION
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Plot|NukeExplosion}}<b>(</b>'''int''' range, {{Type5|Unit}} nukeUnit<b>)</b></code>
|}

==P==
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
PICKFEATUREDUMMYTAG
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''string'''</code>
|width="100%" |<code>{{FuncLabel5|Plot|PickFeatureDummyTag}}<b>(</b>'''int''' mouseX, '''int''' mouseY<b>)</b></code>
|}

==R==
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
REMOVEGOODY
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>{{UnknownSignature5}}</code>
|width="100%" |<code>{{FuncLabel5|Plot|RemoveGoody}}<!-- No arguments --></code>
<!-- 
RESETFEATUREMODEL
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>{{UnknownSignature5}}</code>
|width="100%" |<code>{{FuncLabel5|Plot|ResetFeatureModel}}<!-- No arguments --></code>
|}

==S==
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
SEEFROMLEVEL
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Plot|SeeFromLevel}}<b>(</b>{{Type5|TeamID}} team<b>)</b></code>
<!-- 
SEETHROUGHLEVEL
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Plot|SeeThroughLevel}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
SETAREA
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Plot|SetArea}}<b>(</b>{{Type5|AreaID}} area<b>)</b></code>
<!-- 
SETCONTINENTARTTYPE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Plot|SetContinentArtType}}<b>(</b>{{Type5|ArtStyleType}} style<b>)</b></code>
<!-- 
SETFEATUREDUMMYTEXTURE
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Plot|SetFeatureDummyTexture}}<b>(</b>'''string''' dummyTag, '''string''' textureTag<b>)</b></code>
<!-- 
SETFEATUREDUMMYVISIBILITY
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Plot|SetFeatureDummyVisibility}}<b>(</b>'''string''' dummyTag, '''bool''' show<b>)</b></code>
<!-- 
SETFEATURETYPE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Plot|SetFeatureType}}<b>(</b>'''int''' featureID, '''int''' arg1 = nil<b>)</b></code>
<!-- 
SETIMPROVEMENTDURATION
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Plot|SetImprovementDuration}}<b>(</b>'''int''' newValue<b>)</b></code>
<!-- 
SETIMPROVEMENTPILLAGED
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Plot|SetImprovementPillaged}}<b>(</b>'''bool''' pillaged<b>)</b></code>
<!-- 
SETIMPROVEMENTTYPE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Plot|SetImprovementType}}<b>(</b>'''int''' newValue<b>)</b></code>
<!-- 
SETNEOFRIVER
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Plot|SetNEOfRiver}}<b>(</b>'''bool''' newValue<b>)</b></code>
<!-- 
SETNUMRESOURCE
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Plot|SetNumResource}}<b>(</b>'''int''' num<b>)</b></code>
<!-- 
SETNWOFRIVER
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Plot|SetNWOfRiver}}<b>(</b>'''bool''' newValue<b>)</b></code>
<!-- 
SETOWNER
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Plot|SetOwner}}<b>(</b>{{Type5|PlayerID}} newValue, '''int''' acquiringCityID, '''bool''' checkUnits = true, '''bool''' updateResources = true<b>)</b></code>
<!-- 
SETOWNERSHIPDURATION
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Plot|SetOwnershipDuration}}<b>(</b>'''int''' newValue<b>)</b></code>
<!-- 
SETPLOTTYPE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Plot|SetPlotType}}<b>(</b>{{Type5|PlotType}} terrain, '''bool''' recalculateAreas = nil, '''bool''' rebuildGraphics) = nil<b>)</b></code>
<!-- 
SETRESOURCETYPE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Plot|SetResourceType}}<b>(</b>'''int''' newValue, {{Type5|ResourceType}} numResource<b>)</b></code>
<!-- 
SETREVEALED
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Plot|SetRevealed}}<b>(</b>{{Type5|TeamID}} team, '''bool''' newValue, '''bool''' terrainOnly, {{Type5|TeamID}} fromTeam<b>)</b></code>
<!-- 
SETROUTETYPE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Plot|SetRouteType}}<b>(</b>'''int''' newValue<b>)</b></code>
<!-- 
SETSCRIPTDATA
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Plot|SetScriptData}}<b>(</b>'''string''' newValue<b>)</b></code>
<!-- 
SETSTARTINGPLOT
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Plot|SetStartingPlot}}<b>(</b>'''bool''' newValue<b>)</b></code>
<!-- 
SETTERRAINTYPE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Plot|SetTerrainType}}<b>(</b>{{Type5|TerrainType}} terrain, '''bool''' recalculateAreas, '''bool''' rebuildGraphics)<b>)</b></code>
<!-- 
SETUPGRADEPROGRESS
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Plot|SetUpgradeProgress}}<b>(</b>'''int''' newValue<b>)</b></code>
<!-- 
SETWOFRIVER
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Plot|SetWOfRiver}}<b>(</b>'''bool''' newValue<b>)</b></code>
<!-- 
SHAREADJACENTAREA
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Plot|ShareAdjacentArea}}<b>(</b>{{Type5|Plot}} plot<b>)</b></code>
|}

==U==
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
UPDATEFOG
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>{{UnknownSignature5}}</code>
|width="100%" |<code>{{FuncLabel5|Plot|UpdateFog}}<!-- No arguments --></code>
<!-- 
UPDATEVISIBILITY
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>{{UnknownSignature5}}</code>
|width="100%" |<code>{{FuncLabel5|Plot|UpdateVisibility}}<!-- No arguments --></code>
|}

==W==
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
WATERAREA
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>{{UnknownSignature5}}</code>
|width="100%" |<code>{{FuncLabel5|Plot|WaterArea}}<!-- No arguments --></code>
|}


=Used by=
{|cellspacing="4" cellpadding="0" width="100%" style="background-color:#F0F0F0"
<!-- 
CANPLACEGOODYAT
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Func5|CanPlaceGoodyAt}}<b>(</b>{{Type5|ImprovementType}} improvement, {{Type5|Plot}} plot<b>)</b></code>
<!-- 
DORIVER
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Func5|DoRiver}}<b>(</b>{{Type5|Plot}} startPlot, {{Type5|FlowDirectionType}} thisFlowDirection = nil, {{Type5|FlowDirectionType}} originalFlowDirection = nil, '''int''' riverID = nil<b>)</b></code>
<!-- 
GETCIVSTATEQUESTSTRING
-->
|-
|align="right" width="200" |<code>'''string'''</code>
|style="padding-left:6px" |<code>{{Func5|GetCivStateQuestString}}<b>(</b>{{Type5|Plot}} plot, '''bool''' shortVersion<b>)</b></code>
<!-- 
GETIMPROVEMENTSTRING
-->
|-
|align="right" width="200" |<code>'''string'''</code>
|style="padding-left:6px" |<code>{{Func5|GetImprovementString}}<b>(</b>{{Type5|Plot}} plot<b>)</b></code>
<!-- 
GETNATURESTRING
-->
|-
|align="right" width="200" |<code>'''string'''</code>
|style="padding-left:6px" |<code>{{Func5|GetNatureString}}<b>(</b>{{Type5|Plot}} plot<b>)</b></code>
<!-- 
GETOWNERSTRING
-->
|-
|align="right" width="200" |<code>'''string'''</code>
|style="padding-left:6px" |<code>{{Func5|GetOwnerString}}<b>(</b>{{Type5|Plot}} plot<b>)</b></code>
<!-- 
GETRESOURCESTRING
-->
|-
|align="right" width="200" |<code>'''string'''</code>
|style="padding-left:6px" |<code>{{Func5|GetResourceString}}<b>(</b>{{Type5|Plot}} plot, '''bool''' longForm<b>)</b></code>
<!-- 
GETRIVERVALUEATPLOT
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Func5|GetRiverValueAtPlot}}<b>(</b>{{Type5|Plot}} plot<b>)</b></code>
<!-- 
GETUNITSSTRING
-->
|-
|align="right" width="200" |<code>'''string'''</code>
|style="padding-left:6px" |<code>{{Func5|GetUnitsString}}<b>(</b>{{Type5|Plot}} plot<b>)</b></code>
<!-- 
GETYIELDSTRING
-->
|-
|align="right" width="200" |<code>'''string'''</code>
|style="padding-left:6px" |<code>{{Func5|GetYieldString}}<b>(</b>{{Type5|Plot}} plot<b>)</b></code>
<!-- 
ATPLOT
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|City}}:{{Func5|City|AtPlot}}<b>(</b>{{Type5|Plot}} plot<b>)</b></code>
<!-- 
CANWORK
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|City}}:{{Func5|City|CanWork}}<b>(</b>{{Type5|Plot}} plot<b>)</b></code>
<!-- 
GETCITYINDEXPLOT
-->
|-
|align="right" width="200" |<code>{{Type5|Plot}}</code>
|style="padding-left:6px" |<code>{{Type5|City}}:{{Func5|City|GetCityIndexPlot}}<b>(</b>{{Type5|CityPlotID}} index<b>)</b></code>
<!-- 
GETCITYPLOTINDEX
-->
|-
|align="right" width="200" |<code>{{Type5|CityPlotID}}</code>
|style="padding-left:6px" |<code>{{Type5|City}}:{{Func5|City|GetCityPlotIndex}}<b>(</b>{{Type5|Plot}} plot<b>)</b></code>
<!-- 
GETNUMFORCEDWORKINGPLOTS
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|City}}:{{Func5|City|GetNumForcedWorkingPlots}}<b>(</b>{{Type5|Plot}} plot<b>)</b></code>
<!-- 
ISFORCEDWORKINGPLOT
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|City}}:{{Func5|City|IsForcedWorkingPlot}}<b>(</b>{{Type5|Plot}} plot<b>)</b></code>
<!-- 
ISPLOTBLOCKADED
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|City}}:{{Func5|City|IsPlotBlockaded}}<b>(</b>{{Type5|Plot}} plot<b>)</b></code>
<!-- 
ISWORKINGPLOT
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|City}}:{{Func5|City|IsWorkingPlot}}<b>(</b>{{Type5|Plot}} plot<b>)</b></code>
<!-- 
PLOT
-->
|-
|align="right" width="200" |<code>{{Type5|Plot}}</code>
|style="padding-left:6px" |<code>{{Type5|City}}:{{Func5|City|Plot}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ADDFORESTSATPLOT
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|FeatureGenerator}}:{{Func5|FeatureGenerator|AddForestsAtPlot}}<b>(</b>{{Type5|Plot}} plot, '''int''' x, '''int''' y, '''int''' lat<b>)</b></code>
<!-- 
ADDICEATPLOT
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|FeatureGenerator}}:{{Func5|FeatureGenerator|AddIceAtPlot}}<b>(</b>{{Type5|Plot}} plot, '''int''' x, '''int''' y, '''int''' lat<b>)</b></code>
<!-- 
ADDJUNGLESATPLOT
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|FeatureGenerator}}:{{Func5|FeatureGenerator|AddJunglesAtPlot}}<b>(</b>{{Type5|Plot}} plot, '''int''' x, '''int''' y, '''int''' lat<b>)</b></code>
<!-- 
ADDMARSHATPLOT
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|FeatureGenerator}}:{{Func5|FeatureGenerator|AddMarshAtPlot}}<b>(</b>{{Type5|Plot}} plot, '''int''' x, '''int''' y, '''int''' lat<b>)</b></code>
<!-- 
ADDOASISATPLOT
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|FeatureGenerator}}:{{Func5|FeatureGenerator|AddOasisAtPlot}}<b>(</b>{{Type5|Plot}} plot, '''int''' x, '''int''' y, '''int''' lat<b>)</b></code>
<!-- 
CANHANDLEACTION
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|Game}}.{{Func5|Game|CanHandleAction}}<b>(</b>{{Type5|ActionType}} action, {{Type5|Plot}} plot = nil, '''bool''' testVisible = false<b>)</b></code>
<!-- 
CYCLEPLOTUNITS
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|Game}}.{{Func5|Game|CyclePlotUnits}}<b>(</b>{{Type5|Plot}} plot, '''bool''' forward, '''bool''' auto, '''int''' count<b>)</b></code>
<!-- 
GETIMPROVEMENTUPGRADETIME
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Game}}.{{Func5|Game|GetImprovementUpgradeTime}}<b>(</b>{{Type5|ImprovementType}} improvement, {{Type5|Plot}} plot<b>)</b></code>
<!-- 
SELECTIONLISTMOVE
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Game}}.{{Func5|Game|SelectionListMove}}<b>(</b>{{Type5|Plot}} plot, '''int''' alt, '''bool''' shift, '''int''' ctrl<b>)</b></code>
<!-- 
FINDWATER
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|Map}}.{{Func5|Map|FindWater}}<b>(</b>{{Type5|Plot}} plot, '''int''' range, '''bool''' isFreshWater<b>)</b></code>
<!-- 
GETPLOT
-->
|-
|align="right" width="200" |<code>{{Type5|Plot}}</code>
|style="padding-left:6px" |<code>{{Type5|Map}}.{{Func5|Map|GetPlot}}<b>(</b>'''int''' x, '''int''' y = nil<b>)</b></code>
<!-- 
GETPLOTBYINDEX
-->
|-
|align="right" width="200" |<code>{{Type5|Plot}}</code>
|style="padding-left:6px" |<code>{{Type5|Map}}.{{Func5|Map|GetPlotByIndex}}<b>(</b>{{Type5|PlotID}} index<b>)</b></code>
<!-- 
GETPLOTXY
-->
|-
|align="right" width="200" |<code>{{Type5|Plot}}</code>
|style="padding-left:6px" |<code>{{Type5|Map}}.{{Func5|Map|GetPlotXY}}<b>(</b>'''int''' x, '''int''' y, '''int''' xOffset, '''int''' yOffset<b>)</b></code>
<!-- 
PLOTDIRECTION
-->
|-
|align="right" width="200" |<code>{{Type5|Plot}}</code>
|style="padding-left:6px" |<code>{{Type5|Map}}.{{Func5|Map|PlotDirection}}<b>(</b>'''int''' x, '''int''' y<b>)</b></code>
<!-- 
PLOTXYWITHRANGECHECK
-->
|-
|align="right" width="200" |<code>{{Type5|Plot}}</code>
|style="padding-left:6px" |<code>{{Type5|Map}}.{{Func5|Map|PlotXYWithRangeCheck}}<b>(</b>'''int''' x, '''int''' y, '''int''' xOffset, '''int''' yOffset, '''int''' maxRange<b>)</b></code>
<!-- 
CANBUILD
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|CanBuild}}<b>(</b>{{Type5|Plot}} plot, {{Type5|BuildActionType}} build, '''bool''' testEra = false, '''bool''' testVisible = false, '''bool''' testGold = false<b>)</b></code>
<!-- 
CANRECEIVEGOODY
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|CanReceiveGoody}}<b>(</b>{{Type5|Plot}} plot, {{Type5|GoodyType}} goody, {{Type5|Unit}} unit<b>)</b></code>
<!-- 
DOGOODY
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|DoGoody}}<b>(</b>{{Type5|Plot}} plot, {{Type5|Unit}} unit<b>)</b></code>
<!-- 
GETADVANCEDSTARTCITYCOST
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|GetAdvancedStartCityCost}}<b>(</b>'''bool''' add, {{Type5|Plot}} plot<b>)</b></code>
<!-- 
GETADVANCEDSTARTIMPROVEMENTCOST
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|GetAdvancedStartImprovementCost}}<b>(</b>{{Type5|ImprovementType}} improvement, '''bool''' add, {{Type5|Plot}} plot<b>)</b></code>
<!-- 
GETADVANCEDSTARTROUTECOST
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|GetAdvancedStartRouteCost}}<b>(</b>{{Type5|RouteType}} route, '''bool''' add, {{Type5|Plot}} plot<b>)</b></code>
<!-- 
GETADVANCEDSTARTUNITCOST
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|GetAdvancedStartUnitCost}}<b>(</b>{{Type5|UnitType}} unit, '''bool''' add, {{Type5|Plot}} plot<b>)</b></code>
<!-- 
GETADVANCEDSTARTVISIBILITYCOST
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|GetAdvancedStartVisibilityCost}}<b>(</b>'''bool''' add, {{Type5|Plot}} plot<b>)</b></code>
<!-- 
GETBESTROUTE
-->
|-
|align="right" width="200" |<code>'''unknown'''</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|GetBestRoute}}<b>(</b>{{Type5|Plot}} plot<b>)</b></code>
<!-- 
GETCLOSESTGOODYPLOT
-->
|-
|align="right" width="200" |<code>{{Type5|Plot}}</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|GetClosestGoodyPlot}}<b>(</b>'''unknown''' void<b>)</b></code>
<!-- 
GETFOUNDEDRELIGIONENEMYCITYCOMBATMOD
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|GetFoundedReligionEnemyCityCombatMod}}<b>(</b>{{Type5|Plot}} toPlot<b>)</b></code>
<!-- 
GETFOUNDEDRELIGIONFRIENDLYCITYCOMBATMOD
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|GetFoundedReligionFriendlyCityCombatMod}}<b>(</b>{{Type5|Plot}} toPlot<b>)</b></code>
<!-- 
GETPLOTDANGER
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|GetPlotDanger}}<b>(</b>{{Type5|Plot}} plot<b>)</b></code>
<!-- 
GETPLOTHASORDER
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|GetPlotHasOrder}}<b>(</b>{{Type5|Plot}} Plot<b>)</b></code>
<!-- 
GETSTARTINGPLOT
-->
|-
|align="right" width="200" |<code>{{Type5|Plot}}</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|GetStartingPlot}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
RECEIVEGOODY
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|ReceiveGoody}}<b>(</b>{{Type5|Plot}} plot, {{Type5|GoodyType}} goody, {{Type5|Unit}} unit<b>)</b></code>
<!-- 
SETSTARTINGPLOT
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|SetStartingPlot}}<b>(</b>{{Type5|Plot}} plot<b>)</b></code>
<!-- 
CANSEEPLOT
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|Plot}}:{{Func5|Plot|CanSeePlot}}<b>(</b>{{Type5|Plot}} target, {{Type5|TeamID}} team, '''int''' range<b>)</b></code>
<!-- 
GETINLANDCORNER
-->
|-
|align="right" width="200" |<code>{{Type5|Plot}}</code>
|style="padding-left:6px" |<code>{{Type5|Plot}}:{{Func5|Plot|GetInlandCorner}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETNEARESTLANDPLOT
-->
|-
|align="right" width="200" |<code>{{Type5|Plot}}</code>
|style="padding-left:6px" |<code>{{Type5|Plot}}:{{Func5|Plot|GetNearestLandPlot}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
MOVEMENTCOST
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Plot}}:{{Func5|Plot|MovementCost}}<b>(</b>{{Type5|Unit}} unit, {{Type5|Plot}} fromPlot<b>)</b></code>
<!-- 
SHAREADJACENTAREA
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|Plot}}:{{Func5|Plot|ShareAdjacentArea}}<b>(</b>{{Type5|Plot}} plot<b>)</b></code>
<!-- 
CANPLACEUNITAT
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|UI}}.{{Func5|UI|CanPlaceUnitAt}}<b>(</b>'''unknown''' unit, {{Type5|Plot}} plot<b>)</b></code>
<!-- 
DOSELECTCITYATPLOT
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|UI}}.{{Func5|UI|DoSelectCityAtPlot}}<b>(</b>{{Type5|Plot}} plot<b>)</b></code>
<!-- 
HIGHLIGHTCANPLACEPLOTS
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|UI}}.{{Func5|UI|HighlightCanPlacePlots}}<b>(</b>{{Type5|Unit}} unit, {{Type5|Plot}} arg1<b>)</b></code>
<!-- 
LOCATIONSELECT
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|UI}}.{{Func5|UI|LocationSelect}}<b>(</b>{{Type5|Plot}} plot, '''int''' ctrl, '''int''' alt, '''bool''' shift<b>)</b></code>
<!-- 
LOOKAT
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|UI}}.{{Func5|UI|LookAt}}<b>(</b>{{Type5|Plot}} plot, '''int''' arg1 = nil<b>)</b></code>
<!-- 
ATPLOT
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Unit}}:{{Func5|Unit|AtPlot}}<b>(</b>{{Type5|Plot}} plot<b>)</b></code>
<!-- 
CANAIRDEFEND
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|Unit}}:{{Func5|Unit|CanAirDefend}}<b>(</b>{{Type5|Plot}} plot<b>)</b></code>
<!-- 
CANAIRLIFT
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|Unit}}:{{Func5|Unit|CanAirlift}}<b>(</b>{{Type5|Plot}} plot<b>)</b></code>
<!-- 
CANAIRLIFTAT
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|Unit}}:{{Func5|Unit|CanAirliftAt}}<b>(</b>{{Type5|Plot}} plot, '''int''' x, '''int''' y<b>)</b></code>
<!-- 
CANAIRPATROL
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|Unit}}:{{Func5|Unit|CanAirPatrol}}<b>(</b>{{Type5|Plot}} plot<b>)</b></code>
<!-- 
CANBUILD
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|Unit}}:{{Func5|Unit|CanBuild}}<b>(</b>{{Type5|Plot}} plot, {{Type5|BuildActionType}} build, '''bool''' testVisible = false, '''bool''' testGold = true<b>)</b></code>
<!-- 
CANBUILDSPACESHIP
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|Unit}}:{{Func5|Unit|CanBuildSpaceship}}<b>(</b>{{Type5|Plot}} plot, '''bool''' visible<b>)</b></code>
<!-- 
CANCONSTRUCT
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|Unit}}:{{Func5|Unit|CanConstruct}}<b>(</b>{{Type5|Plot}} plot, {{Type5|BuildingType}} building<b>)</b></code>
<!-- 
CANDISCOVER
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|Unit}}:{{Func5|Unit|CanDiscover}}<b>(</b>{{Type5|Plot}} plot<b>)</b></code>
<!-- 
CANDISEMBARK
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|Unit}}:{{Func5|Unit|CanDisembark}}<b>(</b>{{Type5|Plot}} plot<b>)</b></code>
<!-- 
CANDISEMBARKONTO
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|Unit}}:{{Func5|Unit|CanDisembarkOnto}}<b>(</b>{{Type5|Plot}} plot<b>)</b></code>
<!-- 
CANEMBARK
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|Unit}}:{{Func5|Unit|CanEmbark}}<b>(</b>{{Type5|Plot}} plot<b>)</b></code>
<!-- 
CANEMBARKONTO
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|Unit}}:{{Func5|Unit|CanEmbarkOnto}}<b>(</b>{{Type5|Plot}} plot, {{Type5|Plot}} targetPlot<b>)</b></code>
<!-- 
CANFORTIFY
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|Unit}}:{{Func5|Unit|CanFortify}}<b>(</b>{{Type5|Plot}} plot<b>)</b></code>
<!-- 
CANFOUND
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|Unit}}:{{Func5|Unit|CanFound}}<b>(</b>{{Type5|Plot}} plot, '''bool''' testVisible = false<b>)</b></code>
<!-- 
CANGIVEEXPERIENCE
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|Unit}}:{{Func5|Unit|CanGiveExperience}}<b>(</b>{{Type5|Plot}} plot<b>)</b></code>
<!-- 
CANGOLDENAGE
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|Unit}}:{{Func5|Unit|CanGoldenAge}}<b>(</b>{{Type5|Plot}} plot, '''bool''' testVisible<b>)</b></code>
<!-- 
CANHEAL
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Unit}}:{{Func5|Unit|CanHeal}}<b>(</b>{{Type5|Plot}} plot<b>)</b></code>
<!-- 
CANHOLD
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|Unit}}:{{Func5|Unit|CanHold}}<b>(</b>{{Type5|Plot}} plot<b>)</b></code>
<!-- 
CANJOIN
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|Unit}}:{{Func5|Unit|CanJoin}}<b>(</b>{{Type5|Plot}} plot, {{Type5|SpecialistType}} specialist<b>)</b></code>
<!-- 
CANLEAD
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|Unit}}:{{Func5|Unit|CanLead}}<b>(</b>{{Type5|Plot}} plot, '''int''' unitId<b>)</b></code>
<!-- 
CANLOAD
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|Unit}}:{{Func5|Unit|CanLoad}}<b>(</b>{{Type5|Plot}} plot<b>)</b></code>
<!-- 
CANLOADUNIT
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|Unit}}:{{Func5|Unit|CanLoadUnit}}<b>(</b>{{Type5|Unit}} unit, {{Type5|Plot}} plot<b>)</b></code>
<!-- 
CANMOVEORATTACKINTO
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|Unit}}:{{Func5|Unit|CanMoveOrAttackInto}}<b>(</b>{{Type5|Plot}} plot, '''bool''' declareWar = false, '''bool''' destination = false<b>)</b></code>
<!-- 
CANMOVETHROUGH
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|Unit}}:{{Func5|Unit|CanMoveThrough}}<b>(</b>{{Type5|Plot}} plot<b>)</b></code>
<!-- 
CANNUKE
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Unit}}:{{Func5|Unit|CanNuke}}<b>(</b>{{Type5|Plot}} plot<b>)</b></code>
<!-- 
CANNUKEAT
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|Unit}}:{{Func5|Unit|CanNukeAt}}<b>(</b>{{Type5|Plot}} plot, '''int''' x, '''int''' y<b>)</b></code>
<!-- 
CANPARADROP
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|Unit}}:{{Func5|Unit|CanParadrop}}<b>(</b>{{Type5|Plot}} plot, '''bool''' arg1<b>)</b></code>
<!-- 
CANPARADROPAT
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|Unit}}:{{Func5|Unit|CanParadropAt}}<b>(</b>{{Type5|Plot}} plot, '''int''' x, '''int''' y<b>)</b></code>
<!-- 
CANPILLAGE
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|Unit}}:{{Func5|Unit|CanPillage}}<b>(</b>{{Type5|Plot}} plot<b>)</b></code>
<!-- 
CANREBASEAT
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|Unit}}:{{Func5|Unit|CanRebaseAt}}<b>(</b>{{Type5|Plot}} sourcePlot, '''int''' targetX, '''int''' targetY<b>)</b></code>
<!-- 
CANSENTRY
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|Unit}}:{{Func5|Unit|CanSentry}}<b>(</b>{{Type5|Plot}} plot<b>)</b></code>
<!-- 
CANSLEEP
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|Unit}}:{{Func5|Unit|CanSleep}}<b>(</b>{{Type5|Plot}} plot<b>)</b></code>
<!-- 
CANSTARTMISSION
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|Unit}}:{{Func5|Unit|CanStartMission}}<b>(</b>'''int''' mission, '''int''' data1, '''int''' data2, {{Type5|Plot}} plot = nil, '''bool''' testVisible = false<b>)</b></code>
<!-- 
CANTRADE
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|Unit}}:{{Func5|Unit|CanTrade}}<b>(</b>{{Type5|Plot}} plot, '''bool''' testVisible<b>)</b></code>
<!-- 
EMBARK
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Unit}}:{{Func5|Unit|Embark}}<b>(</b>{{Type5|Plot}} plot<b>)</b></code>
<!-- 
EXECUTESPECIALEXPLOREMOVE
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Unit}}:{{Func5|Unit|ExecuteSpecialExploreMove}}<b>(</b>{{Type5|Plot}} targetPlot<b>)</b></code>
<!-- 
GENERATEPATH
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|Unit}}:{{Func5|Unit|GeneratePath}}<b>(</b>{{Type5|Plot}} toPlot, '''int''' flags = 0, '''bool''' reuse = false, '''unknown''' piPathTurns = nil<b>)</b></code>
<!-- 
GETBESTINTERCEPTOR
-->
|-
|align="right" width="200" |<code>'''unknown'''</code>
|style="padding-left:6px" |<code>{{Type5|Unit}}:{{Func5|Unit|GetBestInterceptor}}<b>(</b>{{Type5|Plot}} plot<b>)</b></code>
<!-- 
GETBESTSEAPILLAGEINTERCEPTOR
-->
|-
|align="right" width="200" |<code>'''unknown'''</code>
|style="padding-left:6px" |<code>{{Type5|Unit}}:{{Func5|Unit|GetBestSeaPillageInterceptor}}<b>(</b>{{Type5|Plot}} plot<b>)</b></code>
<!-- 
GETDECLAREWARRANGESTRIKE
-->
|-
|align="right" width="200" |<code>{{Type5|TeamID}}</code>
|style="padding-left:6px" |<code>{{Type5|Unit}}:{{Func5|Unit|GetDeclareWarRangeStrike}}<b>(</b>{{Type5|Plot}} plot<b>)</b></code>
<!-- 
GETMAXATTACKSTRENGTH
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Unit}}:{{Func5|Unit|GetMaxAttackStrength}}<b>(</b>{{Type5|Plot}} fromPlot, {{Type5|Plot}} toPlot, {{Type5|Unit}} defender<b>)</b></code>
<!-- 
GETMAXDEFENSESTRENGTH
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Unit}}:{{Func5|Unit|GetMaxDefenseStrength}}<b>(</b>{{Type5|Plot}} inPlot, {{Type5|Unit}} attacker, '''bool''' arg2 = nil<b>)</b></code>
<!-- 
GETPLOT
-->
|-
|align="right" width="200" |<code>{{Type5|Plot}}</code>
|style="padding-left:6px" |<code>{{Type5|Unit}}:{{Func5|Unit|GetPlot}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETTRADEGOLD
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Unit}}:{{Func5|Unit|GetTradeGold}}<b>(</b>{{Type5|Plot}} plot<b>)</b></code>
<!-- 
GETUPGRADEUNITFROMPLOT
-->
|-
|align="right" width="200" |<code>{{Type5|Unit}}</code>
|style="padding-left:6px" |<code>{{Type5|Unit}}:{{Func5|Unit|GetUpgradeUnitFromPlot}}<b>(</b>{{Type5|Plot}} adjacentPlot<b>)</b></code>
<!-- 
ISCANDEFEND
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|Unit}}:{{Func5|Unit|IsCanDefend}}<b>(</b>{{Type5|Plot}} plot<b>)</b></code>
<!-- 
ISNUKEVICTIM
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|Unit}}:{{Func5|Unit|IsNukeVictim}}<b>(</b>{{Type5|Plot}} plot, {{Type5|TeamID}} team<b>)</b></code>
<!-- 
ISRANGEATTACKIGNORELOS
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|Unit}}:{{Func5|Unit|IsRangeAttackIgnoreLOS}}<b>(</b>{{Type5|Plot}} plot<b>)</b></code>
<!-- 
PUSHMISSION
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Unit}}:{{Func5|Unit|PushMission}}<b>(</b>{{Type5|MissionType}} mission, '''int''' data1 = -1, '''int''' data2 = -1, '''int''' flags = 0, '''bool''' append = false, '''bool''' manual = fa;se, {{Type5|MissionType}} missionAI = NO_MISSIONAI, {{Type5|Plot}} missionAIPlot = nil, {{Type5|Unit}} missionAIUnit = nil<b>)</b></code>
<!-- 
SETRECONPLOT
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Unit}}:{{Func5|Unit|SetReconPlot}}<b>(</b>{{Type5|Plot}} newValue<b>)</b></code>
|}




{{Civ5 API Footer}}
[[Category:Civ5 Types|Plot]]