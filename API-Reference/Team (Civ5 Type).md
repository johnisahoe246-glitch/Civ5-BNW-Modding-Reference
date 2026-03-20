{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



=Instance Methods=
Methods are functions that belong to an object. Instance methods are invoked through a '''colon''', as in <code>caller:SomeMethod(&lt;args&gt;)</code>, where ''caller'' is an instance of Team.<br/>
A colon implictly passes the caller object as the first argument. That is, the former call is equivalent to this one: <code>caller.SomeMethod(caller, &lt;args&gt;)</code>
==A==
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
ADDTEAM
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Team|AddTeam}}<b>(</b>{{Type5|TeamID}} team<b>)</b></code>
|}

==C==
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
CANCHANGEWARPEACE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Team|CanChangeWarPeace}}<b>(</b>{{Type5|TeamID}} team<b>)</b></code>
<!-- 
CANCONTACT
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Team|CanContact}}<b>(</b>{{Type5|TeamID}} team<b>)</b></code>
<!-- 
CANDECLAREWAR
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Team|CanDeclareWar}}<b>(</b>{{Type5|TeamID}} team<b>)</b></code>
<!-- 
CANDEFENSIVEEMBARK
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>{{UnknownSignature5}}</code>
|width="100%" |<code>{{FuncLabel5|Team|CanDefensiveEmbark}}<!-- No arguments --></code>
<!-- 
CANEMBARK
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Team|CanEmbark}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
CANLAUNCH
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Team|CanLaunch}}<b>(</b>{{Type5|VictoryType}} victory<b>)</b></code>
<!-- 
CHANGEALLOWEMBASSYTRADINGALLOWEDCOUNT
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>{{UnknownSignature5}}</code>
|width="100%" |<code>{{FuncLabel5|Team|ChangeAllowEmbassyTradingAllowedCount}}<!-- No arguments --></code>
<!-- 
CHANGEBORDEROBSTACLECOUNT
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Team|ChangeBorderObstacleCount}}<b>(</b>'''int''' change<b>)</b></code>
<!-- 
CHANGEBRIDGEBUILDINGCOUNT
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Team|ChangeBridgeBuildingCount}}<b>(</b>'''int''' change<b>)</b></code>
<!-- 
CHANGEDEFENSIVEPACTTRADINGALLOWEDCOUNT
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Team|ChangeDefensivePactTradingAllowedCount}}<b>(</b>'''int''' change<b>)</b></code>
<!-- 
CHANGEEXTRAMOVES
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Team|ChangeExtraMoves}}<b>(</b>{{Type5|DomainType}} index, '''int''' change<b>)</b></code>
<!-- 
CHANGEEXTRAWATERSEEFROMCOUNT
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Team|ChangeExtraWaterSeeFromCount}}<b>(</b>'''int''' change<b>)</b></code>
<!-- 
CHANGEFORCETEAMVOTEELIGIBILITYCOUNT
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Team|ChangeForceTeamVoteEligibilityCount}}<b>(</b>{{Type5|VoteSourceType}} voteSource, '''int''' change<b>)</b></code>
<!-- 
CHANGEGOLDTRADINGCOUNT
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Team|ChangeGoldTradingCount}}<b>(</b>'''int''' change<b>)</b></code>
<!-- 
CHANGEIMPROVEMENTYIELDCHANGE
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Team|ChangeImprovementYieldChange}}<b>(</b>{{Type5|ImprovementType}} index1, {{Type5|YieldType}} index2, '''int''' change<b>)</b></code>
<!-- 
CHANGEMAPTRADINGCOUNT
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Team|ChangeMapTradingCount}}<b>(</b>'''int''' change<b>)</b></code>
<!-- 
CHANGENUKEINTERCEPTION
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Team|ChangeNukeInterception}}<b>(</b>'''int''' change<b>)</b></code>
<!-- 
CHANGEOPENBORDERSTRADINGALLOWEDCOUNT
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Team|ChangeOpenBordersTradingAllowedCount}}<b>(</b>'''int''' change<b>)</b></code>
<!-- 
CHANGEPERMANENTALLIANCETRADINGCOUNT
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Team|ChangePermanentAllianceTradingCount}}<b>(</b>'''int''' change<b>)</b></code>
<!-- 
CHANGEPROJECTCOUNT
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Team|ChangeProjectCount}}<b>(</b>{{Type5|ProjectType}} index, '''int''' change<b>)</b></code>
<!-- 
CHANGEROUTECHANGE
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Team|ChangeRouteChange}}<b>(</b>{{Type5|RouteType}} index, '''int''' change<b>)</b></code>
<!-- 
CHANGETECHSHARECOUNT
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Team|ChangeTechShareCount}}<b>(</b>'''int''' index, '''int''' change<b>)</b></code>
<!-- 
CHANGETECHTRADINGCOUNT
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Team|ChangeTechTradingCount}}<b>(</b>'''int''' change<b>)</b></code>
<!-- 
CHANGEVICTORYPOINTS
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Team|ChangeVictoryPoints}}<b>(</b>'''int''' change<b>)</b></code>
<!-- 
CHANGEWATERWORKCOUNT
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Team|ChangeWaterWorkCount}}<b>(</b>'''int''' change<b>)</b></code>
<!-- 
COUNTENEMYDANGERBYAREA
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Team|CountEnemyDangerByArea}}<b>(</b>{{Type5|Area}} area<b>)</b></code>
<!-- 
COUNTNUMCITIESBYAREA
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Team|CountNumCitiesByArea}}<b>(</b>{{Type5|Area}} area<b>)</b></code>
<!-- 
COUNTNUMUNITSBYAREA
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Team|CountNumUnitsByArea}}<b>(</b>{{Type5|Area}} area<b>)</b></code>
<!-- 
COUNTTOTALPOPULATIONBYAREA
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Team|CountTotalPopulationByArea}}<b>(</b>{{Type5|Area}} area<b>)</b></code>
|}

