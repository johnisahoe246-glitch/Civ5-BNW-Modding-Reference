{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



=Static Methods=
Methods are functions that belong to an object. Static methods are invoked through a '''dot''', as in <code>Game.SomeMethod(&lt;args&gt;)</code>. When a dot is used the caller object is not implicitly provided as the first argument.
==A==
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
ADDPLAYER
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Game|AddPlayer}}<b>(</b>{{Type5|PlayerID}} newPlayer, {{Type5|LeaderType}} leader, {{Type5|CivilizationType}} civ<b>)</b></code>
|}

==C==
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
CALCULATEOPTIONSCHECKSUM
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Game|CalculateOptionsChecksum}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
CALCULATESYNCCHECKSUM
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Game|CalculateSyncChecksum}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
CANDOCONTROL
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Game|CanDoControl}}<b>(</b>{{Type5|ControlType}} arg0<b>)</b></code>
<!-- 
CANHANDLEACTION
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Game|CanHandleAction}}<b>(</b>{{Type5|ActionType}} action, {{Type5|Plot}} plot = nil, '''bool''' testVisible = false<b>)</b></code>
<!-- 
CANHAVESECRETARYGENERAL
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Game|CanHaveSecretaryGeneral}}<b>(</b>{{Type5|VoteSourceType}} voteSource<b>)</b></code>
<!-- 
CANTRAINNUKES
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Game|CanTrainNukes}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
CHANGEDIPLOVOTE
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Game|ChangeDiploVote}}<b>(</b>{{Type5|VoteSourceType}} voteSource, '''int''' change<b>)</b></code>
<!-- 
CHANGEMAXTURNS
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Game|ChangeMaxTurns}}<b>(</b>'''int''' change<b>)</b></code>
<!-- 
CHANGENONUKESCOUNT
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Game|ChangeNoNukesCount}}<b>(</b>'''int''' change<b>)</b></code>
<!-- 
CHANGENUKESEXPLODED
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Game|ChangeNukesExploded}}<b>(</b>'''int''' change<b>)</b></code>
<!-- 
CHANGENUMVOTESFORTEAM
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Game|ChangeNumVotesForTeam}}<b>(</b>{{Type5|TeamID}} team, '''int''' kiVaticanExtraVotes<b>)</b></code>
<!-- 
CHANGEPLOTEXTRACOST
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Game|ChangePlotExtraCost}}<b>(</b>'''int''' x, '''int''' y, '''int''' extraCost<b>)</b></code>
<!-- 
CITYPURCHASEBUILDING
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Game|CityPurchaseBuilding}}<b>(</b>{{Type5|City}} city, {{Type5|UnitType}} unitType, '''int''' buildingType, {{Type5|ProjectType}} projectTypes<b>)</b></code>
<!-- 
CITYPURCHASEPROJECT
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Game|CityPurchaseProject}}<b>(</b>{{Type5|City}} city, {{Type5|UnitType}} unitType, '''int''' buildingType, {{Type5|ProjectType}} projectTypes<b>)</b></code>
<!-- 
CITYPURCHASEUNIT
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Game|CityPurchaseUnit}}<b>(</b>{{Type5|City}} city, {{Type5|UnitType}} unitType, '''int''' buildingType, {{Type5|ProjectType}} projectTypes<b>)</b></code>
<!-- 
CITYPUSHORDER
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Game|CityPushOrder}}<b>(</b>{{Type5|City}} city, {{Type5|OrderType}} order, {{Type5|UnitType}} data, '''bool''' alt, '''bool''' shift, '''bool''' ctrl<b>)</b></code>
<!-- 
COUNTCIVPLAYERSALIVE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Game|CountCivPlayersAlive}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
COUNTCIVPLAYERSEVERALIVE
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Game|CountCivPlayersEverAlive}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
COUNTCIVTEAMSALIVE
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Game|CountCivTeamsAlive}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
COUNTCIVTEAMSEVERALIVE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Game|CountCivTeamsEverAlive}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
COUNTHUMANPLAYERSALIVE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Game|CountHumanPlayersAlive}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
COUNTHUMANPLAYERSEVERALIVE
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Game|CountHumanPlayersEverAlive}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
COUNTKNOWNTECHNUMTEAMS
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Game|CountKnownTechNumTeams}}<b>(</b>{{Type5|TechType}} tech<b>)</b></code>
<!-- 
COUNTNUMHUMANGAMETURNACTIVE
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Game|CountNumHumanGameTurnActive}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
COUNTPOSSIBLEVOTE
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Game|CountPossibleVote}}<b>(</b>{{Type5|VoteType}} vote, {{Type5|VoteSourceType}} voteSource<b>)</b></code>
<!-- 
COUNTTOTALCIVPOWER
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Game|CountTotalCivPower}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
COUNTTOTALNUKEUNITS
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Game|CountTotalNukeUnits}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
CYCLECITIES
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Game|CycleCities}}<b>(</b>'''bool''' forward, '''bool''' add<b>)</b></code>
<!-- 
CYCLEPLOTUNITS
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Game|CyclePlotUnits}}<b>(</b>{{Type5|Plot}} plot, '''bool''' forward, '''bool''' auto, '''int''' count<b>)</b></code>
<!-- 
CYCLEUNITS
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Game|CycleUnits}}<b>(</b>'''bool''' clear, '''bool''' forward, '''bool''' workers<b>)</b></code>
|}

