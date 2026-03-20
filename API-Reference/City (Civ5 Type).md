{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



=Instance Methods=
Methods are functions that belong to an object. Instance methods are invoked through a '''colon''', as in <code>caller:SomeMethod(&lt;args&gt;)</code>, where ''caller'' is an instance of City.<br/>
A colon implictly passes the caller object as the first argument. That is, the former call is equivalent to this one: <code>caller.SomeMethod(caller, &lt;args&gt;)</code>
==A==
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
ADDPRODUCTIONEXPERIENCE
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|City|AddProductionExperience}}<b>(</b>{{Type5|Unit}} unit, '''bool''' conscript = false<b>)</b></code>
<!-- 
ADOPTRELIGIONFULLY
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|City|AdoptReligionFully}}<b>(</b>{{Type5|ReligionType}} religion<b>)</b></code>
<!-- 
ALLUPGRADESAVAILABLE
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>{{Type5|UnitType}}</code>
|width="100%" |<code>{{FuncLabel5|City|AllUpgradesAvailable}}<b>(</b>{{Type5|UnitType}} unit, '''int''' upgradeCount = 0<b>)</b></code>
<!-- 
ALTERWORKINGPLOT
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|City|AlterWorkingPlot}}<b>(</b>{{Type5|CityPlotID}} plotIndex<b>)</b></code>
<!-- 
AREA
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>{{UnknownSignature5}}</code>
|width="100%" |<code>{{FuncLabel5|City|Area}}<!-- No arguments --></code>
<!-- 
AT
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|City|At}}<b>(</b>'''int''' x, '''int''' y<b>)</b></code>
<!-- 
ATPLOT
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|City|AtPlot}}<b>(</b>{{Type5|Plot}} plot<b>)</b></code>
|}

==C==
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
CANBUYANYPLOT
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>{{UnknownSignature5}}</code>
|width="100%" |<code>{{FuncLabel5|City|CanBuyAnyPlot}}<!-- No arguments --></code>
<!-- 
CANBUYPLOT
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|City|CanBuyPlot}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
CANBUYPLOTAT
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|City|CanBuyPlotAt}}<b>(</b>'''int''' hexX, '''int''' hexY, '''bool''' arg2<b>)</b></code>
<!-- 
CANCONSCRIPT
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|City|CanConscript}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
CANCONSTRUCT
-->
|-
{{FuncInfos5|yes  |yes  |yes|<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|City|CanConstruct}}<b>(</b>{{Type5|BuildingType}} building, '''int''' continue, '''int''' testVisible, '''bool''' ignoreCost<b>)</b></code>
<!-- 
CANCONSTRUCTTOOLTIP
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|City|CanConstructTooltip}}<b>(</b>'''int''' id<b>)</b></code>
<!-- 
CANCONTINUEPRODUCTION
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|City|CanContinueProduction}}<b>(</b>{{Type5|OrderType}} orderType, '''int''' data1, '''int''' data2, '''bool''' save<b>)</b></code>
<!-- 
CANCREATE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|City|CanCreate}}<b>(</b>{{Type5|ProjectType}} project, '''int''' continue, '''int''' testVisible<b>)</b></code>
<!-- 
CANHURRY
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|City|CanHurry}}<b>(</b>{{Type5|HurryType}} hurry, '''bool''' testVisible<b>)</b></code>
<!-- 
CANJOIN
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|City|CanJoin}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
CANMAINTAIN
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|City|CanMaintain}}<b>(</b>{{Type5|ProcessType}} process, '''int''' continue<b>)</b></code>
<!-- 
CANPLACEUNITHERE
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>{{UnknownSignature5}}</code>
|width="100%" |<code>{{FuncLabel5|City|CanPlaceUnitHere}}<!-- No arguments --></code>
<!-- 
CANPREPARE
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|City|CanPrepare}}<b>(</b>'''int''' specialist, '''bool''' continue<b>)</b></code>
<!-- 
CANRANGESTRIKE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|City|CanRangeStrike}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
CANRANGESTRIKEAT
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|City|CanRangeStrikeAt}}<b>(</b>'''int''' x, '''int''' y, '''bool''' arg2, '''bool''' arg3<b>)</b></code>
<!-- 
CANRANGESTRIKENOW
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|City|CanRangeStrikeNow}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
CANTRAIN
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|City|CanTrain}}<b>(</b>{{Type5|UnitType}} unit, '''int''' continue, '''int''' testVisible, '''bool''' ignoreCost, '''bool''' ignoreUpgrades<b>)</b></code>
<!-- 
CANTRAINTOOLTIP
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|City|CanTrainTooltip}}<b>(</b>{{Type5|UnitType}} id<b>)</b></code>
<!-- 
CANWORK
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|City|CanWork}}<b>(</b>{{Type5|Plot}} plot<b>)</b></code>
<!-- 
CHANGEBASEGREATPEOPLERATE
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|City|ChangeBaseGreatPeopleRate}}<b>(</b>'''int''' change<b>)</b></code>
<!-- 
CHANGEBASEYIELDRATEFROMBUILDINGS
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>{{UnknownSignature5}}</code>
|width="100%" |<code>{{FuncLabel5|City|ChangeBaseYieldRateFromBuildings}}<!-- No arguments --></code>
<!-- 
CHANGEBASEYIELDRATEFROMMISC
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>{{UnknownSignature5}}</code>
|width="100%" |<code>{{FuncLabel5|City|ChangeBaseYieldRateFromMisc}}<!-- No arguments --></code>
<!-- 
CHANGEBASEYIELDRATEFROMRELIGION
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>{{UnknownSignature5}}</code>
|width="100%" |<code>{{FuncLabel5|City|ChangeBaseYieldRateFromReligion}}<!-- No arguments --></code>
<!-- 
CHANGEBASEYIELDRATEFROMSPECIALISTS
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>{{UnknownSignature5}}</code>
|width="100%" |<code>{{FuncLabel5|City|ChangeBaseYieldRateFromSpecialists}}<!-- No arguments --></code>
<!-- 
CHANGEBASEYIELDRATEFROMTERRAIN
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>{{UnknownSignature5}}</code>
|width="100%" |<code>{{FuncLabel5|City|ChangeBaseYieldRateFromTerrain}}<!-- No arguments --></code>
<!-- 
CHANGEBUILDINGPRODUCTION
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|City|ChangeBuildingProduction}}<b>(</b>{{Type5|BuildingType}} index, '''int''' change<b>)</b></code>
<!-- 
CHANGEBUILDINGPRODUCTIONTIME
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|City|ChangeBuildingProductionTime}}<b>(</b>{{Type5|BuildingType}} index, '''int''' change<b>)</b></code>
<!-- 
CHANGECULTURERATEMODIFIER
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|City|ChangeCultureRateModifier}}<b>(</b>'''int''' change<b>)</b></code>
<!-- 
CHANGECULTUREUPDATETIMER
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|City|ChangeCultureUpdateTimer}}<b>(</b>'''int''' change<b>)</b></code>
<!-- 
CHANGEDAMAGE
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|City|ChangeDamage}}<b>(</b>'''int''' change<b>)</b></code>
<!-- 
CHANGEFOOD
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|City|ChangeFood}}<b>(</b>'''int''' change<b>)</b></code>
<!-- 
CHANGEGREATPEOPLEPROGRESS
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|City|ChangeGreatPeopleProgress}}<b>(</b>'''int''' change<b>)</b></code>
<!-- 
CHANGEGREATPEOPLEUNITPROGRESS
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|City|ChangeGreatPeopleUnitProgress}}<b>(</b>{{Type5|UnitType}} index, '''int''' change<b>)</b></code>
<!-- 
CHANGEHEALRATE
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|City|ChangeHealRate}}<b>(</b>'''int''' change<b>)</b></code>
<!-- 
CHANGEJONSCULTURELEVEL
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|City|ChangeJONSCultureLevel}}<b>(</b>'''int''' change<b>)</b></code>
<!-- 
CHANGEJONSCULTUREPERTURNFROMBUILDINGS
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|City|ChangeJONSCulturePerTurnFromBuildings}}<b>(</b>'''int''' change<b>)</b></code>
<!-- 
CHANGEJONSCULTUREPERTURNFROMPOLICIES
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|City|ChangeJONSCulturePerTurnFromPolicies}}<b>(</b>'''int''' change<b>)</b></code>
<!-- 
CHANGEJONSCULTUREPERTURNFROMSPECIALISTS
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|City|ChangeJONSCulturePerTurnFromSpecialists}}<b>(</b>'''int''' change<b>)</b></code>
<!-- 
CHANGEJONSCULTURESTORED
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|City|ChangeJONSCultureStored}}<b>(</b>'''int''' change<b>)</b></code>
<!-- 
CHANGEPOPULATION
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|yes|<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|City|ChangePopulation}}<b>(</b>'''int''' change, '''bool''' flag<b>)</b></code>
<!-- 
CHANGEPRODUCTION
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|City|ChangeProduction}}<b>(</b>'''int''' change<b>)</b></code>
<!-- 
CHANGERAZINGTURNS
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|City|ChangeRazingTurns}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
CHANGERESISTANCETURNS
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|City|ChangeResistanceTurns}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
CHANGESPECIALISTGREATPERSONPROGRESSTIMES100
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|City|ChangeSpecialistGreatPersonProgressTimes100}}<b>(</b>{{Type5|SpecialistType}} index, '''int''' change<b>)</b></code>
<!-- 
CHANGEUNITPRODUCTION
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|City|ChangeUnitProduction}}<b>(</b>{{Type5|UnitType}} index, '''int''' change<b>)</b></code>
<!-- 
CHANGEWELOVETHEKINGDAYCOUNTER
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|City|ChangeWeLoveTheKingDayCounter}}<b>(</b>'''int''' change<b>)</b></code>
<!-- 
CHANGEWONDERPRODUCTIONMODIFIER
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|City|ChangeWonderProductionModifier}}<b>(</b>'''int''' change<b>)</b></code>
<!-- 
CHOOSEPRODUCTION
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|City|ChooseProduction}}<b>(</b>{{Type5|UnitType}} trainUnit, {{Type5|BuildingType}} constructBuilding, {{Type5|ProjectType}} createProject, '''bool''' finish, '''bool''' front<b>)</b></code>
<!-- 
CLEARORDERQUEUE
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>{{UnknownSignature5}}</code>
|width="100%" |<code>{{FuncLabel5|City|ClearOrderQueue}}<!-- No arguments --></code>
<!-- 
CLEARWORKINGOVERRIDE
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|City|ClearWorkingOverride}}<b>(</b>'''int''' index<b>)</b></code>
<!-- 
CONSCRIPT
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>{{UnknownSignature5}}</code>
|width="100%" |<code>{{FuncLabel5|City|Conscript}}<!-- No arguments --></code>
<!-- 
CONSCRIPTMINCITYPOPULATION
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|City|ConscriptMinCityPopulation}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
CONVERTPERCENTFOLLOWERS
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|City|ConvertPercentFollowers}}<b>(</b>{{Type5|ReligionType}} arg0, {{Type5|ReligionType}} arg1, '''int''' arg2<b>)</b></code>
<!-- 
COUNTNUMIMPROVEDPLOTS
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|City|CountNumImprovedPlots}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
COUNTNUMRIVERPLOTS
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|City|CountNumRiverPlots}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
COUNTNUMWATERPLOTS
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|City|CountNumWaterPlots}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
CREATEAPOLLOPROGRAM
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>{{UnknownSignature5}}</code>
|width="100%" |<code>{{FuncLabel5|City|CreateApolloProgram}}<!-- No arguments --></code>
<!-- 
CREATEGREATADMIRAL
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>{{UnknownSignature5}}</code>
|width="100%" |<code>{{FuncLabel5|City|CreateGreatAdmiral}}<!-- No arguments --></code>
<!-- 
CREATEGREATGENERAL
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|City|CreateGreatGeneral}}<b>(</b>{{Type5|UnitType}} greatPersonUnit<b>)</b></code>
|}