==D==
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
DECLAREWAR
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Team|DeclareWar}}<b>(</b>{{Type5|TeamID}} team<b>)</b></code>
|}

==G==
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
GETALLOWEMBASSYTRADINGALLOWEDCOUNT
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>{{UnknownSignature5}}</code>
|width="100%" |<code>{{FuncLabel5|Team|GetAllowEmbassyTradingAllowedCount}}<!-- No arguments --></code>
<!-- 
GETATWARCOUNT
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Team|GetAtWarCount}}<b>(</b>'''bool''' ignoreMinors<b>)</b></code>
<!-- 
GETBORDEROBSTACLECOUNT
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Team|GetBorderObstacleCount}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETBRIDGEBUILDINGCOUNT
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Team|GetBridgeBuildingCount}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETBUILDINGCLASSCOUNT
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Team|GetBuildingClassCount}}<b>(</b>{{Type5|BuildingClassType}} index<b>)</b></code>
<!-- 
GETBUILDINGCLASSCOUNTPLUSMAKING
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Team|GetBuildingClassCountPlusMaking}}<b>(</b>{{Type5|BuildingClassType}} unitClass<b>)</b></code>
<!-- 
GETBUILDINGCLASSMAKING
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Team|GetBuildingClassMaking}}<b>(</b>{{Type5|BuildingClassType}} buildingClass<b>)</b></code>
<!-- 
GETCURRENTERA
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Team|GetCurrentEra}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETDEFENSIVEPACTCOUNT
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Team|GetDefensivePactCount}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETDEFENSIVEPACTTRADINGALLOWEDCOUNT
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Team|GetDefensivePactTradingAllowedCount}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETDEFENSIVEPOWER
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Team|GetDefensivePower}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETEXTRAMOVES
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Team|GetExtraMoves}}<b>(</b>{{Type5|DomainType}} index<b>)</b></code>
<!-- 
GETEXTRAWATERSEEFROMCOUNT
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Team|GetExtraWaterSeeFromCount}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETFORCETEAMVOTEELIGIBILITYCOUNT
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Team|GetForceTeamVoteEligibilityCount}}<b>(</b>{{Type5|VoteSourceType}} voteSource<b>)</b></code>
<!-- 
GETGOLDTRADINGCOUNT
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Team|GetGoldTradingCount}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETHANDICAPTYPE
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>{{Type5|HandicapType}}</code>
|width="100%" |<code>{{FuncLabel5|Team|GetHandicapType}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETHASMETCIVCOUNT
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|yes|<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Team|GetHasMetCivCount}}<b>(</b>'''bool''' ignoreMinors<b>)</b></code>
<!-- 
GETID
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>{{Type5|TeamID}}</code>
|width="100%" |<code>{{FuncLabel5|Team|GetID}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETIMPROVEMENTYIELDCHANGE
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Team|GetImprovementYieldChange}}<b>(</b>{{Type5|ImprovementType}} index, {{Type5|YieldType}} index2<b>)</b></code>
<!-- 
GETLEADERID
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>{{Type5|PlayerID}}</code>
|width="100%" |<code>{{FuncLabel5|Team|GetLeaderID}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETLIBERATEDBYTEAM
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>{{Type5|TeamID}}</code>
|width="100%" |<code>{{FuncLabel5|Team|GetLiberatedByTeam}}<b>(</b>{{Type5|TeamID}} index<b>)</b></code>
<!-- 
GETMAPTRADINGCOUNT
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Team|GetMapTradingCount}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETNAME
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''string'''</code>
|width="100%" |<code>{{FuncLabel5|Team|GetName}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETNAMEKEY
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''unknown'''</code>
|width="100%" |<code>{{FuncLabel5|Team|GetNameKey}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETNUKEINTERCEPTION
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Team|GetNukeInterception}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETNUMCITIES
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Team|GetNumCities}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETNUMMEMBERS
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Team|GetNumMembers}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETNUMNUKEUNITS
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Team|GetNumNukeUnits}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETNUMTURNSLOCKEDINTOWAR
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Team|GetNumTurnsLockedIntoWar}}<b>(</b>{{Type5|TeamID}} team<b>)</b></code>
<!-- 
GETOBSOLETEBUILDINGCOUNT
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Team|GetObsoleteBuildingCount}}<b>(</b>{{Type5|BuildingType}} index<b>)</b></code>
<!-- 
GETOPENBORDERSTRADINGALLOWEDCOUNT
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Team|GetOpenBordersTradingAllowedCount}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETPERMANENTALLIANCETRADINGCOUNT
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Team|GetPermanentAllianceTradingCount}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETPOWER
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Team|GetPower}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETPROJECTARTTYPE
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Team|GetProjectArtType}}<b>(</b>{{Type5|ProjectType}} index, '''int''' number<b>)</b></code>
<!-- 
GETPROJECTCOUNT
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Team|GetProjectCount}}<b>(</b>{{Type5|ProjectType}} index<b>)</b></code>
<!-- 
GETPROJECTDEFAULTARTTYPE
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Team|GetProjectDefaultArtType}}<b>(</b>{{Type5|ProjectType}} index<b>)</b></code>
<!-- 
GETPROJECTEDVOTESFROMCIVS
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Team|GetProjectedVotesFromCivs}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETPROJECTEDVOTESFROMLIBERATEDMINORS
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Team|GetProjectedVotesFromLiberatedMinors}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETPROJECTEDVOTESFROMMINORALLIES
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Team|GetProjectedVotesFromMinorAllies}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETPROJECTMAKING
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Team|GetProjectMaking}}<b>(</b>{{Type5|ProjectType}} index<b>)</b></code>
<!-- 
GETROUTECHANGE
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Team|GetRouteChange}}<b>(</b>{{Type5|RouteType}} index<b>)</b></code>
<!-- 
GETSCORE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Team|GetScore}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETSECRETARYID
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>{{Type5|PlayerID}}</code>
|width="100%" |<code>{{FuncLabel5|Team|GetSecretaryID}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETTEAMTECHS
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>{{Type5|TeamTechs}}</code>
|width="100%" |<code>{{FuncLabel5|Team|GetTeamTechs}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETTEAMVOTINGFORINDIPLO
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>{{Type5|TeamID}}</code>
|width="100%" |<code>{{FuncLabel5|Team|GetTeamVotingForInDiplo}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETTECHSHARECOUNT
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Team|GetTechShareCount}}<b>(</b>'''int''' index<b>)</b></code>
<!-- 
GETTECHTRADINGCOUNT
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Team|GetTechTradingCount}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETTOTALLAND
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Team|GetTotalLand}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETTOTALPOPULATION
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Team|GetTotalPopulation}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETTOTALPROJECTEDVOTES
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Team|GetTotalProjectedVotes}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETTOTALSECUREDVOTES
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Team|GetTotalSecuredVotes}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETUNITCLASSCOUNT
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Team|GetUnitClassCount}}<b>(</b>{{Type5|UnitClassType}} index<b>)</b></code>
<!-- 
GETUNITCLASSCOUNTPLUSMAKING
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Team|GetUnitClassCountPlusMaking}}<b>(</b>{{Type5|UnitClassType}} unitClass<b>)</b></code>
<!-- 
GETUNITCLASSMAKING
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Team|GetUnitClassMaking}}<b>(</b>{{Type5|UnitClassType}} unitClass<b>)</b></code>
<!-- 
GETVICTORYCOUNTDOWN
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Team|GetVictoryCountdown}}<b>(</b>{{Type5|VictoryType}} victory<b>)</b></code>
<!-- 
GETVICTORYDELAY
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Team|GetVictoryDelay}}<b>(</b>{{Type5|VictoryType}} victory<b>)</b></code>
<!-- 
GETVICTORYPOINTS
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Team|GetVictoryPoints}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETWATERWORKCOUNT
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Team|GetWaterWorkCount}}<b>(</b><!-- No arguments --><b>)</b></code>
|}