==D==
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
DOCONTROL
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Game|DoControl}}<b>(</b>{{Type5|ControlType}} control<b>)</b></code>
<!-- 
DOFROMUIDIPLOEVENT
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Game|DoFromUIDiploEvent}}<b>(</b>{{Type5|DiploUIEventType}} event, {{Type5|PlayerID}} aIPlayer, {{Type5|SpecialistType}} button, '''int''' againstPlayer, '''int''' arg3<b>)</b></code>
<!-- 
DOMINORBULLYGOLD
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Game|DoMinorBullyGold}}<b>(</b>{{Type5|PlayerID}} activePlayer, {{Type5|PlayerID}} minorCiv<b>)</b></code>
<!-- 
DOMINORBULLYUNIT
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Game|DoMinorBullyUnit}}<b>(</b>{{Type5|PlayerID}} activePlayer, {{Type5|PlayerID}} minorCiv<b>)</b></code>
<!-- 
DOMINORBUYOUT
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Game|DoMinorBuyout}}<b>(</b>{{Type5|PlayerID}} activePlayer, {{Type5|PlayerID}} minorCiv<b>)</b></code>
<!-- 
DOMINORGIFTGOLD
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>{{UnknownSignature5}}</code>
|width="100%" |<code>{{FuncLabel5|Game|DoMinorGiftGold}}<!-- No arguments --></code>
<!-- 
DOMINORGIFTTILEIMPROVEMENT
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Game|DoMinorGiftTileImprovement}}<b>(</b>{{Type5|PlayerID}} fromPlayer, {{Type5|TaskType}} toPlayer, '''int''' plotX, '''int''' plotY<b>)</b></code>
<!-- 
DOMINORGOLDGIFT
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Game|DoMinorGoldGift}}<b>(</b>{{Type5|TeamID}} gold, '''int''' goldGiftSmall<b>)</b></code>
<!-- 
DOMINORPLEDGEPROTECTION
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Game|DoMinorPledgeProtection}}<b>(</b>{{Type5|PlayerID}} activePlayer, {{Type5|PlayerID}} minorCiv, '''bool''' arg2<b>)</b></code>
|}

==E==
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
ENHANCERELIGION
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Game|EnhanceReligion}}<b>(</b>{{Type5|PlayerID}} vaticanPlayer, {{Type5|ReligionType}} religion, {{Type5|BeliefType}} belief4, {{Type5|BeliefType}} belief5<b>)</b></code>
|}

==F==
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
FOUNDPANTHEON
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Game|FoundPantheon}}<b>(</b>'''int''' vaticanPlayer, {{Type5|BeliefType}} belief1<b>)</b></code>
<!-- 
FOUNDRELIGION
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Game|FoundReligion}}<b>(</b>{{Type5|PlayerID}} vaticanPlayer, {{Type5|ReligionType}} religion, '''unknown''' arg2, {{Type5|BeliefType}} belief2, {{Type5|BeliefType}} belief3, {{Type5|BeliefType}} belief3, '''int''' arg6, {{Type5|City}} vaticanCity<b>)</b></code>
|}