==D==
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
DOJONSCULTURELEVELINCREASE
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>{{UnknownSignature5}}</code>
|width="100%" |<code>{{FuncLabel5|City|DoJONSCultureLevelIncrease}}<!-- No arguments --></code>
<!-- 
DOPICKRESOURCEDEMANDED
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|City|DoPickResourceDemanded}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
DOREALLOCATECITIZENS
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|City|DoReallocateCitizens}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
DOTASK
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|City|DoTask}}<b>(</b>{{Type5|TaskType}} task, '''int''' data1, '''int''' data2, '''bool''' option<b>)</b></code>
<!-- 
DOVERIFYWORKINGPLOTS
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|City|DoVerifyWorkingPlots}}<b>(</b><!-- No arguments --><b>)</b></code>
|}

==F==
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
FINDBASEYIELDRATERANK
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|City|FindBaseYieldRateRank}}<b>(</b>{{Type5|YieldType}} yield<b>)</b></code>
<!-- 
FINDPOPULATIONRANK
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|City|FindPopulationRank}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
FINDYIELDRATERANK
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|City|FindYieldRateRank}}<b>(</b>{{Type5|YieldType}} yield<b>)</b></code>
<!-- 
FOODCONSUMPTION
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|City|FoodConsumption}}<b>(</b>'''bool''' noAngry, '''int''' extra<b>)</b></code>
<!-- 
FOODDIFFERENCE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|City|FoodDifference}}<b>(</b>'''bool''' bottom<b>)</b></code>
<!-- 
FOODDIFFERENCETIMES100
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|City|FoodDifferenceTimes100}}<b>(</b>'''bool''' bottom<b>)</b></code>
|}