==H==
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
HASEMBASSYATTEAM
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Team|HasEmbassyAtTeam}}<b>(</b>{{Type5|TeamID}} themTeam<b>)</b></code>
<!-- 
HASMETHUMAN
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Team|HasMetHuman}}<b>(</b><!-- No arguments --><b>)</b></code>
|}

==I==
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
ISALIVE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Team|IsAlive}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ISALLOWEMBASSYTRADINGALLOWED
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Team|IsAllowEmbassyTradingAllowed}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ISALLOWSOPENBORDERSTOTEAM
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Team|IsAllowsOpenBordersToTeam}}<b>(</b>{{Type5|TeamID}} index<b>)</b></code>
<!-- 
ISATWAR
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Team|IsAtWar}}<b>(</b>{{Type5|TeamID}} index<b>)</b></code>
<!-- 
ISBARBARIAN
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Team|IsBarbarian}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ISBORDEROBSTACLE
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Team|IsBorderObstacle}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ISBRIDGEBUILDING
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Team|IsBridgeBuilding}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ISBUILDINGCLASSMAXEDOUT
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Team|IsBuildingClassMaxedOut}}<b>(</b>{{Type5|BuildingClassType}} index, '''int''' extra<b>)</b></code>
<!-- 
ISDEFENSIVEPACT
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Team|IsDefensivePact}}<b>(</b>{{Type5|TeamID}} index<b>)</b></code>
<!-- 
ISDEFENSIVEPACTTRADINGALLOWED
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Team|IsDefensivePactTradingAllowed}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ISDEFENSIVEPACTTRADINGALLOWEDWITHTEAM
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>{{UnknownSignature5}}</code>
|width="100%" |<code>{{FuncLabel5|Team|IsDefensivePactTradingAllowedWithTeam}}<!-- No arguments --></code>
<!-- 
ISEVERALIVE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Team|IsEverAlive}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ISEXTRAWATERSEEFROM
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Team|IsExtraWaterSeeFrom}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ISFORCEPEACE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Team|IsForcePeace}}<b>(</b>{{Type5|TeamID}} index<b>)</b></code>
<!-- 
ISFORCETEAMVOTEELIGIBLE
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Team|IsForceTeamVoteEligible}}<b>(</b>{{Type5|VoteSourceType}} voteSource<b>)</b></code>
<!-- 
ISGOLDTRADING
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Team|IsGoldTrading}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ISHASMET
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Team|IsHasMet}}<b>(</b>{{Type5|TeamID}} index<b>)</b></code>
<!-- 
ISHASRESEARCHAGREEMENT
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Team|IsHasResearchAgreement}}<b>(</b>{{Type5|TeamID}} team<b>)</b></code>
<!-- 
ISHASTECH
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Team|IsHasTech}}<b>(</b>{{Type5|TechType}} index<b>)</b></code>
<!-- 
ISHASTRADEAGREEMENT
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Team|IsHasTradeAgreement}}<b>(</b>{{Type5|TeamID}} team<b>)</b></code>
<!-- 
ISHOMEOFUNITEDNATIONS
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Team|IsHomeOfUnitedNations}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ISHUMAN
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Team|IsHuman}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ISMAPCENTERING
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Team|IsMapCentering}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ISMAPTRADING
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Team|IsMapTrading}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ISMINORCIV
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Team|IsMinorCiv}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ISMINORCIVWARMONGER
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Team|IsMinorCivWarmonger}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ISNONE
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Team|IsNone}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ISOBSOLETEBUILDING
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Team|IsObsoleteBuilding}}<b>(</b>{{Type5|BuildingType}} index<b>)</b></code>
<!-- 
ISOPENBORDERSTRADINGALLOWED
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Team|IsOpenBordersTradingAllowed}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ISOPENBORDERSTRADINGALLOWEDWITHTEAM
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Team|IsOpenBordersTradingAllowedWithTeam}}<b>(</b>{{Type5|TeamID}} arg0<b>)</b></code>
<!-- 
ISPERMANENTALLIANCETRADING
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Team|IsPermanentAllianceTrading}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ISPERMANENTWARPEACE
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Team|IsPermanentWarPeace}}<b>(</b>{{Type5|TeamID}} index<b>)</b></code>
<!-- 
ISPROJECTANDARTMAXEDOUT
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Team|IsProjectAndArtMaxedOut}}<b>(</b>{{Type5|ProjectType}} index<b>)</b></code>
<!-- 
ISPROJECTMAXEDOUT
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Team|IsProjectMaxedOut}}<b>(</b>{{Type5|ProjectType}} index, '''int''' extra<b>)</b></code>
<!-- 
ISRESEARCHAGREEMENTTRADINGALLOWED
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Team|IsResearchAgreementTradingAllowed}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ISRESEARCHAGREEMENTTRADINGALLOWEDWITHTEAM
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>{{UnknownSignature5}}</code>
|width="100%" |<code>{{FuncLabel5|Team|IsResearchAgreementTradingAllowedWithTeam}}<!-- No arguments --></code>
<!-- 
ISTECHSHARE
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Team|IsTechShare}}<b>(</b>'''int''' index<b>)</b></code>
<!-- 
ISTECHTRADING
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Team|IsTechTrading}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ISTRADEAGREEMENTTRADINGALLOWED
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Team|IsTradeAgreementTradingAllowed}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ISUNITCLASSMAXEDOUT
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Team|IsUnitClassMaxedOut}}<b>(</b>{{Type5|UnitClassType}} index, '''int''' extra<b>)</b></code>
<!-- 
ISWATERWORK
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Team|IsWaterWork}}<b>(</b><!-- No arguments --><b>)</b></code>
|}