==G==
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
GAMEPLAYDIPLOMACYAILEADERMESSAGE
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>{{UnknownSignature5}}</code>
|width="100%" |<code>{{FuncLabel5|Game|GameplayDiplomacyAILeaderMessage}}<!-- No arguments --></code>
<!-- 
GETACTIVECIVILIZATIONTYPE
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>{{Type5|CivilizationType}}</code>
|width="100%" |<code>{{FuncLabel5|Game|GetActiveCivilizationType}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETACTIVEPLAYER
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>{{Type5|PlayerID}}</code>
|width="100%" |<code>{{FuncLabel5|Game|GetActivePlayer}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETACTIVETEAM
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>{{Type5|TeamID}}</code>
|width="100%" |<code>{{FuncLabel5|Game|GetActiveTeam}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETADJUSTEDLANDPERCENT
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Game|GetAdjustedLandPercent}}<b>(</b>{{Type5|VictoryType}} victory<b>)</b></code>
<!-- 
GETADJUSTEDPOPULATIONPERCENT
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Game|GetAdjustedPopulationPercent}}<b>(</b>{{Type5|VictoryType}} victory<b>)</b></code>
<!-- 
GETADVISORCOUNSEL
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''unknown'''</code>
|width="100%" |<code>{{FuncLabel5|Game|GetAdvisorCounsel}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETAIAUTOPLAY
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Game|GetAIAutoPlay}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETALLOWRCLICKMOVEMENTWHILESCROLLING
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Game|GetAllowRClickMovementWhileScrolling}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETAVAILABLEBONUSBELIEFS
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>iterator('''int''', {{Type5|BeliefType}})</code>
|width="100%" |<code>{{FuncLabel5|Game|GetAvailableBonusBeliefs}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETAVAILABLEENHANCERBELIEFS
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>iterator('''int''', {{Type5|BeliefType}})</code>
|width="100%" |<code>{{FuncLabel5|Game|GetAvailableEnhancerBeliefs}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETAVAILABLEFOLLOWERBELIEFS
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>iterator('''int''', {{Type5|BeliefType}})</code>
|width="100%" |<code>{{FuncLabel5|Game|GetAvailableFollowerBeliefs}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETAVAILABLEFOUNDERBELIEFS
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>iterator('''int''', {{Type5|BeliefType}})</code>
|width="100%" |<code>{{FuncLabel5|Game|GetAvailableFounderBeliefs}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETAVAILABLEPANTHEONBELIEFS
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>iterator('''int''', {{Type5|BeliefType}})</code>
|width="100%" |<code>{{FuncLabel5|Game|GetAvailablePantheonBeliefs}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETBELIEFSINRELIGION
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>iterator('''int''', {{Type5|BeliefType}})</code>
|width="100%" |<code>{{FuncLabel5|Game|GetBeliefsInReligion}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETBESTGREATPEOPLEPLAYER
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>{{UnknownSignature5}}</code>
|width="100%" |<code>{{FuncLabel5|Game|GetBestGreatPeoplePlayer}}<!-- No arguments --></code>
<!-- 
GETBESTLANDUNIT
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>{{Type5|UnitType}}</code>
|width="100%" |<code>{{FuncLabel5|Game|GetBestLandUnit}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETBESTLANDUNITCOMBAT
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>{{Type5|UnitType}}</code>
|width="100%" |<code>{{FuncLabel5|Game|GetBestLandUnitCombat}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETBESTPOLICIESPLAYER
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>{{UnknownSignature5}}</code>
|width="100%" |<code>{{FuncLabel5|Game|GetBestPoliciesPlayer}}<!-- No arguments --></code>
<!-- 
GETBESTWONDERSPLAYER
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>{{UnknownSignature5}}</code>
|width="100%" |<code>{{FuncLabel5|Game|GetBestWondersPlayer}}<!-- No arguments --></code>
<!-- 
GETBUILDINGCLASSCREATEDCOUNT
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Game|GetBuildingClassCreatedCount}}<b>(</b>{{Type5|BuildingClassType}} index<b>)</b></code>
<!-- 
GETBUILDINGYIELDCHANGE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Game|GetBuildingYieldChange}}<b>(</b>{{Type5|BuildingType}} building, {{Type5|YieldType}} arg1<b>)</b></code>
<!-- 
GETBUILDINGYIELDMODIFIER
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Game|GetBuildingYieldModifier}}<b>(</b>{{Type5|BuildingType}} building, {{Type5|YieldType}} arg1<b>)</b></code>
<!-- 
GETCALENDAR
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>{{Type5|CalendarType}}</code>
|width="100%" |<code>{{FuncLabel5|Game|GetCalendar}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETCOMBATPREDICTION
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>{{Type5|CombatPredictionType}}</code>
|width="100%" |<code>{{FuncLabel5|Game|GetCombatPrediction}}<b>(</b>{{Type5|Unit}} myUnit, {{Type5|Unit}} theirUnit<b>)</b></code>
<!-- 
GETCURRENTERA
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>{{Type5|EraType}}</code>
|width="100%" |<code>{{FuncLabel5|Game|GetCurrentEra}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETCUSTOMOPTION
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Game|GetCustomOption}}<b>(</b>'''string''' optionName<b>)</b></code>
<!-- 
GETDEALDURATION
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>{{Type5|ResourceType}}</code>
|width="100%" |<code>{{FuncLabel5|Game|GetDealDuration}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETDIPLORESPONSE
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''string'''</code>
|width="100%" |<code>{{FuncLabel5|Game|GetDiploResponse}}<b>(</b>'''unknown''' leaderType, {{Type5|DiploResponseType}} responseType<b>)</b></code>
<!-- 
GETELAPSEDGAMETURNS
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Game|GetElapsedGameTurns}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETESTIMATEENDTURN
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Game|GetEstimateEndTurn}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETFAITHCOST
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Game|GetFaithCost}}<b>(</b>{{Type5|UnitType}} unit<b>)</b></code>
<!-- 
GETFOUNDER
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>{{Type5|PlayerID}}</code>
|width="100%" |<code>{{FuncLabel5|Game|GetFounder}}<b>(</b>{{Type5|ReligionType}} arg0, '''int''' arg1<b>)</b></code>
<!-- 
GETFOUNDERBENEFITSRELIGION
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>{{Type5|ReligionType}}</code>
|width="100%" |<code>{{FuncLabel5|Game|GetFounderBenefitsReligion}}<b>(</b>{{Type5|PlayerID}} player<b>)</b></code>
<!-- 
GETGAMESPEEDTYPE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>{{Type5|GameSpeedType}}</code>
|width="100%" |<code>{{FuncLabel5|Game|GetGameSpeedType}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETGAMESTATE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>{{Type5|GameplayStateType}}</code>
|width="100%" |<code>{{FuncLabel5|Game|GetGameState}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETGAMETURN
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>{{Type5|PlayerID}}</code>
|width="100%" |<code>{{FuncLabel5|Game|GetGameTurn}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETGAMETURNYEAR
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Game|GetGameTurnYear}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETHANDICAPTYPE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>{{Type5|HandicapType}}</code>
|width="100%" |<code>{{FuncLabel5|Game|GetHandicapType}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETHOLYCITYFORRELIGION
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>{{Type5|City}}</code>
|width="100%" |<code>{{FuncLabel5|Game|GetHolyCityForReligion}}<b>(</b>{{Type5|ReligionType}} religion, {{Type5|PlayerID}} player<b>)</b></code>
<!-- 
GETIMPROVEMENTUPGRADETIME
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Game|GetImprovementUpgradeTime}}<b>(</b>{{Type5|ImprovementType}} improvement, {{Type5|Plot}} plot<b>)</b></code>
<!-- 
GETINITLAND
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Game|GetInitLand}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETINITPOPULATION
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Game|GetInitPopulation}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETINITTECH
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Game|GetInitTech}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETINITWONDERS
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Game|GetInitWonders}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETMAXCITYELIMINATION
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Game|GetMaxCityElimination}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETMAXLAND
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Game|GetMaxLand}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETMAXPOPULATION
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Game|GetMaxPopulation}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETMAXTECH
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Game|GetMaxTech}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETMAXTURNS
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Game|GetMaxTurns}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETMAXWONDERS
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Game|GetMaxWonders}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETMINIMUMFAITHNEXTPANTHEON
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Game|GetMinimumFaithNextPantheon}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETMINUTESPLAYED
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Game|GetMinutesPlayed}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETNAME
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''string'''</code>
|width="100%" |<code>{{FuncLabel5|Game|GetName}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETNONUKESCOUNT
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>{{Type5|PlayerID}}</code>
|width="100%" |<code>{{FuncLabel5|Game|GetNoNukesCount}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETNUKESEXPLODED
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Game|GetNukesExploded}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETNUMADVANCEDSTARTPOINTS
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Game|GetNumAdvancedStartPoints}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETNUMCITIES
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Game|GetNumCities}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETNUMCITIESFOLLOWING
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Game|GetNumCitiesFollowing}}<b>(</b>{{Type5|ReligionType}} religion<b>)</b></code>
<!-- 
GETNUMCITIESPOLICYCOSTMOD
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Game|GetNumCitiesPolicyCostMod}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETNUMCIVCITIES
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Game|GetNumCivCities}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETNUMFOLLOWERS
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>{{UnknownSignature5}}</code>
|width="100%" |<code>{{FuncLabel5|Game|GetNumFollowers}}<!-- No arguments --></code>
<!-- 
GETNUMGAMETURNACTIVE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Game|GetNumGameTurnActive}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETNUMHUMANPLAYERS
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Game|GetNumHumanPlayers}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETNUMRELIGIONSFOUNDED
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Game|GetNumReligionsFounded}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETNUMRELIGIONSSTILLTOFOUND
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Game|GetNumReligionsStillToFound}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETNUMREPLAYMESSAGES
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Game|GetNumReplayMessages}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETNUMRESOURCEREQUIREDFORBUILDING
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Game|GetNumResourceRequiredForBuilding}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETNUMRESOURCEREQUIREDFORUNIT
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Game|GetNumResourceRequiredForUnit}}<b>(</b>{{Type5|UnitType}} unit, {{Type5|ResourceType}} resource<b>)</b></code>
<!-- 
GETNUMVICTORYVOTESTALLIED
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Game|GetNumVictoryVotesTallied}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETNUMVOTESFORTEAM
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Game|GetNumVotesForTeam}}<b>(</b>{{Type5|TeamID}} teamLoop<b>)</b></code>
<!-- 
GETNUMWORLDWONDERS
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Game|GetNumWorldWonders}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETPAUSEPLAYER
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Game|GetPausePlayer}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETPITBOSSTURNTIME
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Game|GetPitbossTurnTime}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETPLAYERRANK
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Game|GetPlayerRank}}<b>(</b>{{Type5|PlayerID}} index<b>)</b></code>
<!-- 
GETPLAYERSCORE
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Game|GetPlayerScore}}<b>(</b>{{Type5|PlayerID}} index<b>)</b></code>
<!-- 
GETPLAYERVOTE
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Game|GetPlayerVote}}<b>(</b>{{Type5|PlayerID}} ownerIndex, '''int''' voteId<b>)</b></code>
<!-- 
GETPREVIOUSVOTECAST
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Game|GetPreviousVoteCast}}<b>(</b>{{Type5|TeamID}} teamLoop<b>)</b></code>
<!-- 
GETPRODUCTIONPERPOPULATION
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Game|GetProductionPerPopulation}}<b>(</b>{{Type5|HurryType}} hurry<b>)</b></code>
<!-- 
GETPROJECTCREATEDCOUNT
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Game|GetProjectCreatedCount}}<b>(</b>{{Type5|ProjectType}} index<b>)</b></code>
<!-- 
GETRANKPLAYER
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>{{Type5|PlayerID}}</code>
|width="100%" |<code>{{FuncLabel5|Game|GetRankPlayer}}<b>(</b>'''int''' rank<b>)</b></code>
<!-- 
GETRANKTEAM
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>{{Type5|TeamID}}</code>
|width="100%" |<code>{{FuncLabel5|Game|GetRankTeam}}<b>(</b>'''int''' rank<b>)</b></code>
<!-- 
GETRELIGIONNAME
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''string'''</code>
|width="100%" |<code>{{FuncLabel5|Game|GetReligionName}}<b>(</b>{{Type5|ReligionType}} religion<b>)</b></code>
<!-- 
GETREPLAYINFO
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''unknown'''</code>
|width="100%" |<code>{{FuncLabel5|Game|GetReplayInfo}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETREPLAYMESSAGE
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>{{UnknownSignature5}}</code>
|width="100%" |<code>{{FuncLabel5|Game|GetReplayMessage}}<!-- No arguments --></code>
<!-- 
GETREPLAYMESSAGES
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>table('''int''' => {{Type5|IntrigueInfo}})</code>
|width="100%" |<code>{{FuncLabel5|Game|GetReplayMessages}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETRESEARCHAGREEMENTCOST
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Game|GetResearchAgreementCost}}<b>(</b>{{Type5|PlayerID}} us, {{Type5|PlayerID}} them<b>)</b></code>
<!-- 
GETRESOURCEUSAGETYPE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>{{Type5|ResourceUsageType}}</code>
|width="100%" |<code>{{FuncLabel5|Game|GetResourceUsageType}}<b>(</b>{{Type5|ResourceType}} resourceLoop<b>)</b></code>
<!-- 
GETSECRETARYGENERAL
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Game|GetSecretaryGeneral}}<b>(</b>{{Type5|VoteSourceType}} voteSource<b>)</b></code>
<!-- 
GETSECRETARYGENERALTIMER
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Game|GetSecretaryGeneralTimer}}<b>(</b>'''int''' voteSource<b>)</b></code>
<!-- 
GETSTARTERA
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>{{Type5|EraType}}</code>
|width="100%" |<code>{{FuncLabel5|Game|GetStartEra}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETSTARTTURN
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>{{Type5|PlayerID}}</code>
|width="100%" |<code>{{FuncLabel5|Game|GetStartTurn}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETSTARTYEAR
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Game|GetStartYear}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETTARGETSCORE
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Game|GetTargetScore}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETTEAMRANK
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Game|GetTeamRank}}<b>(</b>{{Type5|TeamID}} index<b>)</b></code>
<!-- 
GETTEAMSCORE
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Game|GetTeamScore}}<b>(</b>{{Type5|TeamID}} index<b>)</b></code>
<!-- 
GETTIMESTRING
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''string'''</code>
|width="100%" |<code>{{FuncLabel5|Game|GetTimeString}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETTOTALPOPULATION
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Game|GetTotalPopulation}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETTURNSBETWEENMINORCIVELECTIONS
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''unknown'''</code>
|width="100%" |<code>{{FuncLabel5|Game|GetTurnsBetweenMinorCivElections}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETTURNSLICE
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Game|GetTurnSlice}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETTURNSUNTILMINORCIVELECTION
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''unknown'''</code>
|width="100%" |<code>{{FuncLabel5|Game|GetTurnsUntilMinorCivElection}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETTURNYEAR
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Game|GetTurnYear}}<b>(</b>'''int''' gameTurn<b>)</b></code>
<!-- 
GETTUTORIALLEVEL
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Game|GetTutorialLevel}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETUNITCLASSCREATEDCOUNT
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Game|GetUnitClassCreatedCount}}<b>(</b>{{Type5|UnitClassType}} index<b>)</b></code>
<!-- 
GETUNITCREATEDCOUNT
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Game|GetUnitCreatedCount}}<b>(</b>{{Type5|UnitType}} index<b>)</b></code>
<!-- 
GETUNITEDNATIONSCOUNTDOWN
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Game|GetUnitedNationsCountdown}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETUNITUPGRADESTO
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>{{Type5|UnitType}}</code>
|width="100%" |<code>{{FuncLabel5|Game|GetUnitUpgradesTo}}<b>(</b>{{Type5|UnitType}} unit<b>)</b></code>
<!-- 
GETVARIABLECITYSIZEFROMPOPULATION
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Game|GetVariableCitySizeFromPopulation}}<b>(</b>'''int''' population<b>)</b></code>
<!-- 
GETVICTORY
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>{{Type5|VictoryType}}</code>
|width="100%" |<code>{{FuncLabel5|Game|GetVictory}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETVOTECAST
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>{{Type5|TeamID}}</code>
|width="100%" |<code>{{FuncLabel5|Game|GetVoteCast}}<b>(</b>{{Type5|TeamID}} team<b>)</b></code>
<!-- 
GETVOTEOUTCOME
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Game|GetVoteOutcome}}<b>(</b>{{Type5|VoteType}} index<b>)</b></code>
<!-- 
GETVOTEREQUIRED
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Game|GetVoteRequired}}<b>(</b>{{Type5|VoteType}} vote, {{Type5|VoteSourceType}} voteSource<b>)</b></code>
<!-- 
GETVOTESNEEDEDFORDIPLOVICTORY
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Game|GetVotesNeededForDiploVictory}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETVOTETIMER
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Game|GetVoteTimer}}<b>(</b>'''int''' voteSource<b>)</b></code>
<!-- 
GETWINNER
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>{{Type5|TeamID}}</code>
|width="100%" |<code>{{FuncLabel5|Game|GetWinner}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETWINNINGTURN
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Game|GetWinningTurn}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETWORLDNUMCITIESUNHAPPINESSPERCENT
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Game|GetWorldNumCitiesUnhappinessPercent}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GOLDENAGELENGTH
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Game|GoldenAgeLength}}<b>(</b><!-- No arguments --><b>)</b></code>
|}