==G==
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
GETAIRMODIFIER
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|City|GetAirModifier}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETARTSTYLETYPE
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>{{Type5|ArtStyleType}}</code>
|width="100%" |<code>{{FuncLabel5|City|GetArtStyleType}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETBASEGREATPEOPLERATE
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|City|GetBaseGreatPeopleRate}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETBASEJONSCULTUREPERTURN
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|City|GetBaseJONSCulturePerTurn}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETBASEYIELDRATE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|City|GetBaseYieldRate}}<b>(</b>{{Type5|YieldType}} index<b>)</b></code>
<!-- 
GETBASEYIELDRATEFROMBUILDINGS
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|City|GetBaseYieldRateFromBuildings}}<b>(</b>{{Type5|YieldType}} yieldType<b>)</b></code>
<!-- 
GETBASEYIELDRATEFROMMISC
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|City|GetBaseYieldRateFromMisc}}<b>(</b>{{Type5|YieldType}} yieldType<b>)</b></code>
<!-- 
GETBASEYIELDRATEFROMRELIGION
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|City|GetBaseYieldRateFromReligion}}<b>(</b>{{Type5|YieldType}} yieldType<b>)</b></code>
<!-- 
GETBASEYIELDRATEFROMSPECIALISTS
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|City|GetBaseYieldRateFromSpecialists}}<b>(</b>{{Type5|YieldType}} yieldType<b>)</b></code>
<!-- 
GETBASEYIELDRATEFROMTERRAIN
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|City|GetBaseYieldRateFromTerrain}}<b>(</b>{{Type5|YieldType}} yieldType<b>)</b></code>
<!-- 
GETBASEYIELDRATEMODIFIER
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|City|GetBaseYieldRateModifier}}<b>(</b>{{Type5|YieldType}} index, '''int''' extra = 0<b>)</b></code>
<!-- 
GETBUILDINGDEFENSE
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|City|GetBuildingDefense}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETBUILDINGESPIONAGEMODIFIER
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|City|GetBuildingEspionageModifier}}<b>(</b>{{Type5|BuildingType}} building<b>)</b></code>
<!-- 
GETBUILDINGFAITHPURCHASECOST
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|City|GetBuildingFaithPurchaseCost}}<b>(</b>{{Type5|BuildingType}} building, '''bool''' arg1 = nil<b>)</b></code>
<!-- 
GETBUILDINGGLOBALESPIONAGEMODIFIER
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|City|GetBuildingGlobalEspionageModifier}}<b>(</b>{{Type5|BuildingType}} building<b>)</b></code>
<!-- 
GETBUILDINGORIGINALOWNER
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|City|GetBuildingOriginalOwner}}<b>(</b>{{Type5|BuildingType}} index<b>)</b></code>
<!-- 
GETBUILDINGORIGINALTIME
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|City|GetBuildingOriginalTime}}<b>(</b>{{Type5|BuildingType}} index<b>)</b></code>
<!-- 
GETBUILDINGPRODUCTION
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|City|GetBuildingProduction}}<b>(</b>{{Type5|BuildingType}} index<b>)</b></code>
<!-- 
GETBUILDINGPRODUCTIONMODIFIER
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|City|GetBuildingProductionModifier}}<b>(</b>{{Type5|BuildingType}} building<b>)</b></code>
<!-- 
GETBUILDINGPRODUCTIONNEEDED
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|City|GetBuildingProductionNeeded}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETBUILDINGPRODUCTIONTIME
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|City|GetBuildingProductionTime}}<b>(</b>{{Type5|BuildingType}} index<b>)</b></code>
<!-- 
GETBUILDINGPRODUCTIONTURNSLEFT
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|City|GetBuildingProductionTurnsLeft}}<b>(</b>{{Type5|BuildingType}} building, '''int''' num<b>)</b></code>
<!-- 
GETBUILDINGPURCHASECOST
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|City|GetBuildingPurchaseCost}}<b>(</b>{{Type5|BuildingType}} building<b>)</b></code>
<!-- 
GETBUILDINGYIELDCHANGE
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|City|GetBuildingYieldChange}}<b>(</b>{{Type5|BuildingClassType}} buildingClass, {{Type5|YieldType}} yield<b>)</b></code>
<!-- 
GETBUYABLEPLOTLIST
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''...'''</code>
|width="100%" |<code>{{FuncLabel5|City|GetBuyablePlotList}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETBUYPLOTCOST
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|City|GetBuyPlotCost}}<b>(</b>'''int''' x, '''int''' y<b>)</b></code>
<!-- 
GETCITYINDEXPLOT
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>{{Type5|Plot}}</code>
|width="100%" |<code>{{FuncLabel5|City|GetCityIndexPlot}}<b>(</b>{{Type5|CityPlotID}} index<b>)</b></code>
<!-- 
GETCITYPLOTINDEX
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>{{Type5|CityPlotID}}</code>
|width="100%" |<code>{{FuncLabel5|City|GetCityPlotIndex}}<b>(</b>{{Type5|Plot}} plot<b>)</b></code>
<!-- 
GETCITYSIZETYPE
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''unknown'''</code>
|width="100%" |<code>{{FuncLabel5|City|GetCitySizeType}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETCIVILIZATIONTYPE
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>{{Type5|CivilizationType}}</code>
|width="100%" |<code>{{FuncLabel5|City|GetCivilizationType}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETCONSCRIPTPOPULATION
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|City|GetConscriptPopulation}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETCONSCRIPTUNIT
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>{{Type5|UnitType}}</code>
|width="100%" |<code>{{FuncLabel5|City|GetConscriptUnit}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETCULTUREFROMSPECIALIST
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|City|GetCultureFromSpecialist}}<b>(</b>{{Type5|SpecialistType}} specialist<b>)</b></code>
<!-- 
GETCULTURERATEMODIFIER
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|City|GetCultureRateModifier}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETCULTUREUPDATETIMER
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|City|GetCultureUpdateTimer}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETCURRAIRLIFT
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|City|GetCurrAirlift}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETCURRENTPRODUCTIONDIFFERENCE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|City|GetCurrentProductionDifference}}<b>(</b>'''bool''' ignoreFood, '''bool''' overflow<b>)</b></code>
<!-- 
GETCURRENTPRODUCTIONDIFFERENCETIMES100
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|City|GetCurrentProductionDifferenceTimes100}}<b>(</b>'''bool''' ignoreFood, '''bool''' overflow<b>)</b></code>
<!-- 
GETDAMAGE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|City|GetDamage}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETDOMAINFREEEXPERIENCE
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|City|GetDomainFreeExperience}}<b>(</b>{{Type5|DomainType}} index<b>)</b></code>
<!-- 
GETDOMAINPRODUCTIONMODIFIER
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|City|GetDomainProductionModifier}}<b>(</b>{{Type5|DomainType}} index<b>)</b></code>
<!-- 
GETEXTRAPRODUCTIONDIFFERENCE
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|City|GetExtraProductionDifference}}<b>(</b>'''int''' extra<b>)</b></code>
<!-- 
GETEXTRASPECIALISTYIELD
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|City|GetExtraSpecialistYield}}<b>(</b>{{Type5|YieldType}} index<b>)</b></code>
<!-- 
GETEXTRASPECIALISTYIELDOFTYPE
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|City|GetExtraSpecialistYieldOfType}}<b>(</b>{{Type5|YieldType}} index, {{Type5|SpecialistType}} specialist<b>)</b></code>
<!-- 
GETFAITHPERTURN
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|City|GetFaithPerTurn}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETFAITHPERTURNFROMBUILDINGS
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|City|GetFaithPerTurnFromBuildings}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETFAITHPERTURNFROMPOLICIES
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|City|GetFaithPerTurnFromPolicies}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETFAITHPERTURNFROMRELIGION
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|City|GetFaithPerTurnFromReligion}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETFAITHPERTURNFROMTRAITS
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|City|GetFaithPerTurnFromTraits}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETFAITHPURCHASEBUILDINGTOOLTIP
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|City|GetFaithPurchaseBuildingTooltip}}<b>(</b>'''int''' id<b>)</b></code>
<!-- 
GETFAITHPURCHASEUNITTOOLTIP
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|City|GetFaithPurchaseUnitTooltip}}<b>(</b>{{Type5|UnitType}} id<b>)</b></code>
<!-- 
GETFAVOREDRELIGION
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>{{UnknownSignature5}}</code>
|width="100%" |<code>{{FuncLabel5|City|GetFavoredReligion}}<!-- No arguments --></code>
<!-- 
GETFEATUREPRODUCTION
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|City|GetFeatureProduction}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETFIRSTBUILDINGORDER
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|City|GetFirstBuildingOrder}}<b>(</b>{{Type5|BuildingType}} building<b>)</b></code>
<!-- 
GETFIRSTPROJECTORDER
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|City|GetFirstProjectOrder}}<b>(</b>{{Type5|ProjectType}} project<b>)</b></code>
<!-- 
GETFIRSTSPECIALISTORDER
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|City|GetFirstSpecialistOrder}}<b>(</b>{{Type5|SpecialistType}} specialist<b>)</b></code>
<!-- 
GETFIRSTUNITORDER
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|City|GetFirstUnitOrder}}<b>(</b>{{Type5|UnitType}} unit<b>)</b></code>
<!-- 
GETFOCUSTYPE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>{{Type5|CityAIFocusType}}</code>
|width="100%" |<code>{{FuncLabel5|City|GetFocusType}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETFOOD
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|City|GetFood}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETFOODKEPT
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|City|GetFoodKept}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETFOODTIMES100
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|City|GetFoodTimes100}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETFOODTURNSLEFT
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|City|GetFoodTurnsLeft}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETFREEEXPERIENCE
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|City|GetFreeExperience}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETFREEPROMOTIONCOUNT
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|City|GetFreePromotionCount}}<b>(</b>{{Type5|PromotionType}} index<b>)</b></code>
<!-- 
GETGAMETURNACQUIRED
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|City|GetGameTurnAcquired}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETGAMETURNFOUNDED
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|City|GetGameTurnFounded}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETGAMETURNLASTEXPANDED
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|City|GetGameTurnLastExpanded}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETGARRISONEDUNIT
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>{{Type5|Unit}}</code>
|width="100%" |<code>{{FuncLabel5|City|GetGarrisonedUnit}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETGENERALPRODUCTIONTURNSLEFT
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|City|GetGeneralProductionTurnsLeft}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETGREATPEOPLEPROGRESS
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|City|GetGreatPeopleProgress}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETGREATPEOPLERATE
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|City|GetGreatPeopleRate}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETGREATPEOPLERATEMODIFIER
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|City|GetGreatPeopleRateModifier}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETGREATPEOPLEUNITPROGRESS
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|City|GetGreatPeopleUnitProgress}}<b>(</b>{{Type5|UnitType}} index<b>)</b></code>
<!-- 
GETGREATPEOPLEUNITRATE
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|City|GetGreatPeopleUnitRate}}<b>(</b>{{Type5|UnitType}} index<b>)</b></code>
<!-- 
GETHANDICAPTYPE
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>{{Type5|HandicapType}}</code>
|width="100%" |<code>{{FuncLabel5|City|GetHandicapType}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETHAPPINESS
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|City|GetHappiness}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETHAPPINESSFROMBUILDINGS
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>{{UnknownSignature5}}</code>
|width="100%" |<code>{{FuncLabel5|City|GetHappinessFromBuildings}}<!-- No arguments --></code>
<!-- 
GETHIGHESTPOPULATION
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|City|GetHighestPopulation}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETID
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>{{Type5|CityID}}</code>
|width="100%" |<code>{{FuncLabel5|City|GetID}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETJONSCULTURELEVEL
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|City|GetJONSCultureLevel}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETJONSCULTUREPERTURN
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|City|GetJONSCulturePerTurn}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETJONSCULTUREPERTURNFROMBUILDINGS
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|City|GetJONSCulturePerTurnFromBuildings}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETJONSCULTUREPERTURNFROMPOLICIES
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|City|GetJONSCulturePerTurnFromPolicies}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETJONSCULTUREPERTURNFROMRELIGION
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|City|GetJONSCulturePerTurnFromReligion}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETJONSCULTUREPERTURNFROMSPECIALISTS
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|City|GetJONSCulturePerTurnFromSpecialists}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETJONSCULTUREPERTURNFROMTERRAIN
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|City|GetJONSCulturePerTurnFromTerrain}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETJONSCULTUREPERTURNFROMTRAITS
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|City|GetJONSCulturePerTurnFromTraits}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETJONSCULTURESTORED
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|City|GetJONSCultureStored}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETJONSCULTURETHRESHOLD
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|City|GetJONSCultureThreshold}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETLAKEPLOTYIELD
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|City|GetLakePlotYield}}<b>(</b>{{Type5|YieldType}} index<b>)</b></code>
<!-- 
GETLOCALHAPPINESS
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|City|GetLocalHappiness}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETLOCALRESOURCEWONDERPRODUCTIONMOD
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|City|GetLocalResourceWonderProductionMod}}<b>(</b>{{Type5|BuildingType}} building<b>)</b></code>
<!-- 
GETMAXAIRLIFT
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|City|GetMaxAirlift}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETMAXFOODKEPTPERCENT
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|City|GetMaxFoodKeptPercent}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETMAXHITPOINTS
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|City|GetMaxHitPoints}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETMILITARYPRODUCTIONMODIFIER
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|City|GetMilitaryProductionModifier}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETNAME
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''string'''</code>
|width="100%" |<code>{{FuncLabel5|City|GetName}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETNAMEKEY
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''string'''</code>
|width="100%" |<code>{{FuncLabel5|City|GetNameKey}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETNEXTBUYABLEPLOT
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''unknown'''</code>
|width="100%" |<code>{{FuncLabel5|City|GetNextBuyablePlot}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETNUKEMODIFIER
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|City|GetNukeModifier}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETNUMACTIVEBUILDING
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|City|GetNumActiveBuilding}}<b>(</b>{{Type5|BuildingType}} buildingType<b>)</b></code>
<!-- 
GETNUMBUILDING
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|City|GetNumBuilding}}<b>(</b>{{Type5|BuildingType}} buildingType<b>)</b></code>
<!-- 
GETNUMBUILDINGS
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|City|GetNumBuildings}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETNUMCITYPLOTS
-->
|-
{{FuncInfos5|yes  |yes  |yes|<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|City|GetNumCityPlots}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETNUMFOLLOWERS
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|City|GetNumFollowers}}<b>(</b>{{Type5|ReligionType}} religion<b>)</b></code>
<!-- 
GETNUMFORCEDWORKINGPLOTS
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|City|GetNumForcedWorkingPlots}}<b>(</b>{{Type5|Plot}} plot<b>)</b></code>
<!-- 
GETNUMFREEBUILDING
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|City|GetNumFreeBuilding}}<b>(</b>{{Type5|BuildingType}} index<b>)</b></code>
<!-- 
GETNUMGREATPEOPLE
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|City|GetNumGreatPeople}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETNUMNATIONALWONDERS
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|City|GetNumNationalWonders}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETNUMREALBUILDING
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|City|GetNumRealBuilding}}<b>(</b>{{Type5|BuildingType}} index<b>)</b></code>
<!-- 
GETNUMSPECIALISTSALLOWEDBYBUILDING
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|City|GetNumSpecialistsAllowedByBuilding}}<b>(</b>{{Type5|BuildingType}} building<b>)</b></code>
<!-- 
GETNUMSPECIALISTSINBUILDING
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|City|GetNumSpecialistsInBuilding}}<b>(</b>{{Type5|BuildingType}} index<b>)</b></code>
<!-- 
GETNUMTEAMWONDERS
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|City|GetNumTeamWonders}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETNUMTHINGSPRODUCED
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|City|GetNumThingsProduced}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETNUMTRAINUNITAI
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|City|GetNumTrainUnitAI}}<b>(</b>{{Type5|UnitAIType}} unitAI<b>)</b></code>
<!-- 
GETNUMWORLDWONDERS
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|City|GetNumWorldWonders}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETORDERFROMQUEUE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>{{Type5|OrderType}}, '''int''', '''unknown''', '''unknown''', '''unknown'''</code>
|width="100%" |<code>{{FuncLabel5|City|GetOrderFromQueue}}<b>(</b>'''int''' arg0<b>)</b></code>
<!-- 
GETORDERQUEUELENGTH
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|City|GetOrderQueueLength}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETORIGINALOWNER
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>{{Type5|PlayerID}}</code>
|width="100%" |<code>{{FuncLabel5|City|GetOriginalOwner}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETOVERFLOWPRODUCTION
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|City|GetOverflowProduction}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETOWNER
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>{{Type5|PlayerID}}</code>
|width="100%" |<code>{{FuncLabel5|City|GetOwner}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETPERSONALITYTYPE
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>{{Type5|LeaderType}}</code>
|width="100%" |<code>{{FuncLabel5|City|GetPersonalityType}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETPOPULATION
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|City|GetPopulation}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETPRESSUREPERTURN
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|City|GetPressurePerTurn}}<b>(</b>{{Type5|ReligionType}} religion<b>)</b></code>
<!-- 
GETPREVIOUSOWNER
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>{{Type5|PlayerID}}</code>
|width="100%" |<code>{{FuncLabel5|City|GetPreviousOwner}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETPRODUCTION
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|City|GetProduction}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETPRODUCTIONBUILDING
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>{{Type5|BuildingType}}</code>
|width="100%" |<code>{{FuncLabel5|City|GetProductionBuilding}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETPRODUCTIONEXPERIENCE
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|City|GetProductionExperience}}<b>(</b>{{Type5|UnitType}} unit<b>)</b></code>
<!-- 
GETPRODUCTIONMODIFIER
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|City|GetProductionModifier}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETPRODUCTIONNAMEKEY
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''string'''</code>
|width="100%" |<code>{{FuncLabel5|City|GetProductionNameKey}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETPRODUCTIONNEEDED
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|City|GetProductionNeeded}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETPRODUCTIONPROCESS
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>{{Type5|ProcessType}}</code>
|width="100%" |<code>{{FuncLabel5|City|GetProductionProcess}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETPRODUCTIONPROJECT
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>{{Type5|ProjectType}}</code>
|width="100%" |<code>{{FuncLabel5|City|GetProductionProject}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETPRODUCTIONSPECIALIST
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>{{Type5|SpecialistType}}</code>
|width="100%" |<code>{{FuncLabel5|City|GetProductionSpecialist}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETPRODUCTIONTIMES100
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|City|GetProductionTimes100}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETPRODUCTIONTURNSLEFT
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|City|GetProductionTurnsLeft}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETPRODUCTIONUNIT
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>{{Type5|UnitType}}</code>
|width="100%" |<code>{{FuncLabel5|City|GetProductionUnit}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETPRODUCTIONUNITAI
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>{{Type5|UnitAIType}}</code>
|width="100%" |<code>{{FuncLabel5|City|GetProductionUnitAI}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETPROJECTPRODUCTIONMODIFIER
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|City|GetProjectProductionModifier}}<b>(</b>{{Type5|ProjectType}} project<b>)</b></code>
<!-- 
GETPROJECTPRODUCTIONNEEDED
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|City|GetProjectProductionNeeded}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETPROJECTPRODUCTIONTURNSLEFT
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|City|GetProjectProductionTurnsLeft}}<b>(</b>{{Type5|ProjectType}} project, '''int''' num<b>)</b></code>
<!-- 
GETPROJECTPURCHASECOST
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|City|GetProjectPurchaseCost}}<b>(</b>{{Type5|ProjectType}} project<b>)</b></code>
<!-- 
GETPURCHASEBUILDINGTOOLTIP
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|City|GetPurchaseBuildingTooltip}}<b>(</b>'''int''' id<b>)</b></code>
<!-- 
GETPURCHASEUNITTOOLTIP
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|City|GetPurchaseUnitTooltip}}<b>(</b>{{Type5|UnitType}} id<b>)</b></code>
<!-- 
GETRALLYPLOT
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''unknown'''</code>
|width="100%" |<code>{{FuncLabel5|City|GetRallyPlot}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETRAWPRODUCTIONDIFFERENCE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|City|GetRawProductionDifference}}<b>(</b>'''bool''' arg0, '''bool''' arg1<b>)</b></code>
<!-- 
GETRAWPRODUCTIONDIFFERENCETIMES100
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>{{UnknownSignature5}}</code>
|width="100%" |<code>{{FuncLabel5|City|GetRawProductionDifferenceTimes100}}<!-- No arguments --></code>
<!-- 
GETRAZINGTURNS
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|City|GetRazingTurns}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETREALPOPULATION
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|City|GetRealPopulation}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETRELIGIONBUILDINGCLASSHAPPINESS
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|City|GetReligionBuildingClassHappiness}}<b>(</b>{{Type5|BuildingClassType}} buildingClass<b>)</b></code>
<!-- 
GETRELIGIONBUILDINGCLASSYIELDCHANGE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|City|GetReligionBuildingClassYieldChange}}<b>(</b>{{Type5|BuildingClassType}} buildingClass, {{Type5|YieldType}} arg1<b>)</b></code>
<!-- 
GETRELIGIONCITYRANGESTRIKEMODIFIER
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|City|GetReligionCityRangeStrikeModifier}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETRELIGIOUSMAJORITY
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>{{Type5|ReligionType}}</code>
|width="100%" |<code>{{FuncLabel5|City|GetReligiousMajority}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETRESISTANCETURNS
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|City|GetResistanceTurns}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETRESOURCEDEMANDED
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>{{Type5|ResourceType}}</code>
|width="100%" |<code>{{FuncLabel5|City|GetResourceDemanded}}<b>(</b>'''bool''' arg0 = nil<b>)</b></code>
<!-- 
GETRESOURCEYIELDRATEMODIFIER
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|City|GetResourceYieldRateModifier}}<b>(</b>{{Type5|YieldType}} index, {{Type5|ResourceType}} resource<b>)</b></code>
<!-- 
GETRIVERPLOTYIELD
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|City|GetRiverPlotYield}}<b>(</b>{{Type5|YieldType}} index<b>)</b></code>
<!-- 
GETSEAPLOTYIELD
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|City|GetSeaPlotYield}}<b>(</b>{{Type5|YieldType}} index<b>)</b></code>
<!-- 
GETSELLBUILDINGREFUND
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|City|GetSellBuildingRefund}}<b>(</b>{{Type5|BuildingType}} index<b>)</b></code>
<!-- 
GETSPACEPRODUCTIONMODIFIER
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|City|GetSpaceProductionModifier}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETSPECIALISTCOUNT
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|City|GetSpecialistCount}}<b>(</b>{{Type5|SpecialistType}} index<b>)</b></code>
<!-- 
GETSPECIALISTFREEEXPERIENCE
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|City|GetSpecialistFreeExperience}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETSPECIALISTGREATPERSONPROGRESS
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|City|GetSpecialistGreatPersonProgress}}<b>(</b>{{Type5|SpecialistType}} index<b>)</b></code>
<!-- 
GETSPECIALISTGREATPERSONPROGRESSTIMES100
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|City|GetSpecialistGreatPersonProgressTimes100}}<b>(</b>{{Type5|SpecialistType}} index<b>)</b></code>
<!-- 
GETSPECIALISTPRODUCTIONMODIFIER
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|City|GetSpecialistProductionModifier}}<b>(</b>{{Type5|SpecialistType}} specialist<b>)</b></code>
<!-- 
GETSPECIALISTPRODUCTIONTURNSLEFT
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|City|GetSpecialistProductionTurnsLeft}}<b>(</b>{{Type5|SpecialistType}} specialist, '''int''' num<b>)</b></code>
<!-- 
GETSPECIALISTUPGRADETHRESHOLD
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|City|GetSpecialistUpgradeThreshold}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETSPECIALISTYIELD
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|City|GetSpecialistYield}}<b>(</b>{{Type5|SpecialistType}} specialist, {{Type5|YieldType}} yield<b>)</b></code>
<!-- 
GETSTRENGTHVALUE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|City|GetStrengthValue}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETTEAM
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>{{Type5|TeamID}}</code>
|width="100%" |<code>{{FuncLabel5|City|GetTeam}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETTOTALBASEBUILDINGMAINTENANCE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|City|GetTotalBaseBuildingMaintenance}}<b>(</b>{{Type5|BuildingType}} index<b>)</b></code>
<!-- 
GETTOTALGREATPEOPLERATEMODIFIER
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|City|GetTotalGreatPeopleRateModifier}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETUNITCOMBATFREEEXPERIENCE
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|City|GetUnitCombatFreeExperience}}<b>(</b>{{Type5|UnitCombatType}} index<b>)</b></code>
<!-- 
GETUNITFAITHPURCHASECOST
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|City|GetUnitFaithPurchaseCost}}<b>(</b>{{Type5|UnitType}} unit, '''bool''' arg1<b>)</b></code>
<!-- 
GETUNITPRODUCTION
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|City|GetUnitProduction}}<b>(</b>'''int''' index<b>)</b></code>
<!-- 
GETUNITPRODUCTIONMODIFIER
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|City|GetUnitProductionModifier}}<b>(</b>{{Type5|UnitType}} unit<b>)</b></code>
<!-- 
GETUNITPRODUCTIONNEEDED
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|City|GetUnitProductionNeeded}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETUNITPRODUCTIONTURNSLEFT
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|City|GetUnitProductionTurnsLeft}}<b>(</b>{{Type5|UnitType}} unit, '''int''' num<b>)</b></code>
<!-- 
GETUNITPURCHASECOST
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|City|GetUnitPurchaseCost}}<b>(</b>{{Type5|UnitType}} unit<b>)</b></code>
<!-- 
GETWELOVETHEKINGDAYCOUNTER
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|City|GetWeLoveTheKingDayCounter}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETWONDERPRODUCTIONMODIFIER
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|City|GetWonderProductionModifier}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETX
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>{{Type5|ResourceType}}</code>
|width="100%" |<code>{{FuncLabel5|City|GetX}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETY
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>{{Type5|ResourceType}}</code>
|width="100%" |<code>{{FuncLabel5|City|GetY}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETYIELDMODIFIERTOOLTIP
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''string'''</code>
|width="100%" |<code>{{FuncLabel5|City|GetYieldModifierTooltip}}<b>(</b>{{Type5|YieldType}} yieldType<b>)</b></code>
<!-- 
GETYIELDPERPOPTIMES100
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|City|GetYieldPerPopTimes100}}<b>(</b>{{Type5|YieldType}} yieldType<b>)</b></code>
<!-- 
GETYIELDRATE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|City|GetYieldRate}}<b>(</b>{{Type5|YieldType}} index<b>)</b></code>
<!-- 
GETYIELDRATEMODIFIER
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|City|GetYieldRateModifier}}<b>(</b>{{Type5|YieldType}} index<b>)</b></code>
<!-- 
GETYIELDRATETIMES100
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|City|GetYieldRateTimes100}}<b>(</b>{{Type5|YieldType}} index<b>)</b></code>
<!-- 
GROWTHTHRESHOLD
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|City|GrowthThreshold}}<b>(</b><!-- No arguments --><b>)</b></code>
|}

