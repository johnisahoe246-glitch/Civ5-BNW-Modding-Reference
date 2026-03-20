{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



=Instance Methods=
Methods are functions that belong to an object. Instance methods are invoked through a '''colon''', as in <code>caller:SomeMethod(&lt;args&gt;)</code>, where ''caller'' is an instance of Area.<br/>
A colon implictly passes the caller object as the first argument. That is, the former call is equivalent to this one: <code>caller.SomeMethod(caller, &lt;args&gt;)</code>
==C==
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
CALCULATETOTALBESTNATUREYIELD
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Area|CalculateTotalBestNatureYield}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
COUNTCOASTALLAND
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Area|CountCoastalLand}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
COUNTNUMUNIQUERESOURCETYPES
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Area|CountNumUniqueResourceTypes}}<b>(</b><!-- No arguments --><b>)</b></code>
|}

==G==
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
GETCITIESPERPLAYER
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Area|GetCitiesPerPlayer}}<b>(</b>{{Type5|PlayerID}} index<b>)</b></code>
<!-- 
GETFREESPECIALIST
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Area|GetFreeSpecialist}}<b>(</b>{{Type5|PlayerID}} index<b>)</b></code>
<!-- 
GETID
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>{{Type5|AreaID}}</code>
|width="100%" |<code>{{FuncLabel5|Area|GetID}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETNUMCITIES
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Area|GetNumCities}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETNUMIMPROVEMENTS
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Area|GetNumImprovements}}<b>(</b>{{Type5|ImprovementType}} improvement<b>)</b></code>
<!-- 
GETNUMOWNEDTILES
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Area|GetNumOwnedTiles}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETNUMRESOURCES
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Area|GetNumResources}}<b>(</b>{{Type5|ResourceType}} resource<b>)</b></code>
<!-- 
GETNUMREVEALEDTILES
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Area|GetNumRevealedTiles}}<b>(</b>{{Type5|TeamID}} index<b>)</b></code>
<!-- 
GETNUMRIVEREDGES
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Area|GetNumRiverEdges}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETNUMSTARTINGPLOTS
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Area|GetNumStartingPlots}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETNUMTILES
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Area|GetNumTiles}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETNUMTOTALRESOURCES
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Area|GetNumTotalResources}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETNUMUNITS
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Area|GetNumUnits}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETNUMUNOWNEDTILES
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Area|GetNumUnownedTiles}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETNUMUNREVEALEDTILES
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Area|GetNumUnrevealedTiles}}<b>(</b>{{Type5|TeamID}} index<b>)</b></code>
<!-- 
GETPOPULATIONPERPLAYER
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Area|GetPopulationPerPlayer}}<b>(</b>{{Type5|PlayerID}} index<b>)</b></code>
<!-- 
GETTARGETCITY
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''unknown'''</code>
|width="100%" |<code>{{FuncLabel5|Area|GetTargetCity}}<b>(</b>{{Type5|PlayerID}} index<b>)</b></code>
<!-- 
GETTOTALPOPULATION
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Area|GetTotalPopulation}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETUNITSPERPLAYER
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Area|GetUnitsPerPlayer}}<b>(</b>{{Type5|PlayerID}} index<b>)</b></code>
<!-- 
GETYIELDRATEMODIFIER
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Area|GetYieldRateModifier}}<b>(</b>{{Type5|PlayerID}} index1, {{Type5|YieldType}} index2<b>)</b></code>
|}

==I==
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
ISNONE
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Area|IsNone}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ISWATER
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Area|IsWater}}<b>(</b><!-- No arguments --><b>)</b></code>
|}


=Used by=
{|cellspacing="4" cellpadding="0" width="100%" style="background-color:#F0F0F0"
<!-- 
AREAS
-->
|-
|align="right" width="200" |<code>iterator({{Type5|AreaID}}, {{Type5|Area}})</code>
|style="padding-left:6px" |<code>{{Type5|Map}}.{{Func5|Map|Areas}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
FINDBIGGESTAREA
-->
|-
|align="right" width="200" |<code>{{Type5|Area}}</code>
|style="padding-left:6px" |<code>{{Type5|Map}}.{{Func5|Map|FindBiggestArea}}<b>(</b>'''bool''' ocean<b>)</b></code>
<!-- 
GETAREA
-->
|-
|align="right" width="200" |<code>{{Type5|Area}}</code>
|style="padding-left:6px" |<code>{{Type5|Map}}.{{Func5|Map|GetArea}}<b>(</b>{{Type5|AreaID}} areaID<b>)</b></code>
<!-- 
AREA
-->
|-
|align="right" width="200" |<code>{{Type5|Area}}</code>
|style="padding-left:6px" |<code>{{Type5|Plot}}:{{Func5|Plot|Area}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ISADJACENTTOAREA
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|Plot}}:{{Func5|Plot|IsAdjacentToArea}}<b>(</b>{{Type5|Area}} area<b>)</b></code>
<!-- 
ISPOTENTIALCITYWORKFORAREA
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|Plot}}:{{Func5|Plot|IsPotentialCityWorkForArea}}<b>(</b>{{Type5|Area}} area<b>)</b></code>
<!-- 
COUNTENEMYDANGERBYAREA
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Team}}:{{Func5|Team|CountEnemyDangerByArea}}<b>(</b>{{Type5|Area}} area<b>)</b></code>
<!-- 
COUNTNUMCITIESBYAREA
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Team}}:{{Func5|Team|CountNumCitiesByArea}}<b>(</b>{{Type5|Area}} area<b>)</b></code>
<!-- 
COUNTNUMUNITSBYAREA
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Team}}:{{Func5|Team|CountNumUnitsByArea}}<b>(</b>{{Type5|Area}} area<b>)</b></code>
<!-- 
COUNTTOTALPOPULATIONBYAREA
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Team}}:{{Func5|Team|CountTotalPopulationByArea}}<b>(</b>{{Type5|Area}} area<b>)</b></code>
<!-- 
GETAREA
-->
|-
|align="right" width="200" |<code>{{Type5|Area}}</code>
|style="padding-left:6px" |<code>{{Type5|Unit}}:{{Func5|Unit|GetArea}}<b>(</b><!-- No arguments --><b>)</b></code>
|}




{{Civ5 API Footer}}
[[Category:Civ5 Types|Area]]