==M==
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
MAKEPEACE
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Team|MakePeace}}<b>(</b>{{Type5|TeamID}} team<b>)</b></code>
<!-- 
MEET
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Team|Meet}}<b>(</b>{{Type5|TeamID}} team, '''bool''' newDiplo<b>)</b></code>
|}

==S==
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
SETCURRENTERA
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Team|SetCurrentEra}}<b>(</b>'''int''' newValue<b>)</b></code>
<!-- 
SETHASTECH
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Team|SetHasTech}}<b>(</b>{{Type5|TechType}} index, '''bool''' newValue, {{Type5|PlayerID}} player, '''bool''' first, '''bool''' announce<b>)</b></code>
<!-- 
SETMAPCENTERING
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Team|SetMapCentering}}<b>(</b>'''bool''' newValue<b>)</b></code>
<!-- 
SETPERMANENTWARPEACE
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Team|SetPermanentWarPeace}}<b>(</b>{{Type5|TeamID}} index, '''bool''' newValue<b>)</b></code>
<!-- 
SETPROJECTARTTYPE
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Team|SetProjectArtType}}<b>(</b>{{Type5|ProjectType}} index, '''int''' number, '''int''' value<b>)</b></code>
<!-- 
SETPROJECTDEFAULTARTTYPE
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Team|SetProjectDefaultArtType}}<b>(</b>{{Type5|ProjectType}} index, '''int''' value<b>)</b></code>
|}

==U==
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
UPDATEEMBARKGRAPHICS
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Team|UpdateEmbarkGraphics}}<b>(</b><!-- No arguments --><b>)</b></code>
|}




{{Civ5 API Footer}}
[[Category:Civ5 Types|Team]]