==H==
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
HASPERFORMEDRANGEDSTRIKETHISTURN
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|City|HasPerformedRangedStrikeThisTurn}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
HURRY
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|City|Hurry}}<b>(</b>{{Type5|HurryType}} hurry<b>)</b></code>
<!-- 
HURRYCOST
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|City|HurryCost}}<b>(</b>{{Type5|HurryType}} hurry, '''bool''' extra<b>)</b></code>
<!-- 
HURRYGOLD
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|City|HurryGold}}<b>(</b>{{Type5|HurryType}} hurry<b>)</b></code>
<!-- 
HURRYPOPULATION
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|City|HurryPopulation}}<b>(</b>{{Type5|HurryType}} hurry<b>)</b></code>
<!-- 
HURRYPRODUCTION
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|City|HurryProduction}}<b>(</b>{{Type5|HurryType}} hurry<b>)</b></code>
|}

==I==
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
ISAIRLIFTTARGETED
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|City|IsAirliftTargeted}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ISBARBARIAN
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|City|IsBarbarian}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ISBLOCKADED
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|City|IsBlockaded}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ISBUILDINGLOCALRESOURCEVALID
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|City|IsBuildingLocalResourceValid}}<b>(</b>{{Type5|BuildingType}} building, '''bool''' checkForImprovement<b>)</b></code>
<!-- 
ISBUILDINGSELLABLE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|City|IsBuildingSellable}}<b>(</b>{{Type5|BuildingType}} index<b>)</b></code>
<!-- 
ISBUILDINGSMAXED
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|City|IsBuildingsMaxed}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ISCANADDSPECIALISTTOBUILDING
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|City|IsCanAddSpecialistToBuilding}}<b>(</b>{{Type5|BuildingType}} building<b>)</b></code>
<!-- 
ISCANPURCHASE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|City|IsCanPurchase}}<b>(</b>{{Type5|UnitType}} unitType, '''int''' buildingType, '''int''' projectType, '''int''' projectID, '''int''' projectID = nil, {{Type5|YieldType}} yield = nil<b>)</b></code>
<!-- 
ISCAPITAL
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|City|IsCapital}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ISCOASTAL
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|City|IsCoastal}}<b>(</b>'''int''' minWaterSize<b>)</b></code>
<!-- 
ISDRAFTED
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|City|IsDrafted}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ISEVEROWNED
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|City|IsEverOwned}}<b>(</b>{{Type5|PlayerID}} index<b>)</b></code>
<!-- 
ISFOODPRODUCTION
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|City|IsFoodProduction}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ISFORCEDAVOIDGROWTH
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|City|IsForcedAvoidGrowth}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ISFORCEDWORKINGPLOT
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|City|IsForcedWorkingPlot}}<b>(</b>{{Type5|Plot}} plot<b>)</b></code>
<!-- 
ISFREEPROMOTION
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|City|IsFreePromotion}}<b>(</b>{{Type5|PromotionType}} index<b>)</b></code>
<!-- 
ISHASBUILDING
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|City|IsHasBuilding}}<b>(</b>{{Type5|BuildingType}} building<b>)</b></code>
<!-- 
ISHASRESOURCELOCAL
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|City|IsHasResourceLocal}}<b>(</b>{{Type5|ResourceType}} resource<b>)</b></code>
<!-- 
ISHOLYCITYANYRELIGION
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>{{UnknownSignature5}}</code>
|width="100%" |<code>{{FuncLabel5|City|IsHolyCityAnyReligion}}<!-- No arguments --></code>
<!-- 
ISHOLYCITYFORRELIGION
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|City|IsHolyCityForReligion}}<b>(</b>{{Type5|ReligionType}} religion<b>)</b></code>
<!-- 
ISHUMAN
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|City|IsHuman}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ISNATIONALWONDERSMAXED
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|City|IsNationalWondersMaxed}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ISNEVERLOST
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|City|IsNeverLost}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ISNOAUTOASSIGNSPECIALISTS
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|City|IsNoAutoAssignSpecialists}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ISNONE
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|City|IsNone}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ISNOOCCUPIEDUNHAPPINESS
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|City|IsNoOccupiedUnhappiness}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ISOCCUPIED
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|City|IsOccupied}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ISORIGINALCAPITAL
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>{{UnknownSignature5}}</code>
|width="100%" |<code>{{FuncLabel5|City|IsOriginalCapital}}<!-- No arguments --></code>
<!-- 
ISPLOTBLOCKADED
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|City|IsPlotBlockaded}}<b>(</b>{{Type5|Plot}} plot<b>)</b></code>
<!-- 
ISPRODUCTION
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|City|IsProduction}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ISPRODUCTIONAUTOMATED
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|City|IsProductionAutomated}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ISPRODUCTIONBUILDING
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|City|IsProductionBuilding}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ISPRODUCTIONLIMITED
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|City|IsProductionLimited}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ISPRODUCTIONPROCESS
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|City|IsProductionProcess}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ISPRODUCTIONPROJECT
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|City|IsProductionProject}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ISPRODUCTIONSPECIALIST
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|City|IsProductionSpecialist}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ISPRODUCTIONUNIT
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|City|IsProductionUnit}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ISPUPPET
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|City|IsPuppet}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ISRAZING
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|City|IsRazing}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ISRELIGIONINCITY
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>{{UnknownSignature5}}</code>
|width="100%" |<code>{{FuncLabel5|City|IsReligionInCity}}<!-- No arguments --></code>
<!-- 
ISRESISTANCE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|City|IsResistance}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ISREVEALED
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|City|IsRevealed}}<b>(</b>{{Type5|TeamID}} index, '''bool''' debug<b>)</b></code>
<!-- 
ISTEAMWONDERSMAXED
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|City|IsTeamWondersMaxed}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ISUNITFOODPRODUCTION
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|City|IsUnitFoodProduction}}<b>(</b>{{Type5|UnitType}} unit<b>)</b></code>
<!-- 
ISVISIBLE
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|City|IsVisible}}<b>(</b>{{Type5|TeamID}} team, '''bool''' debug<b>)</b></code>
<!-- 
ISWORKINGPLOT
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|City|IsWorkingPlot}}<b>(</b>{{Type5|Plot}} plot<b>)</b></code>
<!-- 
ISWORLDWONDERSMAXED
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|City|IsWorldWondersMaxed}}<b>(</b><!-- No arguments --><b>)</b></code>
|}