==H==
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
HANDLEACTION
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Game|HandleAction}}<b>(</b>{{Type5|PolicyType}} action<b>)</b></code>
<!-- 
HASADVISORMESSAGEBEENSEEN
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Game|HasAdvisorMessageBeenSeen}}<b>(</b>'''string''' tutorialID<b>)</b></code>
|}

==I==
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
ISBUILDINGCLASSMAXEDOUT
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Game|IsBuildingClassMaxedOut}}<b>(</b>{{Type5|BuildingClassType}} index, '''int''' extra<b>)</b></code>
<!-- 
ISBUILDINGEVERACTIVE
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Game|IsBuildingEverActive}}<b>(</b>{{Type5|BuildingType}} building<b>)</b></code>
<!-- 
ISBUILDINGRECOMMENDED
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Game|IsBuildingRecommended}}<b>(</b>'''int''' building, {{Type5|AdvisorType}} advisorLoop<b>)</b></code>
<!-- 
ISCHOOSEELECTION
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Game|IsChooseElection}}<b>(</b>{{Type5|VoteType}} vote<b>)</b></code>
<!-- 
ISCIRCUMNAVIGATED
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Game|IsCircumnavigated}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ISCIVEVERACTIVE
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Game|IsCivEverActive}}<b>(</b>{{Type5|CivilizationType}} civilization<b>)</b></code>
<!-- 
ISCOMBATWARNED
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Game|IsCombatWarned}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ISDEBUGMODE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Game|IsDebugMode}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ISDIPLOVOTE
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Game|IsDiploVote}}<b>(</b>{{Type5|VoteSourceType}} voteSource<b>)</b></code>
<!-- 
ISEVERATTACKEDTUTORIAL
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Game|IsEverAttackedTutorial}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ISEVERRIGHTCLICKMOVED
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Game|IsEverRightClickMoved}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ISFINALINITIALIZED
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Game|IsFinalInitialized}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ISGAMEMULTIPLAYER
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Game|IsGameMultiPlayer}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ISHOTSEAT
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Game|IsHotSeat}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ISINADVANCEDSTART
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Game|IsInAdvancedStart}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ISLEADEREVERACTIVE
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Game|IsLeaderEverActive}}<b>(</b>{{Type5|LeaderType}} leader<b>)</b></code>
<!-- 
ISMPOPTION
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Game|IsMPOption}}<b>(</b>{{Type5|MultiOptionType}} index<b>)</b></code>
<!-- 
ISNETWORKMULTIPLAYER
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Game|IsNetworkMultiPlayer}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ISNONUKES
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Game|IsNoNukes}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ISNUKESVALID
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Game|IsNukesValid}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ISOPTION
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Game|IsOption}}<b>(</b>'''string''' index<b>)</b></code>
<!-- 
ISPAUSED
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Game|IsPaused}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ISPBEM
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Game|IsPbem}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ISPITBOSS
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Game|IsPitboss}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ISPROCESSINGMESSAGES
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Game|IsProcessingMessages}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ISPROJECTMAXEDOUT
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Game|IsProjectMaxedOut}}<b>(</b>{{Type5|ProjectType}} index, '''int''' extra<b>)</b></code>
<!-- 
ISPROJECTRECOMMENDED
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Game|IsProjectRecommended}}<b>(</b>'''int''' project, {{Type5|AdvisorType}} advisorLoop<b>)</b></code>
<!-- 
ISSCOREDIRTY
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Game|IsScoreDirty}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ISSIMULTANEOUSTEAMTURNS
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Game|IsSimultaneousTeamTurns}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ISSPECIALUNITVALID
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Game|IsSpecialUnitValid}}<b>(</b>{{Type5|SpecialUnitType}} specialUnitType<b>)</b></code>
<!-- 
ISSTATICTUTORIALACTIVE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Game|IsStaticTutorialActive}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ISTEAMGAME
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Game|IsTeamGame}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ISTEAMVOTE
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Game|IsTeamVote}}<b>(</b>{{Type5|VoteType}} vote<b>)</b></code>
<!-- 
ISTEAMVOTEELIGIBLE
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Game|IsTeamVoteEligible}}<b>(</b>{{Type5|TeamID}} team, {{Type5|VoteSourceType}} voteSource<b>)</b></code>
<!-- 
ISTECHRECOMMENDED
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Game|IsTechRecommended}}<b>(</b>{{Type5|TechType}} arg0, {{Type5|AdvisorType}} advisorLoop<b>)</b></code>
<!-- 
ISTUTORIALDEBUGGING
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Game|IsTutorialDebugging}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ISTUTORIALLOGGING
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Game|IsTutorialLogging}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ISUNITCLASSMAXEDOUT
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Game|IsUnitClassMaxedOut}}<b>(</b>{{Type5|UnitClassType}} index, '''int''' extra<b>)</b></code>
<!-- 
ISUNITEVERACTIVE
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Game|IsUnitEverActive}}<b>(</b>{{Type5|UnitType}} unit<b>)</b></code>
<!-- 
ISUNITRECOMMENDED
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Game|IsUnitRecommended}}<b>(</b>'''int''' unit, {{Type5|AdvisorType}} advisorLoop<b>)</b></code>
<!-- 
ISVICTORYVALID
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Game|IsVictoryValid}}<b>(</b>{{Type5|VictoryType}} index<b>)</b></code>
<!-- 
ISVOTEPASSED
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Game|IsVotePassed}}<b>(</b>{{Type5|VoteType}} index<b>)</b></code>
|}