==K==
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
KILL
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>{{UnknownSignature5}}</code>
|width="100%" |<code>{{FuncLabel5|City|Kill}}<!-- No arguments --></code>
|}

==M==
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
MAXHURRYPOPULATION
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|City|MaxHurryPopulation}}<b>(</b><!-- No arguments --><b>)</b></code>
|}

==P==
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
PLOT
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>{{Type5|Plot}}</code>
|width="100%" |<code>{{FuncLabel5|City|Plot}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
POPORDER
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|City|PopOrder}}<b>(</b>'''int''' num, '''bool''' finish, '''bool''' choose<b>)</b></code>
<!-- 
PRODUCTIONLEFT
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|City|ProductionLeft}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
PUSHORDER
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|City|PushOrder}}<b>(</b>{{Type5|OrderType}} order, '''int''' data1, '''int''' data2, '''bool''' save, '''bool''' pop, '''bool''' append, '''bool''' force<b>)</b></code>
|}

==R==
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
RANGECOMBATDAMAGE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|City|RangeCombatDamage}}<b>(</b>{{Type5|Unit}} theirUnit, '''unknown''' arg1<b>)</b></code>
<!-- 
RANGECOMBATUNITDEFENSE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|City|RangeCombatUnitDefense}}<b>(</b>{{Type5|Unit}} theirUnit<b>)</b></code>
|}

==S==
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
SETAIRLIFTTARGETED
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|City|SetAirliftTargeted}}<b>(</b>'''int''' newValue<b>)</b></code>
<!-- 
SETBUILDINGPRODUCTION
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|City|SetBuildingProduction}}<b>(</b>{{Type5|BuildingType}} index, '''int''' newValue<b>)</b></code>
<!-- 
SETBUILDINGPRODUCTIONTIME
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|City|SetBuildingProductionTime}}<b>(</b>{{Type5|BuildingType}} index, '''int''' newValue<b>)</b></code>
<!-- 
SETBUILDINGYIELDCHANGE
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|City|SetBuildingYieldChange}}<b>(</b>{{Type5|BuildingClassType}} buildingClass, {{Type5|YieldType}} yield, '''int''' change<b>)</b></code>
<!-- 
SETCITYSIZEBOOST
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|City|SetCitySizeBoost}}<b>(</b>'''int''' boost<b>)</b></code>
<!-- 
SETDAMAGE
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|City|SetDamage}}<b>(</b>'''int''' value<b>)</b></code>
<!-- 
SETDRAFTED
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|City|SetDrafted}}<b>(</b>'''int''' newValue<b>)</b></code>
<!-- 
SETFEATUREPRODUCTION
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|City|SetFeatureProduction}}<b>(</b>'''int''' newValue<b>)</b></code>
<!-- 
SETFOCUSTYPE
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|City|SetFocusType}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
SETFOOD
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|City|SetFood}}<b>(</b>'''int''' newValue<b>)</b></code>
<!-- 
SETGREATPEOPLEUNITPROGRESS
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|City|SetGreatPeopleUnitProgress}}<b>(</b>{{Type5|UnitType}} index, '''int''' newValue<b>)</b></code>
<!-- 
SETHIGHESTPOPULATION
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|City|SetHighestPopulation}}<b>(</b>'''int''' newValue<b>)</b></code>
<!-- 
SETJONSCULTURELEVEL
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|City|SetJONSCultureLevel}}<b>(</b>'''int''' value<b>)</b></code>
<!-- 
SETJONSCULTURESTORED
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|City|SetJONSCultureStored}}<b>(</b>'''int''' value<b>)</b></code>
<!-- 
SETNAME
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|City|SetName}}<b>(</b>'''string''' newValue, '''bool''' found<b>)</b></code>
<!-- 
SETNEVERLOST
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|City|SetNeverLost}}<b>(</b>'''int''' newValue<b>)</b></code>
<!-- 
SETNUMREALBUILDING
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|City|SetNumRealBuilding}}<b>(</b>{{Type5|BuildingType}} index, '''int''' newValue<b>)</b></code>
<!-- 
SETOCCUPIED
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|City|SetOccupied}}<b>(</b>'''bool''' value<b>)</b></code>
<!-- 
SETOVERFLOWPRODUCTION
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|City|SetOverflowProduction}}<b>(</b>'''int''' newValue<b>)</b></code>
<!-- 
SETPOPULATION
-->
|-
{{FuncInfos5|yes  |yes  |yes|<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|City|SetPopulation}}<b>(</b>'''int''' newValue, '''bool''' flag<b>)</b></code>
<!-- 
SETPRODUCTION
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|City|SetProduction}}<b>(</b>'''int''' newValue<b>)</b></code>
<!-- 
SETPRODUCTIONAUTOMATED
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|City|SetProductionAutomated}}<b>(</b>'''bool''' newValue<b>)</b></code>
<!-- 
SETPUPPET
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|City|SetPuppet}}<b>(</b>'''bool''' value<b>)</b></code>
<!-- 
SETRESOURCEDEMANDED
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|City|SetResourceDemanded}}<b>(</b>{{Type5|ResourceType}} resource<b>)</b></code>
<!-- 
SETREVEALED
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|City|SetRevealed}}<b>(</b>{{Type5|TeamID}} index, '''bool''' newValue<b>)</b></code>
<!-- 
SETUNITPRODUCTION
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|City|SetUnitProduction}}<b>(</b>'''int''' index, '''int''' newValue<b>)</b></code>
<!-- 
SETWELOVETHEKINGDAYCOUNTER
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|City|SetWeLoveTheKingDayCounter}}<b>(</b>'''int''' value<b>)</b></code>
|}