==M==
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
MAKECIRCUMNAVIGATED
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>{{UnknownSignature5}}</code>
|width="100%" |<code>{{FuncLabel5|Game|MakeCircumnavigated}}<!-- No arguments --></code>
<!-- 
MAKENUKESVALID
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Game|MakeNukesValid}}<b>(</b>'''bool''' valid<b>)</b></code>
<!-- 
MAKESPECIALUNITVALID
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Game|MakeSpecialUnitValid}}<b>(</b>{{Type5|SpecialUnitType}} specialUnitType<b>)</b></code>
|}

==R==
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
RAND
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Game|Rand}}<b>(</b>'''int''' max_num, '''string''' log<b>)</b></code>
<!-- 
REVIVEACTIVEPLAYER
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>{{UnknownSignature5}}</code>
|width="100%" |<code>{{FuncLabel5|Game|ReviveActivePlayer}}<!-- No arguments --></code>
|}

==S==
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
SAVEREPLAY
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Game|SaveReplay}}<b>(</b>{{Type5|PlayerID}} player<b>)</b></code>
<!-- 
SELECTEDCITIESGAMENETMESSAGE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Game|SelectedCitiesGameNetMessage}}<b>(</b>{{Type5|GameMessageType}} message, {{Type5|TaskType}} data2, '''int''' data3, {{Type5|BuildingType}} data4, '''bool''' option, '''bool''' alt, '''bool''' shift, '''bool''' ctrl<b>)</b></code>
<!-- 
SELECTIONLISTGAMENETMESSAGE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Game|SelectionListGameNetMessage}}<b>(</b>{{Type5|GameMessageType}} message, '''int''' data2 = -1, {{Type5|BuildActionType}} data3 = -1, {{Type5|UnitID}} data4 = -1, '''int''' flags = 0, '''bool''' alt = false, '''bool''' shift = false<b>)</b></code>
<!-- 
SELECTIONLISTMOVE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Game|SelectionListMove}}<b>(</b>{{Type5|Plot}} plot, '''int''' alt, '''bool''' shift, '''int''' ctrl<b>)</b></code>
<!-- 
SETACTIVEPLAYER
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Game|SetActivePlayer}}<b>(</b>{{Type5|PlayerID}} newValue, '''bool''' forceHotSeat<b>)</b></code>
<!-- 
SETADVISORBADATTACKINTERRUPT
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Game|SetAdvisorBadAttackInterrupt}}<b>(</b>'''bool''' arg0<b>)</b></code>
<!-- 
SETADVISORCITYATTACKINTERRUPT
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Game|SetAdvisorCityAttackInterrupt}}<b>(</b>'''bool''' arg0<b>)</b></code>
<!-- 
SETADVISORMESSAGEHASBEENSEEN
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Game|SetAdvisorMessageHasBeenSeen}}<b>(</b>'''unknown''' arg0, '''bool''' arg1<b>)</b></code>
<!-- 
SETADVISORRECOMMENDERCITY
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Game|SetAdvisorRecommenderCity}}<b>(</b>{{Type5|City}} city<b>)</b></code>
<!-- 
SETADVISORRECOMMENDERTECH
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Game|SetAdvisorRecommenderTech}}<b>(</b>{{Type5|PlayerID}} player<b>)</b></code>
<!-- 
SETAIAUTOPLAY
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Game|SetAIAutoPlay}}<b>(</b>'''int''' newValue<b>)</b></code>
<!-- 
SETCOMBATWARNED
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Game|SetCombatWarned}}<b>(</b>'''bool''' arg0<b>)</b></code>
<!-- 
SETDEBUGMODE
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Game|SetDebugMode}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
SETESTIMATEENDTURN
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Game|SetEstimateEndTurn}}<b>(</b>'''int''' newValue<b>)</b></code>
<!-- 
SETEVERRIGHTCLICKMOVED
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Game|SetEverRightClickMoved}}<b>(</b>'''bool''' arg0<b>)</b></code>
<!-- 
SETFOUNDER
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Game|SetFounder}}<b>(</b>{{Type5|ReligionType}} arg0, {{Type5|PlayerID}} newOwner<b>)</b></code>
<!-- 
SETGAMESTATE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Game|SetGameState}}<b>(</b>{{Type5|GameplayStateType}} arg0<b>)</b></code>
<!-- 
SETGAMETURN
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Game|SetGameTurn}}<b>(</b>'''int''' newValue<b>)</b></code>
<!-- 
SETHOLYCITY
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Game|SetHolyCity}}<b>(</b>{{Type5|ReligionType}} arg0, {{Type5|City}} newHolyCity<b>)</b></code>
<!-- 
SETMAXCITYELIMINATION
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Game|SetMaxCityElimination}}<b>(</b>'''int''' newValue<b>)</b></code>
<!-- 
SETMAXTURNS
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Game|SetMaxTurns}}<b>(</b>'''int''' newValue<b>)</b></code>
<!-- 
SETMINIMUMFAITHNEXTPANTHEON
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>{{UnknownSignature5}}</code>
|width="100%" |<code>{{FuncLabel5|Game|SetMinimumFaithNextPantheon}}<!-- No arguments --></code>
<!-- 
SETNAME
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Game|SetName}}<b>(</b>'''string''' name<b>)</b></code>
<!-- 
SETNUMADVANCEDSTARTPOINTS
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Game|SetNumAdvancedStartPoints}}<b>(</b>'''int''' newValue<b>)</b></code>
<!-- 
SETNUMVOTESFORTEAM
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>{{UnknownSignature5}}</code>
|width="100%" |<code>{{FuncLabel5|Game|SetNumVotesForTeam}}<!-- No arguments --></code>
<!-- 
SETOPTION
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Game|SetOption}}<b>(</b>{{Type5|GameOptionType}} index, '''bool''' enabled<b>)</b></code>
<!-- 
SETPAUSEPLAYER
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Game|SetPausePlayer}}<b>(</b>{{Type5|PlayerID}} arg0<b>)</b></code>
<!-- 
SETPITBOSSTURNTIME
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Game|SetPitbossTurnTime}}<b>(</b>'''int''' hours<b>)</b></code>
<!-- 
SETPLOTEXTRAYIELD
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Game|SetPlotExtraYield}}<b>(</b>'''int''' x, '''int''' y, {{Type5|YieldType}} yield, '''int''' extraYield<b>)</b></code>
<!-- 
SETSCOREDIRTY
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Game|SetScoreDirty}}<b>(</b>'''bool''' newValue<b>)</b></code>
<!-- 
SETSTARTYEAR
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Game|SetStartYear}}<b>(</b>'''int''' newValue<b>)</b></code>
<!-- 
SETSTATICTUTORIALACTIVE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Game|SetStaticTutorialActive}}<b>(</b>'''bool''' arg0<b>)</b></code>
<!-- 
SETTARGETSCORE
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Game|SetTargetScore}}<b>(</b>'''int''' newValue<b>)</b></code>
<!-- 
SETUNITEDNATIONSCOUNTDOWN
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Game|SetUnitedNationsCountdown}}<b>(</b>'''int''' arg0<b>)</b></code>
<!-- 
SETVICTORYVALID
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Game|SetVictoryValid}}<b>(</b>{{Type5|VictoryType}} arg0, '''bool''' arg1<b>)</b></code>
<!-- 
SETWINNER
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Game|SetWinner}}<b>(</b>{{Type5|TeamID}} newWinner, {{Type5|VictoryType}} newVictory<b>)</b></code>
|}

==T==
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
TOGGLEDEBUGMODE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Game|ToggleDebugMode}}<b>(</b><!-- No arguments --><b>)</b></code>
|}

==U==
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
UPDATEFOW
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Game|UpdateFOW}}<b>(</b>'''bool''' arg0<b>)</b></code>
<!-- 
UPDATESCORE
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Game|UpdateScore}}<b>(</b>'''bool''' force<b>)</b></code>
|}

==V==
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
VICTORYDELAY
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Game|VictoryDelay}}<b>(</b>{{Type5|VictoryType}} victory<b>)</b></code>
|}




{{Civ5 API Footer}}
[[Category:Civ5 Types|Game]]