==U==
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| 
<!-- 
UPDATESTRENGTHVALUE
-->
{{FuncInfos5|no  |yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>{{UnknownSignature5}}</code>
|width="100%" |<code>{{FuncLabel5|City|UpdateStrengthValue}}<!-- No arguments --></code>
|}

==W==
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
WATERAREA
-->
|-
{{FuncInfos5|no  |yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>{{UnknownSignature5}}</code>
|width="100%" |<code>{{FuncLabel5|City|WaterArea}}<!-- No arguments --></code>
|}

=Used by=
{|cellspacing="4" cellpadding="0" width="100%" style="background-color:#F0F0F0"
<!-- 
GETCULTURETOOLTIP
-->
|-
|align="right" width="200" |<code>'''string'''</code>
|style="padding-left:6px" |<code>{{Func5|GetCultureTooltip}}<b>(</b>{{Type5|City}} city<b>)</b></code>
<!-- 
GETFAITHTOOLTIP
-->
|-
|align="right" width="200" |<code>'''string'''</code>
|style="padding-left:6px" |<code>{{Func5|GetFaithTooltip}}<b>(</b>{{Type5|City}} city<b>)</b></code>
<!-- 
GETFOODTOOLTIP
-->
|-
|align="right" width="200" |<code>'''string'''</code>
|style="padding-left:6px" |<code>{{Func5|GetFoodTooltip}}<b>(</b>{{Type5|City}} city<b>)</b></code>
<!-- 
GETGOLDTOOLTIP
-->
|-
|align="right" width="200" |<code>'''string'''</code>
|style="padding-left:6px" |<code>{{Func5|GetGoldTooltip}}<b>(</b>{{Type5|City}} city<b>)</b></code>
<!-- 
GETPRODUCTIONTOOLTIP
-->
|-
|align="right" width="200" |<code>'''string'''</code>
|style="padding-left:6px" |<code>{{Func5|GetProductionTooltip}}<b>(</b>{{Type5|City}} city<b>)</b></code>
<!-- 
GETRELIGIONTOOLTIP
-->
|-
|align="right" width="200" |<code>'''string'''</code>
|style="padding-left:6px" |<code>{{Func5|GetReligionTooltip}}<b>(</b>{{Type5|City}} city<b>)</b></code>
<!-- 
GETSCIENCETOOLTIP
-->
|-
|align="right" width="200" |<code>'''string'''</code>
|style="padding-left:6px" |<code>{{Func5|GetScienceTooltip}}<b>(</b>{{Type5|City}} city<b>)</b></code>
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
CITYPURCHASEBUILDING
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Game}}.{{Func5|Game|CityPurchaseBuilding}}<b>(</b>{{Type5|City}} city, {{Type5|UnitType}} unitType, '''int''' buildingType, {{Type5|ProjectType}} projectTypes<b>)</b></code>
<!-- 
CITYPURCHASEPROJECT
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Game}}.{{Func5|Game|CityPurchaseProject}}<b>(</b>{{Type5|City}} city, {{Type5|UnitType}} unitType, '''int''' buildingType, {{Type5|ProjectType}} projectTypes<b>)</b></code>
<!-- 
CITYPURCHASEUNIT
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Game}}.{{Func5|Game|CityPurchaseUnit}}<b>(</b>{{Type5|City}} city, {{Type5|UnitType}} unitType, '''int''' buildingType, {{Type5|ProjectType}} projectTypes<b>)</b></code>
<!-- 
CITYPUSHORDER
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Game}}.{{Func5|Game|CityPushOrder}}<b>(</b>{{Type5|City}} city, {{Type5|OrderType}} order, {{Type5|UnitType}} data, '''bool''' alt, '''bool''' shift, '''bool''' ctrl<b>)</b></code>
<!-- 
FOUNDRELIGION
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Game}}.{{Func5|Game|FoundReligion}}<b>(</b>{{Type5|PlayerID}} vaticanPlayer, {{Type5|ReligionType}} religion, '''unknown''' arg2, {{Type5|BeliefType}} belief2, {{Type5|BeliefType}} belief3, {{Type5|BeliefType}} belief3, '''int''' arg6, {{Type5|City}} vaticanCity<b>)</b></code>
<!-- 
GETHOLYCITYFORRELIGION
-->
|-
|align="right" width="200" |<code>{{Type5|City}}</code>
|style="padding-left:6px" |<code>{{Type5|Game}}.{{Func5|Game|GetHolyCityForReligion}}<b>(</b>{{Type5|ReligionType}} religion, {{Type5|PlayerID}} player<b>)</b></code>
<!-- 
SETADVISORRECOMMENDERCITY
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Game}}.{{Func5|Game|SetAdvisorRecommenderCity}}<b>(</b>{{Type5|City}} city<b>)</b></code>
<!-- 
SETHOLYCITY
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Game}}.{{Func5|Game|SetHolyCity}}<b>(</b>{{Type5|ReligionType}} arg0, {{Type5|City}} newHolyCity<b>)</b></code>
<!-- 
ACQUIRECITY
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|AcquireCity}}<b>(</b>{{Type5|City}} city, '''bool''' conquest, '''bool''' trade<b>)</b></code>
<!-- 
CANRAZE
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|CanRaze}}<b>(</b>{{Type5|City}} city, '''bool''' arg1 = nil<b>)</b></code>
<!-- 
CITIES
-->
|-
|align="right" width="200" |<code>iterator({{Type5|City}})</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|Cities}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
DISBAND
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|Disband}}<b>(</b>{{Type5|City}} city<b>)</b></code>
<!-- 
GETADVANCEDSTARTBUILDINGCOST
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|GetAdvancedStartBuildingCost}}<b>(</b>{{Type5|BuildingType}} building, '''bool''' add, {{Type5|City}} city<b>)</b></code>
<!-- 
GETADVANCEDSTARTPOPCOST
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|GetAdvancedStartPopCost}}<b>(</b>'''bool''' add, {{Type5|City}} city<b>)</b></code>
<!-- 
GETCAPITALCITY
-->
|-
|align="right" width="200" |<code>{{Type5|City}}</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|GetCapitalCity}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETCITYBYID
-->
|-
|align="right" width="200" |<code>{{Type5|City}}</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|GetCityByID}}<b>(</b>{{Type5|CityID}} city<b>)</b></code>
<!-- 
GETROUTEGOLDTIMES100
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|GetRouteGoldTimes100}}<b>(</b>{{Type5|City}} city<b>)</b></code>
<!-- 
GETUNHAPPINESSFORECAST
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|GetUnhappinessForecast}}<b>(</b>{{Type5|City}} newCity, {{Type5|City}} newCity<b>)</b></code>
<!-- 
GETUNHAPPINESSFROMCITYFORUI
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|GetUnhappinessFromCityForUI}}<b>(</b>{{Type5|City}} city<b>)</b></code>
<!-- 
INITCITY
-->
|-
|align="right" width="200" |<code>{{Type5|City}}</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|InitCity}}<b>(</b>'''int''' x, '''int''' y, '''bool''' bumpUnits = true<b>)</b></code>
<!-- 
ISCAPITALCONNECTEDTOCITY
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|IsCapitalConnectedToCity}}<b>(</b>{{Type5|City}} city<b>)</b></code>
<!-- 
RAZE
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|Raze}}<b>(</b>{{Type5|City}} city<b>)</b></code>
<!-- 
GETFEATUREPRODUCTION
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Plot}}:{{Func5|Plot|GetFeatureProduction}}<b>(</b>{{Type5|BuildActionType}} build, {{Type5|TeamID}} team, {{Type5|City}} city<b>)</b></code>
<!-- 
GETWORKINGCITY
-->
|-
|align="right" width="200" |<code>{{Type5|City}}</code>
|style="padding-left:6px" |<code>{{Type5|Plot}}:{{Func5|Plot|GetWorkingCity}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETHEADSELECTEDCITY
-->
|-
|align="right" width="200" |<code>{{Type5|City}}</code>
|style="padding-left:6px" |<code>{{Type5|UI}}.{{Func5|UI|GetHeadSelectedCity}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
SELECTCITY
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|UI}}.{{Func5|UI|SelectCity}}<b>(</b>{{Type5|City}} city<b>)</b></code>
<!-- 
GETRANGECOMBATDAMAGE
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Unit}}:{{Func5|Unit|GetRangeCombatDamage}}<b>(</b>{{Type5|Unit}} defender, {{Type5|City}} city, '''bool''' includeRand<b>)</b></code>
|}




{{Civ5 API Footer}}
[[Category:Civ5 Types|City]]