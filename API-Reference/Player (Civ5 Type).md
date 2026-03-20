{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



=Instance Methods=
Methods are functions that belong to an object. Instance methods are invoked through a '''colon''', as in <code>caller:SomeMethod(&lt;args&gt;)</code>, where ''caller'' is an instance of Player.<br/>
A colon implictly passes the caller object as the first argument. That is, the former call is equivalent to this one: <code>caller.SomeMethod(caller, &lt;args&gt;)</code>
==A==
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
ACQUIRECITY
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Player|AcquireCity}}<b>(</b>{{Type5|City}} city, '''bool''' conquest, '''bool''' trade<b>)</b></code>
<!-- 
ADDCITYNAME
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Player|AddCityName}}<b>(</b>'''string''' name<b>)</b></code>
<!-- 
ADDFREEUNIT
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Player|AddFreeUnit}}<b>(</b>{{Type5|UnitType}} arg0, {{Type5|UnitAIType}} UNITAI_DEFENSE<b>)</b></code>
<!-- 
ADDMINORCIVQUESTIFABLE
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>{{UnknownSignature5}}</code>
|width="100%" |<code>{{FuncLabel5|Player|AddMinorCivQuestIfAble}}<!-- No arguments --></code>
<!-- 
ADDNOTIFICATION
-->
|-
{{FuncInfos5|yes  |yes  |yes|Triggers a notification for a Player. Notifications appear as icons on the right side of the screen.}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Player|AddNotification}}<b>(</b>{{Type5|NotificationType}} notificationType, '''string''' description, '''string''' title, '''int''' x = -1, '''int''' y = -1, {{Type5|PlayerID}} extra1 = -1, '''int''' extra2 = -1<b>)</b></code>
<!-- 
ADDTEMPORARYDOMINANCEZONE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Player|AddTemporaryDominanceZone}}<b>(</b>'''int''' arg0, '''int''' arg1<b>)</b></code>
<!-- 
AI_FOUNDVALUE
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|AI_foundValue}}<b>(</b>'''int''' x, '''int''' y, '''int''' alwaysOne, '''bool''' alwaysFalse<b>)</b></code>
<!-- 
AI_UPDATEFOUNDVALUES
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Player|AI_updateFoundValues}}<b>(</b>'''bool''' startingLoc<b>)</b></code>
|}

==C==
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
CALCULATEGOLDRATE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|CalculateGoldRate}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
CALCULATEGOLDRATETIMES100
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|CalculateGoldRateTimes100}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
CALCULATEGROSSGOLD
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|CalculateGrossGold}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
CALCULATEGROSSGOLDTIMES100
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|CalculateGrossGoldTimes100}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
CALCULATEINFLATEDCOSTS
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|CalculateInflatedCosts}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
CALCULATERESEARCHMODIFIER
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|CalculateResearchModifier}}<b>(</b>{{Type5|TechType}} tech<b>)</b></code>
<!-- 
CALCULATETOTALYIELD
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|CalculateTotalYield}}<b>(</b>{{Type5|YieldType}} yield<b>)</b></code>
<!-- 
CALCULATEUNITCOST
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|CalculateUnitCost}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
CALCULATEUNITSUPPLY
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|CalculateUnitSupply}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
CANADOPTPOLICY
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|CanAdoptPolicy}}<b>(</b>{{Type5|PolicyType}} policy<b>)</b></code>
<!-- 
CANBUILD
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Player|CanBuild}}<b>(</b>{{Type5|Plot}} plot, {{Type5|BuildActionType}} build, '''bool''' testEra = false, '''bool''' testVisible = false, '''bool''' testGold = false<b>)</b></code>
<!-- 
CANCONSTRUCT
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Player|CanConstruct}}<b>(</b>{{Type5|BuildingType}} building, '''bool''' continue, '''bool''' testVisible, '''bool''' ignoreCost<b>)</b></code>
<!-- 
CANCONTACT
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Player|CanContact}}<b>(</b>{{Type5|PlayerID}} player<b>)</b></code>
<!-- 
CANCREATE
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Player|CanCreate}}<b>(</b>{{Type5|ProjectType}} project, '''bool''' continue, '''bool''' testVisible<b>)</b></code>
<!-- 
CANCREATEPANTHEON
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Player|CanCreatePantheon}}<b>(</b>'''bool''' arg0<b>)</b></code>
<!-- 
CANEVERRESEARCH
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Player|CanEverResearch}}<b>(</b>{{Type5|TechType}} tech<b>)</b></code>
<!-- 
CANFOUND
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Player|CanFound}}<b>(</b>'''int''' x, '''int''' y<b>)</b></code>
<!-- 
CANMAINTAIN
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Player|CanMaintain}}<b>(</b>{{Type5|ProcessType}} process, '''bool''' continue<b>)</b></code>
<!-- 
CANMAJORBULLYGOLD
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Player|CanMajorBullyGold}}<b>(</b>{{Type5|PlayerID}} major<b>)</b></code>
<!-- 
CANMAJORBULLYUNIT
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Player|CanMajorBullyUnit}}<b>(</b>{{Type5|PlayerID}} activePlayer<b>)</b></code>
<!-- 
CANMAJORBUYOUT
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|CanMajorBuyout}}<b>(</b>{{Type5|PlayerID}} activePlayer<b>)</b></code>
<!-- 
CANMAJORGIFTTILEIMPROVEMENT
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Player|CanMajorGiftTileImprovement}}<b>(</b>{{Type5|PlayerID}} activePlayer<b>)</b></code>
<!-- 
CANMAJORGIFTTILEIMPROVEMENTATPLOT
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Player|CanMajorGiftTileImprovementAtPlot}}<b>(</b>{{Type5|PlayerID}} fromPlayer, '''int''' plotX, '''int''' plotY<b>)</b></code>
<!-- 
CANMAJORPROTECT
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>{{UnknownSignature5}}</code>
|width="100%" |<code>{{FuncLabel5|Player|CanMajorProtect}}<!-- No arguments --></code>
<!-- 
CANMAJORSTARTPROTECTION
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Player|CanMajorStartProtection}}<b>(</b>{{Type5|PlayerID}} activePlayer<b>)</b></code>
<!-- 
CANMAJORWITHDRAWPROTECTION
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Player|CanMajorWithdrawProtection}}<b>(</b>{{Type5|PlayerID}} activePlayer<b>)</b></code>
<!-- 
CANPREPARE
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Player|CanPrepare}}<b>(</b>{{Type5|SpecialistType}} specialist, '''bool''' continue<b>)</b></code>
<!-- 
CANRAZE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Player|CanRaze}}<b>(</b>{{Type5|City}} city, '''bool''' arg1 = nil<b>)</b></code>
<!-- 
CANRECEIVEGOODY
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Player|CanReceiveGoody}}<b>(</b>{{Type5|Plot}} plot, {{Type5|GoodyType}} goody, {{Type5|Unit}} unit<b>)</b></code>
<!-- 
CANRESEARCH
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|CanResearch}}<b>(</b>{{Type5|TechType}} tech, '''bool''' trade = false<b>)</b></code>
<!-- 
CANRESEARCHFORFREE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Player|CanResearchForFree}}<b>(</b>{{Type5|TechType}} tech<b>)</b></code>
<!-- 
CANSPYSTAGECOUP
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Player|CanSpyStageCoup}}<b>(</b>'''unknown''' arg0<b>)</b></code>
<!-- 
CANSTOPTRADINGWITHTEAM
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Player|CanStopTradingWithTeam}}<b>(</b>{{Type5|TeamID}} team<b>)</b></code>
<!-- 
CANTRADEWITH
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Player|CanTradeWith}}<b>(</b>{{Type5|PlayerID}} whoTo<b>)</b></code>
<!-- 
CANTRAIN
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|CanTrain}}<b>(</b>{{Type5|UnitType}} unit, '''bool''' continue, '''bool''' testVisible, '''bool''' arg3, '''bool''' arg4<b>)</b></code>
<!-- 
CANUNLOCKPOLICYBRANCH
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|CanUnlockPolicyBranch}}<b>(</b>'''int''' policyBranch<b>)</b></code>
<!-- 
CHANGEADVANCEDSTARTPOINTS
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Player|ChangeAdvancedStartPoints}}<b>(</b>'''int''' change<b>)</b></code>
<!-- 
CHANGEALWAYSSEEBARBCAMPSCOUNT
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>{{UnknownSignature5}}</code>
|width="100%" |<code>{{FuncLabel5|Player|ChangeAlwaysSeeBarbCampsCount}}<!-- No arguments --></code>
<!-- 
CHANGEANARCHYNUMTURNS
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|ChangeAnarchyNumTurns}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
CHANGEBARBARIANCOMBATBONUS
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>{{UnknownSignature5}}</code>
|width="100%" |<code>{{FuncLabel5|Player|ChangeBarbarianCombatBonus}}<!-- No arguments --></code>
<!-- 
CHANGEBASEBUILDINGGOLDMAINTENANCE
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|ChangeBaseBuildingGoldMaintenance}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
CHANGECOMBATEXPERIENCE
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Player|ChangeCombatExperience}}<b>(</b>'''int''' change<b>)</b></code>
<!-- 
CHANGECONSCRIPTCOUNT
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Player|ChangeConscriptCount}}<b>(</b>'''int''' change<b>)</b></code>
<!-- 
CHANGEEXTRAHAPPINESSPERCITY
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Player|ChangeExtraHappinessPerCity}}<b>(</b>'''int''' change<b>)</b></code>
<!-- 
CHANGEFAITH
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>{{UnknownSignature5}}</code>
|width="100%" |<code>{{FuncLabel5|Player|ChangeFaith}}<!-- No arguments --></code>
<!-- 
CHANGEFREEPROMOTIONCOUNT
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>{{UnknownSignature5}}</code>
|width="100%" |<code>{{FuncLabel5|Player|ChangeFreePromotionCount}}<!-- No arguments --></code>
<!-- 
CHANGEGARRISONEDCITYRANGESTRIKEMODIFIER
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>{{UnknownSignature5}}</code>
|width="100%" |<code>{{FuncLabel5|Player|ChangeGarrisonedCityRangeStrikeModifier}}<!-- No arguments --></code>
<!-- 
CHANGEGOLD
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Player|ChangeGold}}<b>(</b>'''int''' change<b>)</b></code>
<!-- 
CHANGEGOLDENAGEPROGRESSMETER
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>{{UnknownSignature5}}</code>
|width="100%" |<code>{{FuncLabel5|Player|ChangeGoldenAgeProgressMeter}}<!-- No arguments --></code>
<!-- 
CHANGEGOLDENAGETURNS
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Player|ChangeGoldenAgeTurns}}<b>(</b>'''int''' change<b>)</b></code>
<!-- 
CHANGEGOLDPERUNITTIMES100
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>{{UnknownSignature5}}</code>
|width="100%" |<code>{{FuncLabel5|Player|ChangeGoldPerUnitTimes100}}<!-- No arguments --></code>
<!-- 
CHANGEHAPPINESSPERGARRISONEDUNIT
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Player|ChangeHappinessPerGarrisonedUnit}}<b>(</b>'''int''' change<b>)</b></code>
<!-- 
CHANGEHAPPINESSPERTRADEROUTE
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Player|ChangeHappinessPerTradeRoute}}<b>(</b>'''int''' change<b>)</b></code>
<!-- 
CHANGEJONSCULTURE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Player|ChangeJONSCulture}}<b>(</b>'''int''' change<b>)</b></code>
<!-- 
CHANGEJONSCULTUREPERTURNFORFREE
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Player|ChangeJONSCulturePerTurnForFree}}<b>(</b>'''int''' change<b>)</b></code>
<!-- 
CHANGEJONSCULTUREPERTURNFROMMINORCIVS
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Player|ChangeJONSCulturePerTurnFromMinorCivs}}<b>(</b>'''int''' change<b>)</b></code>
<!-- 
CHANGEMINORCIVFRIENDSHIPWITHMAJOR
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Player|ChangeMinorCivFriendshipWithMajor}}<b>(</b>{{Type5|PlayerID}} player<b>)</b></code>
<!-- 
CHANGENAVALCOMBATEXPERIENCE
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>{{UnknownSignature5}}</code>
|width="100%" |<code>{{FuncLabel5|Player|ChangeNavalCombatExperience}}<!-- No arguments --></code>
<!-- 
CHANGENEWCITYEXTRAPOPULATION
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>{{UnknownSignature5}}</code>
|width="100%" |<code>{{FuncLabel5|Player|ChangeNewCityExtraPopulation}}<!-- No arguments --></code>
<!-- 
CHANGENUMFAITHGREATPEOPLE
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>{{UnknownSignature5}}</code>
|width="100%" |<code>{{FuncLabel5|Player|ChangeNumFaithGreatPeople}}<!-- No arguments --></code>
<!-- 
CHANGENUMFREEGREATPEOPLE
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>{{UnknownSignature5}}</code>
|width="100%" |<code>{{FuncLabel5|Player|ChangeNumFreeGreatPeople}}<!-- No arguments --></code>
<!-- 
CHANGENUMFREEPOLICIES
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Player|ChangeNumFreePolicies}}<b>(</b>'''int''' arg0<b>)</b></code>
<!-- 
CHANGENUMGOLDENAGES
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>{{UnknownSignature5}}</code>
|width="100%" |<code>{{FuncLabel5|Player|ChangeNumGoldenAges}}<!-- No arguments --></code>
<!-- 
CHANGENUMMAYABOOSTS
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>{{UnknownSignature5}}</code>
|width="100%" |<code>{{FuncLabel5|Player|ChangeNumMayaBoosts}}<!-- No arguments --></code>
<!-- 
CHANGENUMPLOTSBOUGHT
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Player|ChangeNumPlotsBought}}<b>(</b>'''int''' change<b>)</b></code>
<!-- 
CHANGENUMRESOURCETOTAL
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Player|ChangeNumResourceTotal}}<b>(</b>{{Type5|ResourceType}} resource, '''int''' change<b>)</b></code>
<!-- 
CHANGENUMUNITGOLDENAGES
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Player|ChangeNumUnitGoldenAges}}<b>(</b>'''int''' change<b>)</b></code>
<!-- 
CHANGENUMWORLDWONDERS
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Player|ChangeNumWorldWonders}}<b>(</b>'''int''' numWondersToCredit<b>)</b></code>
<!-- 
CHANGESCOREFROMFUTURETECH
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Player|ChangeScoreFromFutureTech}}<b>(</b>'''int''' vPReceived<b>)</b></code>
<!-- 
CHANGESCOREFROMTECHS
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Player|ChangeScoreFromTechs}}<b>(</b>'''int''' score<b>)</b></code>
<!-- 
CHANGEUNHAPPINESSFROMUNITS
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Player|ChangeUnhappinessFromUnits}}<b>(</b>'''int''' change<b>)</b></code>
<!-- 
CHOOSETECH
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Player|ChooseTech}}<b>(</b>'''int''' arg0, '''string''' arg1, '''int''' arg2<b>)</b></code>
<!-- 
CITIES
-->
|-
{{FuncInfos5|yes  |yes  |yes|Returns all of a player's cities. Must be used in a for loop because it's an iterator function (see example)}}
|align="right"  |<code>iterator({{Type5|City}})</code>
|width="100%" |<code>{{FuncLabel5|Player|Cities}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
CLEARRESEARCHQUEUE
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>{{UnknownSignature5}}</code>
|width="100%" |<code>{{FuncLabel5|Player|ClearResearchQueue}}<!-- No arguments --></code>
<!-- 
CONTACT
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Player|Contact}}<b>(</b>{{Type5|PlayerID}} player<b>)</b></code>
<!-- 
COUNTCITYFEATURES
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|CountCityFeatures}}<b>(</b>{{Type5|FeatureType}} feature<b>)</b></code>
<!-- 
COUNTNUMBUILDINGS
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|CountNumBuildings}}<b>(</b>{{Type5|BuildingType}} building<b>)</b></code>
<!-- 
CREATEGREATGENERAL
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Player|CreateGreatGeneral}}<b>(</b>{{Type5|Unit}} eGreatPersonUnit, '''bool''' incrementThreshold, '''bool''' incrementExperience, '''int''' x, '''int''' y<b>)</b></code>
|}

==D==
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
DISBAND
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Player|Disband}}<b>(</b>{{Type5|City}} city<b>)</b></code>
<!-- 
DISBANDUNIT
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Player|DisbandUnit}}<b>(</b>'''bool''' announce<b>)</b></code>
<!-- 
DOADOPTPOLICY
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Player|DoAdoptPolicy}}<b>(</b>{{Type5|PolicyType}} policy<b>)</b></code>
<!-- 
DOBEGINDIPLOWITHHUMAN
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Player|DoBeginDiploWithHuman}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
DOFORCEDENOUNCE
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Player|DoForceDenounce}}<b>(</b>{{Type5|PlayerID}} player<b>)</b></code>
<!-- 
DOFORCEDOF
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Player|DoForceDoF}}<b>(</b>{{Type5|PlayerID}} player<b>)</b></code>
<!-- 
DOGOODY
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Player|DoGoody}}<b>(</b>{{Type5|Plot}} plot, {{Type5|Unit}} unit<b>)</b></code>
<!-- 
DOMINORLIBERATIONBYMAJOR
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Player|DoMinorLiberationByMajor}}<b>(</b>{{Type5|PlayerID}} player<b>)</b></code>
<!-- 
DOTRADESCREENCLOSED
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Player|DoTradeScreenClosed}}<b>(</b>'''bool''' aIMakingOffer<b>)</b></code>
<!-- 
DOTRADESCREENOPENED
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Player|DoTradeScreenOpened}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
DOUPDATEPROXIMITYTOPLAYER
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Player|DoUpdateProximityToPlayer}}<b>(</b>{{Type5|PlayerID}} player<b>)</b></code>
|}

==F==
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
FINDNEWCAPITAL
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>{{UnknownSignature5}}</code>
|width="100%" |<code>{{FuncLabel5|Player|FindNewCapital}}<!-- No arguments --></code>
<!-- 
FINDPATHLENGTH
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|FindPathLength}}<b>(</b>{{Type5|TechType}} tech, '''bool''' cost<b>)</b></code>
<!-- 
FORCEPEACE
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Player|ForcePeace}}<b>(</b>{{Type5|PlayerID}} player<b>)</b></code>
<!-- 
FOUND
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Player|Found}}<b>(</b>'''int''' x, '''int''' y<b>)</b></code>
|}

==G==
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
GETACTIVEQUESTFORPLAYER
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>{{Type5|MinorCivQuestType}}</code>
|width="100%" |<code>{{FuncLabel5|Player|GetActiveQuestForPlayer}}<b>(</b>{{Type5|PlayerID}} player<b>)</b></code>
<!-- 
GETADVANCEDSTARTBUILDINGCOST
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetAdvancedStartBuildingCost}}<b>(</b>{{Type5|BuildingType}} building, '''bool''' add, {{Type5|City}} city<b>)</b></code>
<!-- 
GETADVANCEDSTARTCITYCOST
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetAdvancedStartCityCost}}<b>(</b>'''bool''' add, {{Type5|Plot}} plot<b>)</b></code>
<!-- 
GETADVANCEDSTARTIMPROVEMENTCOST
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetAdvancedStartImprovementCost}}<b>(</b>{{Type5|ImprovementType}} improvement, '''bool''' add, {{Type5|Plot}} plot<b>)</b></code>
<!-- 
GETADVANCEDSTARTPOINTS
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetAdvancedStartPoints}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETADVANCEDSTARTPOPCOST
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetAdvancedStartPopCost}}<b>(</b>'''bool''' add, {{Type5|City}} city<b>)</b></code>
<!-- 
GETADVANCEDSTARTROUTECOST
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetAdvancedStartRouteCost}}<b>(</b>{{Type5|RouteType}} route, '''bool''' add, {{Type5|Plot}} plot<b>)</b></code>
<!-- 
GETADVANCEDSTARTTECHCOST
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetAdvancedStartTechCost}}<b>(</b>{{Type5|TechType}} tech, '''bool''' add<b>)</b></code>
<!-- 
GETADVANCEDSTARTUNITCOST
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetAdvancedStartUnitCost}}<b>(</b>{{Type5|UnitType}} unit, '''bool''' add, {{Type5|Plot}} plot<b>)</b></code>
<!-- 
GETADVANCEDSTARTVISIBILITYCOST
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetAdvancedStartVisibilityCost}}<b>(</b>'''bool''' add, {{Type5|Plot}} plot<b>)</b></code>
<!-- 
GETAGRICULTUREHISTORY
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetAgricultureHistory}}<b>(</b>'''int''' turn<b>)</b></code>
<!-- 
GETALLY
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>{{Type5|PlayerID}}</code>
|width="100%" |<code>{{FuncLabel5|Player|GetAlly}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETANARCHYNUMTURNS
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetAnarchyNumTurns}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETANYUNITHASORDERTOGOODY
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetAnyUnitHasOrderToGoody}}<b>(</b>'''unknown''' void<b>)</b></code>
<!-- 
GETAPPROACHTOWARDSUSGUESS
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>{{Type5|MajorCivApproachType}}</code>
|width="100%" |<code>{{FuncLabel5|Player|GetApproachTowardsUsGuess}}<b>(</b>{{Type5|PlayerID}} player<b>)</b></code>
<!-- 
GETARTSTYLETYPE
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>{{Type5|ArtStyleType}}</code>
|width="100%" |<code>{{FuncLabel5|Player|GetArtStyleType}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETATTACKBONUSTURNS
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetAttackBonusTurns}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETAVAILABLESPYRELOCATIONCITIES
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''unknown'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetAvailableSpyRelocationCities}}<b>(</b>'''unknown''' agentID<b>)</b></code>
<!-- 
GETAVERAGEPOPULATION
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetAveragePopulation}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETBARBARIANCOMBATBONUS
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetBarbarianCombatBonus}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETBELIEFINPANTHEON
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>{{Type5|BeliefType}}</code>
|width="100%" |<code>{{FuncLabel5|Player|GetBeliefInPantheon}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETBESTROUTE
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''unknown'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetBestRoute}}<b>(</b>{{Type5|Plot}} plot<b>)</b></code>
<!-- 
GETBRANCHPICKED1
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetBranchPicked1}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETBRANCHPICKED2
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetBranchPicked2}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETBRANCHPICKED3
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetBranchPicked3}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETBUILDINGCLASSCOUNT
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetBuildingClassCount}}<b>(</b>{{Type5|BuildingClassType}} buildingClass<b>)</b></code>
<!-- 
GETBUILDINGCLASSCOUNTPLUSMAKING
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetBuildingClassCountPlusMaking}}<b>(</b>{{Type5|BuildingClassType}} buildingClass<b>)</b></code>
<!-- 
GETBUILDINGCLASSMAKING
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetBuildingClassMaking}}<b>(</b>{{Type5|BuildingClassType}} buildingClass<b>)</b></code>
<!-- 
GETBUILDINGCLASSPREREQBUILDING
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetBuildingClassPrereqBuilding}}<b>(</b>{{Type5|BuildingType}} building, '''unknown''' ePrereqBuildingClass, '''int''' extra<b>)</b></code>
<!-- 
GETBUILDINGGOLDMAINTENANCE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetBuildingGoldMaintenance}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETBUILDINGPRODUCTIONMODIFIER
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>{{UnknownSignature5}}</code>
|width="100%" |<code>{{FuncLabel5|Player|GetBuildingProductionModifier}}<!-- No arguments --></code>
<!-- 
GETBUILDINGPRODUCTIONNEEDED
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetBuildingProductionNeeded}}<b>(</b>'''int''' building<b>)</b></code>
<!-- 
GETBUYOUTCOST
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetBuyoutCost}}<b>(</b>{{Type5|PlayerID}} activePlayer<b>)</b></code>
<!-- 
GETBUYPLOTCOST
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>{{UnknownSignature5}}</code>
|width="100%" |<code>{{FuncLabel5|Player|GetBuyPlotCost}}<!-- No arguments --></code>
<!-- 
GETCAPITALCITY
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>{{Type5|City}}</code>
|width="100%" |<code>{{FuncLabel5|Player|GetCapitalCity}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETCAPITALSETTLERPRODUCTIONMODIFIER
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>{{UnknownSignature5}}</code>
|width="100%" |<code>{{FuncLabel5|Player|GetCapitalSettlerProductionModifier}}<!-- No arguments --></code>
<!-- 
GETCAPITALUNHAPPINESSMOD
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetCapitalUnhappinessMod}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETCAPITALYIELDRATEMODIFIER
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetCapitalYieldRateModifier}}<b>(</b>{{Type5|YieldType}} index<b>)</b></code>
<!-- 
GETCITIESLOST
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetCitiesLost}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETCITYBYID
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>{{Type5|City}}</code>
|width="100%" |<code>{{FuncLabel5|Player|GetCityByID}}<b>(</b>{{Type5|CityID}} city<b>)</b></code>
<!-- 
GETCITYCONNECTIONGOLD
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetCityConnectionGold}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETCITYCONNECTIONGOLDTIMES100
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetCityConnectionGoldTimes100}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETCITYCOUNTUNHAPPINESSMOD
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetCityCountUnhappinessMod}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETCITYDEFENSEMODIFIER
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetCityDefenseModifier}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETCITYNAME
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''string'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetCityName}}<b>(</b>'''int''' index<b>)</b></code>
<!-- 
GETCIVILIZATIONADJECTIVE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''string'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetCivilizationAdjective}}<b>(</b>'''int''' form<b>)</b></code>
<!-- 
GETCIVILIZATIONADJECTIVEKEY
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''string'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetCivilizationAdjectiveKey}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETCIVILIZATIONDESCRIPTION
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''string'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetCivilizationDescription}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETCIVILIZATIONDESCRIPTIONKEY
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''string'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetCivilizationDescriptionKey}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETCIVILIZATIONSHORTDESCRIPTION
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''string'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetCivilizationShortDescription}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETCIVILIZATIONSHORTDESCRIPTIONKEY
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''string'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetCivilizationShortDescriptionKey}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETCIVILIZATIONTYPE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>{{Type5|CivilizationType}}</code>
|width="100%" |<code>{{FuncLabel5|Player|GetCivilizationType}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETCLOSESTGOODYPLOT
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>{{Type5|Plot}}</code>
|width="100%" |<code>{{FuncLabel5|Player|GetClosestGoodyPlot}}<b>(</b>'''unknown''' void<b>)</b></code>
<!-- 
GETCOMBATBONUSVSHIGHERTECH
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetCombatBonusVsHigherTech}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETCOMBATBONUSVSLARGERCIV
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetCombatBonusVsLargerCiv}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETCOMBATEXPERIENCE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetCombatExperience}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETCOMMONFOEVALUE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetCommonFoeValue}}<b>(</b>{{Type5|PlayerID}} activePlayer<b>)</b></code>
<!-- 
GETCONSCRIPTCOUNT
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetConscriptCount}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETCONVERSIONTIMER
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetConversionTimer}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETCOOPWARACCEPTEDSTATE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>{{Type5|CoopWarState}}</code>
|width="100%" |<code>{{FuncLabel5|Player|GetCoopWarAcceptedState}}<b>(</b>{{Type5|PlayerID}} withPlayer, {{Type5|PlayerID}} againstPlayer<b>)</b></code>
<!-- 
GETCOUPCHANCEOFSUCCESS
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''unknown'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetCoupChanceOfSuccess}}<b>(</b>'''int''' city<b>)</b></code>
<!-- 
GETCULTUREBOMBTIMER
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetCultureBombTimer}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETCULTURECITYMODIFIER
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetCultureCityModifier}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETCULTUREPERTURNFROMMINOR
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>{{UnknownSignature5}}</code>
|width="100%" |<code>{{FuncLabel5|Player|GetCulturePerTurnFromMinor}}<!-- No arguments --></code>
<!-- 
GETCULTUREPERTURNFROMMINORCIVS
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetCulturePerTurnFromMinorCivs}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETCULTUREPERTURNFROMRELIGION
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetCulturePerTurnFromReligion}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETCULTUREWONDERMULTIPLIER
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetCultureWonderMultiplier}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETCURRENTCAPITALFOODBONUS
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetCurrentCapitalFoodBonus}}<b>(</b>{{Type5|PlayerID}} major<b>)</b></code>
<!-- 
GETCURRENTCULTUREBONUS
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetCurrentCultureBonus}}<b>(</b>{{Type5|PlayerID}} activePlayer<b>)</b></code>
<!-- 
GETCURRENTERA
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>{{Type5|EraType}}</code>
|width="100%" |<code>{{FuncLabel5|Player|GetCurrentEra}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETCURRENTOTHERCITYFOODBONUS
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetCurrentOtherCityFoodBonus}}<b>(</b>{{Type5|PlayerID}} major<b>)</b></code>
<!-- 
GETCURRENTRESEARCH
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>{{Type5|TechType}}</code>
|width="100%" |<code>{{FuncLabel5|Player|GetCurrentResearch}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETCURRENTSCIENCEFRIENDSHIPBONUSTIMES100
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetCurrentScienceFriendshipBonusTimes100}}<b>(</b>{{Type5|PlayerID}} major<b>)</b></code>
<!-- 
GETCURRENTSPAWNESTIMATE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetCurrentSpawnEstimate}}<b>(</b>{{Type5|PlayerID}} major<b>)</b></code>
<!-- 
GETDEALMYVALUE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>{{Type5|SpecialistType}}</code>
|width="100%" |<code>{{FuncLabel5|Player|GetDealMyValue}}<b>(</b>{{Type5|Deal}} Deal<b>)</b></code>
<!-- 
GETDEALTHEYREVALUE
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>{{UnknownSignature5}}</code>
|width="100%" |<code>{{FuncLabel5|Player|GetDealTheyreValue}}<!-- No arguments --></code>
<!-- 
GETDEALVALUE
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>{{UnknownSignature5}}</code>
|width="100%" |<code>{{FuncLabel5|Player|GetDealValue}}<!-- No arguments --></code>
<!-- 
GETDOMESTICGREATGENERALRATEMODIFIER
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetDomesticGreatGeneralRateModifier}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETDOMINANTPOLICYBRANCHFORTITLE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>{{Type5|PolicyBranchType}}</code>
|width="100%" |<code>{{FuncLabel5|Player|GetDominantPolicyBranchForTitle}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETECONOMYHISTORY
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetEconomyHistory}}<b>(</b>'''int''' turn<b>)</b></code>
<!-- 
GETEMBARKEDGRAPHICOVERRIDE
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>{{UnknownSignature5}}</code>
|width="100%" |<code>{{FuncLabel5|Player|GetEmbarkedGraphicOverride}}<!-- No arguments --></code>
<!-- 
GETENDTURNBLOCKINGNOTIFICATIONINDEX
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>{{Type5|EndTurnBlockingType}}</code>
|width="100%" |<code>{{FuncLabel5|Player|GetEndTurnBlockingNotificationIndex}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETENDTURNBLOCKINGTYPE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>{{Type5|EndTurnBlockingType}}</code>
|width="100%" |<code>{{FuncLabel5|Player|GetEndTurnBlockingType}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETESPIONAGECITYSTATUS
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>table('''int''' => {{Type5|CityEspionageInfo}})</code>
|width="100%" |<code>{{FuncLabel5|Player|GetEspionageCityStatus}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETESPIONAGESPIES
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>table('''int''' => {{Type5|SpyInfo}})</code>
|width="100%" |<code>{{FuncLabel5|Player|GetEspionageSpies}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETEVERPOPPEDGOODY
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetEverPoppedGoody}}<b>(</b>'''unknown''' void<b>)</b></code>
<!-- 
GETEVERTRAINEDBUILDER
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetEverTrainedBuilder}}<b>(</b>'''unknown''' void<b>)</b></code>
<!-- 
GETEXCESSHAPPINESS
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetExcessHappiness}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETEXPINBORDERMODIFIER
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetExpInBorderModifier}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETEXTRABUILDINGHAPPINESSFROMPOLICIES
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetExtraBuildingHappinessFromPolicies}}<b>(</b>{{Type5|PlayerID}} building<b>)</b></code>
<!-- 
GETEXTRAHAPPINESSPERCITY
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetExtraHappinessPerCity}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETEXTRAHAPPINESSPERLUXURY
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetExtraHappinessPerLuxury}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETEXTRAUNITCOST
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetExtraUnitCost}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETEXTRAYIELDTHRESHOLD
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetExtraYieldThreshold}}<b>(</b>{{Type5|YieldType}} index<b>)</b></code>
<!-- 
GETFAITH
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetFaith}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETFAITHPERTURNFROMCITIES
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetFaithPerTurnFromCities}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETFAITHPERTURNFROMMINORCIVS
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetFaithPerTurnFromMinorCivs}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETFAITHPERTURNFROMRELIGION
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetFaithPerTurnFromReligion}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETFAITHPURCHASEINDEX
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetFaithPurchaseIndex}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETFAITHPURCHASETYPE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>{{Type5|FaithPurchaseType}}</code>
|width="100%" |<code>{{FuncLabel5|Player|GetFaithPurchaseType}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETFEATUREPRODUCTIONMODIFIER
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetFeatureProductionModifier}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETFIRSTREADYUNIT
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>{{Type5|Unit}}</code>
|width="100%" |<code>{{FuncLabel5|Player|GetFirstReadyUnit}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETFIRSTREADYUNITPLOT
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''unknown'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetFirstReadyUnitPlot}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETFOUNDEDRELIGIONENEMYCITYCOMBATMOD
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetFoundedReligionEnemyCityCombatMod}}<b>(</b>{{Type5|Plot}} toPlot<b>)</b></code>
<!-- 
GETFOUNDEDRELIGIONFRIENDLYCITYCOMBATMOD
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetFoundedReligionFriendlyCityCombatMod}}<b>(</b>{{Type5|Plot}} toPlot<b>)</b></code>
<!-- 
GETFREEEXPERIENCE
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetFreeExperience}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETFREEPROMOTIONCOUNT
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>{{UnknownSignature5}}</code>
|width="100%" |<code>{{FuncLabel5|Player|GetFreePromotionCount}}<!-- No arguments --></code>
<!-- 
GETFRIENDSHIPCHANGEPERTURNTIMES100
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetFriendshipChangePerTurnTimes100}}<b>(</b>{{Type5|PlayerID}} major<b>)</b></code>
<!-- 
GETFRIENDSHIPFROMGOLDGIFT
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetFriendshipFromGoldGift}}<b>(</b>{{Type5|PlayerID}} activePlayer, '''int''' gold<b>)</b></code>
<!-- 
GETFRIENDSHIPNEEDEDFORNEXTLEVEL
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetFriendshipNeededForNextLevel}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETGARRISONEDCITYRANGESTRIKEMODIFIER
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetGarrisonedCityRangeStrikeModifier}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETGIFTTILEIMPROVEMENTCOST
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetGiftTileImprovementCost}}<b>(</b>{{Type5|PlayerID}} activePlayer<b>)</b></code>
<!-- 
GETGOLD
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetGold}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETGOLDENAGELENGTH
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetGoldenAgeLength}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETGOLDENAGEMODIFIER
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetGoldenAgeModifier}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETGOLDENAGEPROGRESSMETER
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''unknown'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetGoldenAgeProgressMeter}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETGOLDENAGEPROGRESSTHRESHOLD
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetGoldenAgeProgressThreshold}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETGOLDENAGETURNS
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetGoldenAgeTurns}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETGOLDFROMCITIESTIMES100
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetGoldFromCitiesTimes100}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETGOLDPERMILITARYUNIT
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetGoldPerMilitaryUnit}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETGOLDPERTURNFROMDIPLOMACY
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetGoldPerTurnFromDiplomacy}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETGOLDPERTURNFROMRELIGION
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetGoldPerTurnFromReligion}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETGOLDPERUNIT
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetGoldPerUnit}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETGREATADMIRALSTHRESHOLDMODIFIER
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>{{UnknownSignature5}}</code>
|width="100%" |<code>{{FuncLabel5|Player|GetGreatAdmiralsThresholdModifier}}<!-- No arguments --></code>
<!-- 
GETGREATGENERALRATEMODIFIER
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetGreatGeneralRateModifier}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETGREATGENERALSCREATED
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetGreatGeneralsCreated}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETGREATGENERALSTHRESHOLDMODIFIER
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetGreatGeneralsThresholdModifier}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETGREATPEOPLECREATED
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetGreatPeopleCreated}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETGREATPEOPLERATEMODIFIER
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetGreatPeopleRateModifier}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETGREATPEOPLETHRESHOLDMODIFIER
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetGreatPeopleThresholdModifier}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETHANDICAPTYPE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>{{Type5|HandicapType}}</code>
|width="100%" |<code>{{FuncLabel5|Player|GetHandicapType}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETHAPPINESS
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetHappiness}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETHAPPINESSFROMBUILDINGS
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetHappinessFromBuildings}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETHAPPINESSFROMCITIES
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetHappinessFromCities}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETHAPPINESSFROMGARRISONEDUNITS
-->
|-
{{FuncInfos5|yes  |no   |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetHappinessFromGarrisonedUnits}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETHAPPINESSFROMLUXURY
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetHappinessFromLuxury}}<b>(</b>{{Type5|ResourceType}} resource<b>)</b></code>
<!-- 
GETHAPPINESSFROMMINOR
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetHappinessFromMinor}}<b>(</b>{{Type5|PlayerID}} minor<b>)</b></code>
<!-- 
GETHAPPINESSFROMMINORCIVS
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetHappinessFromMinorCivs}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETHAPPINESSFROMNATURALWONDERS
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetHappinessFromNaturalWonders}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETHAPPINESSFROMPOLICIES
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetHappinessFromPolicies}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETHAPPINESSFROMRELIGION
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetHappinessFromReligion}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETHAPPINESSFROMRESOURCES
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetHappinessFromResources}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETHAPPINESSFROMRESOURCEVARIETY
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetHappinessFromResourceVariety}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETHAPPINESSFROMTRADEROUTES
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetHappinessFromTradeRoutes}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETHAPPINESSPERGARRISONEDUNIT
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetHappinessPerGarrisonedUnit}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETHAPPINESSPERTRADEROUTE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetHappinessPerTradeRoute}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETHAPPYPERMILITARYUNIT
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetHappyPerMilitaryUnit}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETHIGHESTUNITLEVEL
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetHighestUnitLevel}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETHURRYCOUNT
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetHurryCount}}<b>(</b>{{Type5|HurryType}} hurry<b>)</b></code>
<!-- 
GETHURRYGOLDCOST
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetHurryGoldCost}}<b>(</b>{{Type5|HurryType}} hurry<b>)</b></code>
<!-- 
GETHURRYMODIFIER
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetHurryModifier}}<b>(</b>{{Type5|HurryType}} hurry<b>)</b></code>
<!-- 
GETID
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>{{Type5|PlayerID}}</code>
|width="100%" |<code>{{FuncLabel5|Player|GetID}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETIMPROVEMENTCOUNT
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetImprovementCount}}<b>(</b>{{Type5|ImprovementType}} improvement<b>)</b></code>
<!-- 
GETIMPROVEMENTGOLDMAINTENANCE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetImprovementGoldMaintenance}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETIMPROVEMENTUPGRADERATE
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetImprovementUpgradeRate}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETIMPROVEMENTUPGRADERATEMODIFIER
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetImprovementUpgradeRateModifier}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETINDUSTRYHISTORY
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetIndustryHistory}}<b>(</b>'''int''' turn<b>)</b></code>
<!-- 
GETINTRIGUEMESSAGES
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>table('''int''' => {{Type5|IntrigueInfo}})</code>
|width="100%" |<code>{{FuncLabel5|Player|GetIntrigueMessages}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETJONSCULTURE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetJONSCulture}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETJONSCULTUREEVERGENERATED
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>{{UnknownSignature5}}</code>
|width="100%" |<code>{{FuncLabel5|Player|GetJONSCultureEverGenerated}}<!-- No arguments --></code>
<!-- 
GETJONSCULTUREPERTURNFORFREE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetJONSCulturePerTurnForFree}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETJONSCULTUREPERTURNFROMCITIES
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetJONSCulturePerTurnFromCities}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETJONSCULTUREPERTURNFROMEXCESSHAPPINESS
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetJONSCulturePerTurnFromExcessHappiness}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETJONSCULTUREPERTURNFROMMINORCIVS
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetJONSCulturePerTurnFromMinorCivs}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETLANDDISPUTELEVEL
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>{{Type5|DisputeLevelType}}</code>
|width="100%" |<code>{{FuncLabel5|Player|GetLandDisputeLevel}}<b>(</b>{{Type5|PlayerID}} activePlayer<b>)</b></code>
<!-- 
GETLANDSCORE
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetLandScore}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETLATEGAMEPOLICYTREE
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>{{UnknownSignature5}}</code>
|width="100%" |<code>{{FuncLabel5|Player|GetLateGamePolicyTree}}<!-- No arguments --></code>
<!-- 
GETLEADERTYPE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>{{Type5|LeaderType}}</code>
|width="100%" |<code>{{FuncLabel5|Player|GetLeaderType}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETLENGTHRESEARCHQUEUE
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetLengthResearchQueue}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETLEVELEXPERIENCEMODIFIER
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetLevelExperienceModifier}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETLIFETIMECOMBATEXPERIENCE
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>{{UnknownSignature5}}</code>
|width="100%" |<code>{{FuncLabel5|Player|GetLifetimeCombatExperience}}<!-- No arguments --></code>
<!-- 
GETLIFETIMEGROSSGOLD
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetLifetimeGrossGold}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETMAJORCIVAPPROACH
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>{{UnknownSignature5}}</code>
|width="100%" |<code>{{FuncLabel5|Player|GetMajorCivApproach}}<!-- No arguments --></code>
<!-- 
GETMAXCONSCRIPT
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetMaxConscript}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETMAXGLOBALBUILDINGPRODUCTIONMODIFIER
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetMaxGlobalBuildingProductionModifier}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETMAXPLAYERBUILDINGPRODUCTIONMODIFIER
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetMaxPlayerBuildingProductionModifier}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETMAXTEAMBUILDINGPRODUCTIONMODIFIER
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetMaxTeamBuildingProductionModifier}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETMAYACALENDARLONGSTRING
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''string'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetMayaCalendarLongString}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETMAYACALENDARSTRING
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''string'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetMayaCalendarString}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETMILITARYMIGHT
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetMilitaryMight}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETMILITARYPRODUCTIONMODIFIER
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetMilitaryProductionModifier}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETMINIMUMFAITHNEXTGREATPROPHET
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''unknown'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetMinimumFaithNextGreatProphet}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETMINORCIVBULLYGOLDAMOUNT
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetMinorCivBullyGoldAmount}}<b>(</b>{{Type5|PlayerID}} activePlayer<b>)</b></code>
<!-- 
GETMINORCIVCONTESTVALUEFORLEADER
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetMinorCivContestValueForLeader}}<b>(</b>{{Type5|MinorCivQuestType}} arg0<b>)</b></code>
<!-- 
GETMINORCIVCONTESTVALUEFORPLAYER
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetMinorCivContestValueForPlayer}}<b>(</b>{{Type5|PlayerID}} major, {{Type5|MinorCivQuestType}} arg1<b>)</b></code>
<!-- 
GETMINORCIVCULTUREFRIENDSHIPBONUS
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetMinorCivCultureFriendshipBonus}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETMINORCIVCURRENTCULTUREBONUS
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetMinorCivCurrentCultureBonus}}<b>(</b>{{Type5|PlayerID}} major<b>)</b></code>
<!-- 
GETMINORCIVCURRENTCULTUREFLATBONUS
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>{{UnknownSignature5}}</code>
|width="100%" |<code>{{FuncLabel5|Player|GetMinorCivCurrentCultureFlatBonus}}<!-- No arguments --></code>
<!-- 
GETMINORCIVCURRENTCULTUREPERBUILDINGBONUS
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>{{UnknownSignature5}}</code>
|width="100%" |<code>{{FuncLabel5|Player|GetMinorCivCurrentCulturePerBuildingBonus}}<!-- No arguments --></code>
<!-- 
GETMINORCIVCURRENTFAITHBONUS
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetMinorCivCurrentFaithBonus}}<b>(</b>{{Type5|PlayerID}} major<b>)</b></code>
<!-- 
GETMINORCIVCURRENTHAPPINESSBONUS
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetMinorCivCurrentHappinessBonus}}<b>(</b>{{Type5|PlayerID}} major<b>)</b></code>
<!-- 
GETMINORCIVCURRENTHAPPINESSFLATBONUS
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>{{UnknownSignature5}}</code>
|width="100%" |<code>{{FuncLabel5|Player|GetMinorCivCurrentHappinessFlatBonus}}<!-- No arguments --></code>
<!-- 
GETMINORCIVCURRENTHAPPINESSPERLUXURYBONUS
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>{{UnknownSignature5}}</code>
|width="100%" |<code>{{FuncLabel5|Player|GetMinorCivCurrentHappinessPerLuxuryBonus}}<!-- No arguments --></code>
<!-- 
GETMINORCIVDISPUTELEVEL
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>{{Type5|DisputeLevelType}}</code>
|width="100%" |<code>{{FuncLabel5|Player|GetMinorCivDisputeLevel}}<b>(</b>{{Type5|PlayerID}} activePlayer<b>)</b></code>
<!-- 
GETMINORCIVFAVORITEMAJOR
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''unknown'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetMinorCivFavoriteMajor}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETMINORCIVFRIENDSHIPANCHORWITHMAJOR
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetMinorCivFriendshipAnchorWithMajor}}<b>(</b>{{Type5|PlayerID}} major<b>)</b></code>
<!-- 
GETMINORCIVFRIENDSHIPLEVELWITHMAJOR
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetMinorCivFriendshipLevelWithMajor}}<b>(</b>{{Type5|PlayerID}} arg0<b>)</b></code>
<!-- 
GETMINORCIVFRIENDSHIPWITHMAJOR
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetMinorCivFriendshipWithMajor}}<b>(</b>{{Type5|PlayerID}} major<b>)</b></code>
<!-- 
GETMINORCIVHAPPINESSFRIENDSHIPBONUS
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetMinorCivHappinessFriendshipBonus}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETMINORCIVNUMACTIVEQUESTSFORPLAYER
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetMinorCivNumActiveQuestsForPlayer}}<b>(</b>{{Type5|PlayerID}} player<b>)</b></code>
<!-- 
GETMINORCIVSCIENCEFRIENDSHIPBONUS
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetMinorCivScienceFriendshipBonus}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETMINORCIVTRAIT
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>{{Type5|MinorCivTraitType}}</code>
|width="100%" |<code>{{FuncLabel5|Player|GetMinorCivTrait}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETMINORCIVTYPE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetMinorCivType}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETMINORCIVUNIQUEUNIT
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>{{Type5|UnitType}}</code>
|width="100%" |<code>{{FuncLabel5|Player|GetMinorCivUniqueUnit}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETMINORWARQUESTWITHMAJORREMAININGCOUNT
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetMinorWarQuestWithMajorRemainingCount}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETNAME
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''string'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetName}}<b>(</b>'''string''' form<b>)</b></code>
<!-- 
GETNAMEKEY
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''string'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetNameKey}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETNATURALWONDERYIELDMODIFIER
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetNaturalWonderYieldModifier}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETNAVALCOMBATEXPERIENCE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetNavalCombatExperience}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETNEGATIVERELIGIOUSCONVERSIONPOINTS
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>{{UnknownSignature5}}</code>
|width="100%" |<code>{{FuncLabel5|Player|GetNegativeReligiousConversionPoints}}<!-- No arguments --></code>
<!-- 
GETNEWCITYEXTRAPOPULATION
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>{{UnknownSignature5}}</code>
|width="100%" |<code>{{FuncLabel5|Player|GetNewCityExtraPopulation}}<!-- No arguments --></code>
<!-- 
GETNEWCITYNAME
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''string'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetNewCityName}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETNEXTCITY
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''unknown'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetNextCity}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETNEXTPOLICYCOST
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetNextPolicyCost}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETNICKNAME
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''string'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetNickName}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETNOTIFICATIONDISMISSED
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetNotificationDismissed}}<b>(</b>'''int''' arg0<b>)</b></code>
<!-- 
GETNOTIFICATIONINDEX
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>{{Type5|EndTurnBlockingType}}</code>
|width="100%" |<code>{{FuncLabel5|Player|GetNotificationIndex}}<b>(</b>'''int''' i<b>)</b></code>
<!-- 
GETNOTIFICATIONSTR
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''string'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetNotificationStr}}<b>(</b>'''int''' i<b>)</b></code>
<!-- 
GETNOTIFICATIONSUMMARYSTR
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''string'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetNotificationSummaryStr}}<b>(</b>'''int''' i<b>)</b></code>
<!-- 
GETNOTIFICATIONTURN
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetNotificationTurn}}<b>(</b>'''int''' arg0<b>)</b></code>
<!-- 
GETNUMCITIES
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetNumCities}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETNUMCITYNAMES
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetNumCityNames}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETNUMCIVILIANSRETURNEDTOME
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetNumCiviliansReturnedToMe}}<b>(</b>{{Type5|PlayerID}} activePlayer<b>)</b></code>
<!-- 
GETNUMFAITHGREATPEOPLE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetNumFaithGreatPeople}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETNUMFREEGREATPEOPLE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetNumFreeGreatPeople}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETNUMFREEPOLICIES
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetNumFreePolicies}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETNUMFREETECHS
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>{{Type5|ResourceType}}</code>
|width="100%" |<code>{{FuncLabel5|Player|GetNumFreeTechs}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETNUMFRIENDSDENOUNCEDBY
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetNumFriendsDenouncedBy}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETNUMGOLDENAGES
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetNumGoldenAges}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETNUMMAINTENANCEFREEUNITS
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetNumMaintenanceFreeUnits}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETNUMMAYABOOSTS
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetNumMayaBoosts}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETNUMMILITARYUNITS
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetNumMilitaryUnits}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETNUMMINORCIVSMET
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetNumMinorCivsMet}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETNUMNOTIFICATIONS
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetNumNotifications}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETNUMNUKEUNITS
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetNumNukeUnits}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETNUMOUTSIDEUNITS
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetNumOutsideUnits}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETNUMPLOTS
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetNumPlots}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETNUMPLOTSBOUGHT
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetNumPlotsBought}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETNUMPOLICIES
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetNumPolicies}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETNUMPOLICYBRANCHESALLOWED
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetNumPolicyBranchesAllowed}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETNUMPOLICYBRANCHESFINISHED
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetNumPolicyBranchesFinished}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETNUMPOLICYBRANCHESUNLOCKED
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetNumPolicyBranchesUnlocked}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETNUMREQUESTSREFUSED
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetNumRequestsRefused}}<b>(</b>{{Type5|PlayerID}} activePlayer<b>)</b></code>
<!-- 
GETNUMRESOURCEAVAILABLE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetNumResourceAvailable}}<b>(</b>{{Type5|ResourceType}} resource, '''bool''' includeImport<b>)</b></code>
<!-- 
GETNUMRESOURCETOTAL
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetNumResourceTotal}}<b>(</b>{{Type5|ResourceType}} resource, '''bool''' includeImport<b>)</b></code>
<!-- 
GETNUMRESOURCEUSED
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetNumResourceUsed}}<b>(</b>{{Type5|ResourceType}} resource<b>)</b></code>
<!-- 
GETNUMSPIES
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetNumSpies}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETNUMTECHSTOSTEAL
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetNumTechsToSteal}}<b>(</b>'''int''' stealingTechTargetPlayerID<b>)</b></code>
<!-- 
GETNUMTIMESCULTUREBOMBED
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetNumTimesCultureBombed}}<b>(</b>{{Type5|PlayerID}} activePlayer<b>)</b></code>
<!-- 
GETNUMTIMESINTRIGUESHAREDBY
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>{{UnknownSignature5}}</code>
|width="100%" |<code>{{FuncLabel5|Player|GetNumTimesIntrigueSharedBy}}<!-- No arguments --></code>
<!-- 
GETNUMTIMESROBBEDBY
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>{{UnknownSignature5}}</code>
|width="100%" |<code>{{FuncLabel5|Player|GetNumTimesRobbedBy}}<!-- No arguments --></code>
<!-- 
GETNUMTRADERESOURCEIMPORTS
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetNumTradeResourceImports}}<b>(</b>{{Type5|PlayerID}} player<b>)</b></code>
<!-- 
GETNUMUNASSIGNEDSPIES
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetNumUnassignedSpies}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETNUMUNITGOLDENAGES
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetNumUnitGoldenAges}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETNUMUNITS
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetNumUnits}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETNUMUNITSOUTOFSUPPLY
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetNumUnitsOutOfSupply}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETNUMUNITSSUPPLIED
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetNumUnitsSupplied}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETNUMUNITSSUPPLIEDBYCITIES
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetNumUnitsSuppliedByCities}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETNUMUNITSSUPPLIEDBYHANDICAP
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetNumUnitsSuppliedByHandicap}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETNUMUNITSSUPPLIEDBYPOPULATION
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetNumUnitsSuppliedByPopulation}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETNUMWARSFOUGHT
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetNumWarsFought}}<b>(</b>{{Type5|PlayerID}} otherPlayer<b>)</b></code>
<!-- 
GETNUMWONDERSBEATENTO
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>{{UnknownSignature5}}</code>
|width="100%" |<code>{{FuncLabel5|Player|GetNumWondersBeatenTo}}<!-- No arguments --></code>
<!-- 
GETNUMWORLDWONDERS
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetNumWorldWonders}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETOCCUPIEDPOPULATIONUNHAPPINESSMOD
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetOccupiedPopulationUnhappinessMod}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETOPINIONTABLE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>table('''unknown''' => '''unknown''')</code>
|width="100%" |<code>{{FuncLabel5|Player|GetOpinionTable}}<b>(</b>{{Type5|PlayerID}} activePlayer<b>)</b></code>
<!-- 
GETOTHERPLAYERNUMPROTECTEDMINORSATTACKED
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetOtherPlayerNumProtectedMinorsAttacked}}<b>(</b>{{Type5|PlayerID}} activePlayer<b>)</b></code>
<!-- 
GETOTHERPLAYERNUMPROTECTEDMINORSKILLED
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetOtherPlayerNumProtectedMinorsKilled}}<b>(</b>{{Type5|PlayerID}} activePlayer<b>)</b></code>
<!-- 
GETOVERFLOWRESEARCH
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetOverflowResearch}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETPERSONALITY
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>{{Type5|MinorCivPersonalityType}}</code>
|width="100%" |<code>{{FuncLabel5|Player|GetPersonality}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETPERSONALITYTYPE
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''unknown'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetPersonalityType}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETPLAYERBUILDINGCLASSHAPPINESS
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetPlayerBuildingClassHappiness}}<b>(</b>{{Type5|BuildingClassType}} buildingClass<b>)</b></code>
<!-- 
GETPLAYERBUILDINGCLASSYIELDCHANGE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetPlayerBuildingClassYieldChange}}<b>(</b>{{Type5|BuildingClassType}} buildingClass, {{Type5|YieldType}} arg1<b>)</b></code>
<!-- 
GETPLAYERCOLOR
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>{{Type5|ColorType}}</code>
|width="100%" |<code>{{FuncLabel5|Player|GetPlayerColor}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETPLAYERCOLORS
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>{{Type5|Vector4}}, {{Type5|Vector4}}</code>
|width="100%" |<code>{{FuncLabel5|Player|GetPlayerColors}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETPLAYERVISIBLEPLOT
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''unknown'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetPlayerVisiblePlot}}<b>(</b>{{Type5|Player}} player<b>)</b></code>
<!-- 
GETPLOTDANGER
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetPlotDanger}}<b>(</b>{{Type5|Plot}} plot<b>)</b></code>
<!-- 
GETPLOTHASORDER
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetPlotHasOrder}}<b>(</b>{{Type5|Plot}} Plot<b>)</b></code>
<!-- 
GETPOLICYBRANCHCHOSEN
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetPolicyBranchChosen}}<b>(</b>{{Type5|PolicyType}} policyBranch<b>)</b></code>
<!-- 
GETPOLICYBUILDINGCLASSYIELDCHANGE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetPolicyBuildingClassYieldChange}}<b>(</b>{{Type5|BuildingClassType}} buildingClass, {{Type5|YieldType}} arg1<b>)</b></code>
<!-- 
GETPOLICYBUILDINGCLASSYIELDMODIFIER
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetPolicyBuildingClassYieldModifier}}<b>(</b>{{Type5|BuildingClassType}} buildingClass, {{Type5|YieldType}} arg1<b>)</b></code>
<!-- 
GETPOLICYCATCHSPIESMODIFIER
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetPolicyCatchSpiesModifier}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETPOLICYESPIONAGECATCHSPIESMODIFIER
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetPolicyEspionageCatchSpiesModifier}}<b>(</b>'''int''' i<b>)</b></code>
<!-- 
GETPOLICYESPIONAGEMODIFIER
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetPolicyEspionageModifier}}<b>(</b>'''int''' i<b>)</b></code>
<!-- 
GETPOPSCORE
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetPopScore}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETPOWER
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetPower}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETPOWERHISTORY
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetPowerHistory}}<b>(</b>'''int''' turn<b>)</b></code>
<!-- 
GETPREVCITY
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''unknown'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetPrevCity}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETPRODUCTIONMODIFIER
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>{{UnknownSignature5}}</code>
|width="100%" |<code>{{FuncLabel5|Player|GetProductionModifier}}<!-- No arguments --></code>
<!-- 
GETPROJECTPRODUCTIONMODIFIER
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>{{UnknownSignature5}}</code>
|width="100%" |<code>{{FuncLabel5|Player|GetProjectProductionModifier}}<!-- No arguments --></code>
<!-- 
GETPROJECTPRODUCTIONNEEDED
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetProjectProductionNeeded}}<b>(</b>{{Type5|ProjectType}} project<b>)</b></code>
<!-- 
GETPROXIMITYTOPLAYER
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetProximityToPlayer}}<b>(</b>{{Type5|PlayerID}} index<b>)</b></code>
<!-- 
GETQUESTDATA1
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetQuestData1}}<b>(</b>{{Type5|PlayerID}} major, {{Type5|MinorCivQuestType}} type = nil<b>)</b></code>
<!-- 
GETQUESTDATA2
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetQuestData2}}<b>(</b>{{Type5|PlayerID}} major, {{Type5|MinorCivQuestType}} type = nil<b>)</b></code>
<!-- 
GETQUESTTURNSREMAINING
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetQuestTurnsRemaining}}<b>(</b>{{Type5|PlayerID}} major, {{Type5|MinorCivQuestType}} type, {{Type5|PlayerID}} arg2<b>)</b></code>
<!-- 
GETQUEUEPOSITION
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetQueuePosition}}<b>(</b>{{Type5|TechType}} tech<b>)</b></code>
<!-- 
GETREALPOPULATION
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetRealPopulation}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETRECENTASSISTVALUE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetRecentAssistValue}}<b>(</b>{{Type5|PlayerID}} activePlayer<b>)</b></code>
<!-- 
GETRECENTINTRIGUEINFO
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>{{Type5|SpecialistType}}, '''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetRecentIntrigueInfo}}<b>(</b>{{Type5|PlayerID}} aIPlayer<b>)</b></code>
<!-- 
GETRECENTTRADEVALUE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetRecentTradeValue}}<b>(</b>{{Type5|PlayerID}} activePlayer<b>)</b></code>
<!-- 
GETRECOMMENDEDFOUNDCITYPLOTS
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>table('''unknown''' => '''unknown''')</code>
|width="100%" |<code>{{FuncLabel5|Player|GetRecommendedFoundCityPlots}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETRECOMMENDEDWORKERPLOTS
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>table('''unknown''' => '''unknown''')</code>
|width="100%" |<code>{{FuncLabel5|Player|GetRecommendedWorkerPlots}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETRELIGIONCREATEDBYPLAYER
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>{{Type5|ReligionType}}</code>
|width="100%" |<code>{{FuncLabel5|Player|GetReligionCreatedByPlayer}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETREPLAYDATA
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>table('''unknown''' => '''unknown''')</code>
|width="100%" |<code>{{FuncLabel5|Player|GetReplayData}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETRESEARCHCOST
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetResearchCost}}<b>(</b>{{Type5|TechType}} currentTech<b>)</b></code>
<!-- 
GETRESEARCHPROGRESS
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetResearchProgress}}<b>(</b>{{Type5|TechType}} currentTech<b>)</b></code>
<!-- 
GETRESEARCHTURNSLEFT
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetResearchTurnsLeft}}<b>(</b>{{Type5|TechType}} tech, '''bool''' overflow<b>)</b></code>
<!-- 
GETRESOURCEEXPORT
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetResourceExport}}<b>(</b>{{Type5|ResourceType}} resource<b>)</b></code>
<!-- 
GETRESOURCEFROMMINORS
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetResourceFromMinors}}<b>(</b>{{Type5|ResourceType}} resource<b>)</b></code>
<!-- 
GETRESOURCEIMPORT
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetResourceImport}}<b>(</b>{{Type5|ResourceType}} resource<b>)</b></code>
<!-- 
GETROUTEGOLDTIMES100
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetRouteGoldTimes100}}<b>(</b>{{Type5|City}} city<b>)</b></code>
<!-- 
GETSCIENCE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetScience}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETSCIENCEFROMBUDGETDEFICITTIMES100
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetScienceFromBudgetDeficitTimes100}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETSCIENCEFROMCITIESTIMES100
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetScienceFromCitiesTimes100}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETSCIENCEFROMHAPPINESSTIMES100
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetScienceFromHappinessTimes100}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETSCIENCEFROMOTHERPLAYERSTIMES100
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetScienceFromOtherPlayersTimes100}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETSCIENCEFROMRESEARCHAGREEMENTSTIMES100
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetScienceFromResearchAgreementsTimes100}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETSCIENCETIMES100
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetScienceTimes100}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETSCORE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetScore}}<b>(</b>'''bool''' arg0 = nil, '''bool''' winner = nil<b>)</b></code>
<!-- 
GETSCOREFROMCITIES
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetScoreFromCities}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETSCOREFROMFUTURETECH
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetScoreFromFutureTech}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETSCOREFROMLAND
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetScoreFromLand}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETSCOREFROMPOPULATION
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetScoreFromPopulation}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETSCOREFROMTECHS
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetScoreFromTechs}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETSCOREFROMWONDERS
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetScoreFromWonders}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETSCOREHISTORY
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetScoreHistory}}<b>(</b>'''int''' turn<b>)</b></code>
<!-- 
GETSCRIPTDATA
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''string'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetScriptData}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETSEAPLOTYIELD
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetSeaPlotYield}}<b>(</b>{{Type5|YieldType}} index<b>)</b></code>
<!-- 
GETSETTLERPRODUCTIONMODIFIER
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetSettlerProductionModifier}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETSPACEPRODUCTIONMODIFIER
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetSpaceProductionModifier}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETSPECIALISTEXTRAYIELD
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetSpecialistExtraYield}}<b>(</b>{{Type5|SpecialistType}} index1, {{Type5|YieldType}} index2<b>)</b></code>
<!-- 
GETSPECIALISTPRODUCTIONMODIFIER
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>{{UnknownSignature5}}</code>
|width="100%" |<code>{{FuncLabel5|Player|GetSpecialistProductionModifier}}<!-- No arguments --></code>
<!-- 
GETSTARTINGPLOT
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>{{Type5|Plot}}</code>
|width="100%" |<code>{{FuncLabel5|Player|GetStartingPlot}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETSTATERELIGIONKEY
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''string'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetStateReligionKey}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETSTATERELIGIONNAME
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''string'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetStateReligionName}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETSTRIKETURNS
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetStrikeTurns}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETTEAM
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>{{Type5|PlayerID}}</code>
|width="100%" |<code>{{FuncLabel5|Player|GetTeam}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETTECHSCORE
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetTechScore}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETTOTALFAITHPERTURN
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''unknown'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetTotalFaithPerTurn}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETTOTALJONSCULTUREPERTURN
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetTotalJONSCulturePerTurn}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETTOTALLAND
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetTotalLand}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETTOTALLANDSCORED
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetTotalLandScored}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETTOTALPOPULATION
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetTotalPopulation}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETTOTALTIMEPLAYED
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetTotalTimePlayed}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETTRADEROUTEGOLDMODIFIER
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetTradeRouteGoldModifier}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETTRAITCITYSTATECOMBATMODIFIER
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetTraitCityStateCombatModifier}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETTRAITCITYUNHAPPINESSMOD
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetTraitCityUnhappinessMod}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETTRAITGOLDENAGECOMBATMODIFIER
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetTraitGoldenAgeCombatModifier}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETTRAITGREATGENERALEXTRABONUS
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetTraitGreatGeneralExtraBonus}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETTRAITGREATSCIENTISTRATEMODIFIER
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetTraitGreatScientistRateModifier}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETTRAITPOPUNHAPPINESSMOD
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetTraitPopUnhappinessMod}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETTURNLASTPLEDGEBROKENBYMAJOR
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetTurnLastPledgeBrokenByMajor}}<b>(</b>{{Type5|PlayerID}} activePlayer<b>)</b></code>
<!-- 
GETTURNLASTPLEDGEDPROTECTIONBYMAJOR
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetTurnLastPledgedProtectionByMajor}}<b>(</b>{{Type5|PlayerID}} activePlayer<b>)</b></code>
<!-- 
GETTURNSSINCEPLAYERBULLIEDPROTECTEDMINOR
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>{{UnknownSignature5}}</code>
|width="100%" |<code>{{FuncLabel5|Player|GetTurnsSincePlayerBulliedProtectedMinor}}<!-- No arguments --></code>
<!-- 
GETTURNSSINCETHREATENEDANNOUNCEMENT
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>{{UnknownSignature5}}</code>
|width="100%" |<code>{{FuncLabel5|Player|GetTurnsSinceThreatenedAnnouncement}}<!-- No arguments --></code>
<!-- 
GETTURNSSINCETHREATENEDBYBARBARIANS
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetTurnsSinceThreatenedByBarbarians}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETUNHAPPINESS
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetUnhappiness}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETUNHAPPINESSFORECAST
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetUnhappinessForecast}}<b>(</b>{{Type5|City}} newCity, {{Type5|City}} newCity<b>)</b></code>
<!-- 
GETUNHAPPINESSFROMCAPTUREDCITYCOUNT
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetUnhappinessFromCapturedCityCount}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETUNHAPPINESSFROMCITYCOUNT
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetUnhappinessFromCityCount}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETUNHAPPINESSFROMCITYFORUI
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetUnhappinessFromCityForUI}}<b>(</b>{{Type5|City}} city<b>)</b></code>
<!-- 
GETUNHAPPINESSFROMCITYPOPULATION
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetUnhappinessFromCityPopulation}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETUNHAPPINESSFROMCITYSPECIALISTS
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetUnhappinessFromCitySpecialists}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETUNHAPPINESSFROMOCCUPIEDCITIES
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetUnhappinessFromOccupiedCities}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETUNHAPPINESSFROMPUPPETCITYPOPULATION
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetUnhappinessFromPuppetCityPopulation}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETUNHAPPINESSFROMUNITS
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetUnhappinessFromUnits}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETUNHAPPINESSMOD
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetUnhappinessMod}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETUNIMPROVEDAVAILABLELUXURYRESOURCE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''unknown'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetUnimprovedAvailableLuxuryResource}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETUNITBAKTUN
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetUnitBaktun}}<b>(</b>{{Type5|UnitType}} arg0<b>)</b></code>
<!-- 
GETUNITBYID
-->
|-
{{FuncInfos5|yes  |yes  |yes|<!-- No comment -->}}
|align="right"  |<code>{{Type5|Unit}}</code>
|width="100%" |<code>{{FuncLabel5|Player|GetUnitByID}}<b>(</b>{{Type5|UnitID}} unit<b>)</b></code>
<!-- 
GETUNITCLASSCOUNT
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetUnitClassCount}}<b>(</b>{{Type5|UnitClassType}} index<b>)</b></code>
<!-- 
GETUNITCLASSCOUNTPLUSMAKING
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetUnitClassCountPlusMaking}}<b>(</b>{{Type5|UnitClassType}} index<b>)</b></code>
<!-- 
GETUNITCLASSMAKING
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetUnitClassMaking}}<b>(</b>{{Type5|UnitClassType}} index<b>)</b></code>
<!-- 
GETUNITPRODUCTIONMAINTENANCEMOD
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetUnitProductionMaintenanceMod}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETUNITPRODUCTIONMODIFIER
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>{{UnknownSignature5}}</code>
|width="100%" |<code>{{FuncLabel5|Player|GetUnitProductionModifier}}<!-- No arguments --></code>
<!-- 
GETUNITPRODUCTIONNEEDED
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetUnitProductionNeeded}}<b>(</b>{{Type5|UnitType}} index<b>)</b></code>
<!-- 
GETVICTORYDISPUTELEVEL
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetVictoryDisputeLevel}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETVOTES
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetVotes}}<b>(</b>{{Type5|VoteType}} vote, {{Type5|VoteSourceType}} voteSource<b>)</b></code>
<!-- 
GETWARMONGERTHREAT
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>{{Type5|ThreatType}}</code>
|width="100%" |<code>{{FuncLabel5|Player|GetWarmongerThreat}}<b>(</b>{{Type5|PlayerID}} activePlayer<b>)</b></code>
<!-- 
GETWEDECLAREDWARONFRIENDCOUNT
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetWeDeclaredWarOnFriendCount}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETWEDENOUNCEDFRIENDCOUNT
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetWeDenouncedFriendCount}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETWONDERDISPUTELEVEL
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>{{Type5|DisputeLevelType}}</code>
|width="100%" |<code>{{FuncLabel5|Player|GetWonderDisputeLevel}}<b>(</b>{{Type5|PlayerID}} activePlayer<b>)</b></code>
<!-- 
GETWONDERPRODUCTIONMODIFIER
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetWonderProductionModifier}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETWONDERSSCORE
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetWondersScore}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETWORKERSPEEDMODIFIER
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetWorkerSpeedModifier}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETWORSTENEMYNAME
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''string'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetWorstEnemyName}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETYIELDRATEMODIFIER
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GetYieldRateModifier}}<b>(</b>{{Type5|YieldType}} index<b>)</b></code>
<!-- 
GREATADMIRALTHRESHOLD
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GreatAdmiralThreshold}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GREATGENERALTHRESHOLD
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|GreatGeneralThreshold}}<b>(</b>'''bool''' military<b>)</b></code>
|}

==H==
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
HASBUSYMOVINGUNIT
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Player|HasBusyMovingUnit}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
HASBUSYUNIT
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Player|HasBusyUnit}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
HASCREATEDPANTHEON
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|HasCreatedPantheon}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
HASCREATEDRELIGION
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|HasCreatedReligion}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
HASOTHERSRELIGIONINMOSTCITIES
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>{{UnknownSignature5}}</code>
|width="100%" |<code>{{FuncLabel5|Player|HasOthersReligionInMostCities}}<!-- No arguments --></code>
<!-- 
HASPOLICY
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|HasPolicy}}<b>(</b>{{Type5|PolicyType}} policy<b>)</b></code>
<!-- 
HASREADYUNIT
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Player|HasReadyUnit}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
HASRECEIVEDNETTURNCOMPLETE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|HasReceivedNetTurnComplete}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
HASRECENTINTRIGUEABOUT
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|HasRecentIntrigueAbout}}<b>(</b>{{Type5|PlayerID}} player<b>)</b></code>
<!-- 
HASRELIGIONINMOSTCITIES
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Player|HasReligionInMostCities}}<b>(</b>{{Type5|ReligionType}} religion<b>)</b></code>
<!-- 
HASSPYESTABLISHEDSURVEILLANCE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Player|HasSpyEstablishedSurveillance}}<b>(</b>'''unknown''' arg0<b>)</b></code>
|}

==I==
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
INITCITY
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>{{Type5|City}}</code>
|width="100%" |<code>{{FuncLabel5|Player|InitCity}}<b>(</b>'''int''' x, '''int''' y, '''bool''' bumpUnits = true<b>)</b></code>
<!-- 
INITUNIT
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>{{Type5|Unit}}</code>
|width="100%" |<code>{{FuncLabel5|Player|InitUnit}}<b>(</b>{{Type5|UnitType}} unit, {{Type5|ResourceType}} x, {{Type5|ResourceType}} y, {{Type5|UnitAIType}} unitAI = NO_UNITAI, {{Type5|DirectionType}} facingDirection = NO_DIRECTION<b>)</b></code>
<!-- 
ISABLETOANNEXCITYSTATES
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|IsAbleToAnnexCityStates}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ISALIVE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|IsAlive}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ISALLIES
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Player|IsAllies}}<b>(</b>{{Type5|PlayerID}} major<b>)</b></code>
<!-- 
ISALWAYSSEEBARBCAMPS
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Player|IsAlwaysSeeBarbCamps}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ISANARCHY
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Player|IsAnarchy}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ISANGRYABOUTPROTECTEDMINORATTACKED
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>{{UnknownSignature5}}</code>
|width="100%" |<code>{{FuncLabel5|Player|IsAngryAboutProtectedMinorAttacked}}<!-- No arguments --></code>
<!-- 
ISANGRYABOUTPROTECTEDMINORBULLIED
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>{{UnknownSignature5}}</code>
|width="100%" |<code>{{FuncLabel5|Player|IsAngryAboutProtectedMinorBullied}}<!-- No arguments --></code>
<!-- 
ISANGRYABOUTPROTECTEDMINORKILLED
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>{{UnknownSignature5}}</code>
|width="100%" |<code>{{FuncLabel5|Player|IsAngryAboutProtectedMinorKilled}}<!-- No arguments --></code>
<!-- 
ISANGRYABOUTSIDEDWITHTHEIRPROTECTEDMINOR
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>{{UnknownSignature5}}</code>
|width="100%" |<code>{{FuncLabel5|Player|IsAngryAboutSidedWithTheirProtectedMinor}}<!-- No arguments --></code>
<!-- 
ISANYGOODYPLOTACCESSIBLE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Player|IsAnyGoodyPlotAccessible}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ISANYPLOTIMPROVED
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Player|IsAnyPlotImproved}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ISBARBARIAN
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Player|IsBarbarian}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ISBUILDBLOCKEDBYFEATURE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Player|IsBuildBlockedByFeature}}<b>(</b>{{Type5|BuildActionType}} build, {{Type5|FeatureType}} feature<b>)</b></code>
<!-- 
ISBUILDINGCLASSMAXEDOUT
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Player|IsBuildingClassMaxedOut}}<b>(</b>{{Type5|BuildingClassType}} buildingClass, '''int''' extra<b>)</b></code>
<!-- 
ISBUILDINGFREE
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Player|IsBuildingFree}}<b>(</b>{{Type5|BuildingType}} building<b>)</b></code>
<!-- 
ISCANHURRY
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Player|IsCanHurry}}<b>(</b>{{Type5|HurryType}} index<b>)</b></code>
<!-- 
ISCANPURCHASEANYCITY
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|IsCanPurchaseAnyCity}}<b>(</b>'''bool''' arg0, '''bool''' arg1, {{Type5|UnitType}} arg2, {{Type5|BuildingType}} arg3, {{Type5|YieldType}} arg4<b>)</b></code>
<!-- 
ISCAPITALCAPTUREDBY
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Player|IsCapitalCapturedBy}}<b>(</b>{{Type5|PlayerID}} activePlayer<b>)</b></code>
<!-- 
ISCAPITALCONNECTEDTOCITY
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|IsCapitalConnectedToCity}}<b>(</b>{{Type5|City}} city<b>)</b></code>
<!-- 
ISCURRENTRESEARCHREPEAT
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Player|IsCurrentResearchRepeat}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ISDEMANDEVERMADE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Player|IsDemandEverMade}}<b>(</b>{{Type5|PlayerID}} activePlayer<b>)</b></code>
<!-- 
ISDENOUNCEDPLAYER
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Player|IsDenouncedPlayer}}<b>(</b>{{Type5|PlayerID}} otherPlayer<b>)</b></code>
<!-- 
ISDENOUNCINGPLAYER
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Player|IsDenouncingPlayer}}<b>(</b>{{Type5|PlayerID}} player<b>)</b></code>
<!-- 
ISDOF
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Player|IsDoF}}<b>(</b>{{Type5|PlayerID}} otherPlayer<b>)</b></code>
<!-- 
ISDOFMESSAGETOOSOON
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Player|IsDoFMessageTooSoon}}<b>(</b>{{Type5|PlayerID}} activePlayer<b>)</b></code>
<!-- 
ISDONTSETTLEMESSAGETOOSOON
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Player|IsDontSettleMessageTooSoon}}<b>(</b>{{Type5|PlayerID}} withPlayer<b>)</b></code>
<!-- 
ISEMPIRESUPERUNHAPPY
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Player|IsEmpireSuperUnhappy}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ISEMPIREUNHAPPY
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Player|IsEmpireUnhappy}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ISEMPIREVERYUNHAPPY
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|IsEmpireVeryUnhappy}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ISEVERALIVE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|IsEverAlive}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ISEXTENDEDGAME
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Player|IsExtendedGame}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ISFOUNDEDFIRSTCITY
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Player|IsFoundedFirstCity}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ISFREEMAYAGREATPERSONCHOICE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Player|IsFreeMayaGreatPersonChoice}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ISFREEPROMOTION
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>{{UnknownSignature5}}</code>
|width="100%" |<code>{{FuncLabel5|Player|IsFreePromotion}}<!-- No arguments --></code>
<!-- 
ISFRIENDDECLAREDWARONUS
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|IsFriendDeclaredWarOnUs}}<b>(</b>{{Type5|PlayerID}} activePlayer<b>)</b></code>
<!-- 
ISFRIENDDENOUNCEDUS
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|IsFriendDenouncedUs}}<b>(</b>{{Type5|PlayerID}} activePlayer<b>)</b></code>
<!-- 
ISFRIENDS
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|IsFriends}}<b>(</b>{{Type5|PlayerID}} major = nil<b>)</b></code>
<!-- 
ISFULLMEMBER
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Player|IsFullMember}}<b>(</b>{{Type5|VoteSourceType}} voteSource<b>)</b></code>
<!-- 
ISGAVEASSISTANCETO
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Player|IsGaveAssistanceTo}}<b>(</b>{{Type5|PlayerID}} activePlayer<b>)</b></code>
<!-- 
ISGOLDENAGE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|IsGoldenAge}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ISHALFSPECIALISTUNHAPPINESS
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Player|IsHalfSpecialistUnhappiness}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ISHASACCESSTOHURRY
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Player|IsHasAccessToHurry}}<b>(</b>{{Type5|HurryType}} index<b>)</b></code>
<!-- 
ISHASLOSTCAPITAL
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|IsHasLostCapital}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ISHASPAIDTRIBUTETO
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Player|IsHasPaidTributeTo}}<b>(</b>{{Type5|PlayerID}} activePlayer<b>)</b></code>
<!-- 
ISHASPLAYERBULLIEDPROTECTEDMINOR
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>{{UnknownSignature5}}</code>
|width="100%" |<code>{{FuncLabel5|Player|IsHasPlayerBulliedProtectedMinor}}<!-- No arguments --></code>
<!-- 
ISHUMAN
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|IsHuman}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ISLIBERATEDCAPITAL
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Player|IsLiberatedCapital}}<b>(</b>{{Type5|PlayerID}} activePlayer<b>)</b></code>
<!-- 
ISLIBERATEDCITY
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Player|IsLiberatedCity}}<b>(</b>{{Type5|PlayerID}} activePlayer<b>)</b></code>
<!-- 
ISLOYALMEMBER
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Player|IsLoyalMember}}<b>(</b>{{Type5|PlayerID}} minor<b>)</b></code>
<!-- 
ISMILITARYFOODPRODUCTION
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Player|IsMilitaryFoodProduction}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ISMINORCIV
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|IsMinorCiv}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ISMINORCIVACTIVEQUESTFORPLAYER
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Player|IsMinorCivActiveQuestForPlayer}}<b>(</b>{{Type5|PlayerID}} major, {{Type5|MinorCivQuestType}} type<b>)</b></code>
<!-- 
ISMINORCIVCONTESTLEADER
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Player|IsMinorCivContestLeader}}<b>(</b>{{Type5|PlayerID}} major, {{Type5|MinorCivQuestType}} arg1<b>)</b></code>
<!-- 
ISMINORCIVHASUNIQUEUNIT
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Player|IsMinorCivHasUniqueUnit}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ISMINORCIVROUTEESTABLISHEDWITHMAJOR
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Player|IsMinorCivRouteEstablishedWithMajor}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ISMINORCIVUNITSPAWNINGDISABLED
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Player|IsMinorCivUnitSpawningDisabled}}<b>(</b>{{Type5|PlayerID}} activePlayer<b>)</b></code>
<!-- 
ISMINORPERMANENTWAR
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Player|IsMinorPermanentWar}}<b>(</b>{{Type5|TeamID}} activeTeam<b>)</b></code>
<!-- 
ISMINORWARQUESTWITHMAJORACTIVE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Player|IsMinorWarQuestWithMajorActive}}<b>(</b>{{Type5|PlayerID}} playerLoop = nil<b>)</b></code>
<!-- 
ISNORESEARCHAVAILABLE
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Player|IsNoResearchAvailable}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ISNUKEDBY
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Player|IsNukedBy}}<b>(</b>{{Type5|PlayerID}} activePlayer<b>)</b></code>
<!-- 
ISOPTION
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Player|IsOption}}<b>(</b>{{Type5|PlayerOptionType}} index<b>)</b></code>
<!-- 
ISPEACEBLOCKED
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Player|IsPeaceBlocked}}<b>(</b>{{Type5|TeamID}} activeTeam<b>)</b></code>
<!-- 
ISPLAYABLE
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Player|IsPlayable}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ISPLAYERBROKENATTACKCITYSTATEPROMISE
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>{{UnknownSignature5}}</code>
|width="100%" |<code>{{FuncLabel5|Player|IsPlayerBrokenAttackCityStatePromise}}<!-- No arguments --></code>
<!-- 
ISPLAYERBROKENBORDERPROMISE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Player|IsPlayerBrokenBorderPromise}}<b>(</b>{{Type5|PlayerID}} activePlayer<b>)</b></code>
<!-- 
ISPLAYERBROKENBULLYCITYSTATEPROMISE
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>{{UnknownSignature5}}</code>
|width="100%" |<code>{{FuncLabel5|Player|IsPlayerBrokenBullyCityStatePromise}}<!-- No arguments --></code>
<!-- 
ISPLAYERBROKENCITYSTATEPROMISE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Player|IsPlayerBrokenCityStatePromise}}<b>(</b>{{Type5|PlayerID}} activePlayer<b>)</b></code>
<!-- 
ISPLAYERBROKENCOOPWARPROMISE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Player|IsPlayerBrokenCoopWarPromise}}<b>(</b>{{Type5|PlayerID}} activePlayer<b>)</b></code>
<!-- 
ISPLAYERBROKENEXPANSIONPROMISE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Player|IsPlayerBrokenExpansionPromise}}<b>(</b>{{Type5|PlayerID}} activePlayer<b>)</b></code>
<!-- 
ISPLAYERBROKENMILITARYPROMISE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Player|IsPlayerBrokenMilitaryPromise}}<b>(</b>{{Type5|PlayerID}} activePlayer<b>)</b></code>
<!-- 
ISPLAYERBROKENNOCONVERTPROMISE
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>{{UnknownSignature5}}</code>
|width="100%" |<code>{{FuncLabel5|Player|IsPlayerBrokenNoConvertPromise}}<!-- No arguments --></code>
<!-- 
ISPLAYERBROKENSPYPROMISE
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>{{UnknownSignature5}}</code>
|width="100%" |<code>{{FuncLabel5|Player|IsPlayerBrokenSpyPromise}}<!-- No arguments --></code>
<!-- 
ISPLAYERDENOUNCEDENEMY
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Player|IsPlayerDenouncedEnemy}}<b>(</b>{{Type5|PlayerID}} otherPlayer<b>)</b></code>
<!-- 
ISPLAYERDENOUNCEDFRIEND
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Player|IsPlayerDenouncedFriend}}<b>(</b>{{Type5|PlayerID}} activePlayer<b>)</b></code>
<!-- 
ISPLAYERDOFWITHANYENEMY
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Player|IsPlayerDoFwithAnyEnemy}}<b>(</b>{{Type5|PlayerID}} activePlayer<b>)</b></code>
<!-- 
ISPLAYERDOFWITHANYFRIEND
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Player|IsPlayerDoFwithAnyFriend}}<b>(</b>{{Type5|PlayerID}} otherPlayer<b>)</b></code>
<!-- 
ISPLAYERFORGIVENFORSPYING
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>{{UnknownSignature5}}</code>
|width="100%" |<code>{{FuncLabel5|Player|IsPlayerForgivenForSpying}}<!-- No arguments --></code>
<!-- 
ISPLAYERHASOPENBORDERS
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Player|IsPlayerHasOpenBorders}}<b>(</b>{{Type5|PlayerID}} major<b>)</b></code>
<!-- 
ISPLAYERHASOPENBORDERSAUTOMATICALLY
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Player|IsPlayerHasOpenBordersAutomatically}}<b>(</b>{{Type5|PlayerID}} major<b>)</b></code>
<!-- 
ISPLAYERIGNOREDATTACKCITYSTATEPROMISE
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>{{UnknownSignature5}}</code>
|width="100%" |<code>{{FuncLabel5|Player|IsPlayerIgnoredAttackCityStatePromise}}<!-- No arguments --></code>
<!-- 
ISPLAYERIGNOREDBORDERPROMISE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Player|IsPlayerIgnoredBorderPromise}}<b>(</b>{{Type5|PlayerID}} activePlayer<b>)</b></code>
<!-- 
ISPLAYERIGNOREDBULLYCITYSTATEPROMISE
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>{{UnknownSignature5}}</code>
|width="100%" |<code>{{FuncLabel5|Player|IsPlayerIgnoredBullyCityStatePromise}}<!-- No arguments --></code>
<!-- 
ISPLAYERIGNOREDCITYSTATEPROMISE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Player|IsPlayerIgnoredCityStatePromise}}<b>(</b>{{Type5|PlayerID}} activePlayer<b>)</b></code>
<!-- 
ISPLAYERIGNOREDEXPANSIONPROMISE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Player|IsPlayerIgnoredExpansionPromise}}<b>(</b>{{Type5|PlayerID}} activePlayer<b>)</b></code>
<!-- 
ISPLAYERIGNOREDMILITARYPROMISE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Player|IsPlayerIgnoredMilitaryPromise}}<b>(</b>{{Type5|PlayerID}} activePlayer<b>)</b></code>
<!-- 
ISPLAYERIGNOREDNOCONVERTPROMISE
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>{{UnknownSignature5}}</code>
|width="100%" |<code>{{FuncLabel5|Player|IsPlayerIgnoredNoConvertPromise}}<!-- No arguments --></code>
<!-- 
ISPLAYERIGNOREDSPYPROMISE
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>{{UnknownSignature5}}</code>
|width="100%" |<code>{{FuncLabel5|Player|IsPlayerIgnoredSpyPromise}}<!-- No arguments --></code>
<!-- 
ISPLAYERNOSETTLEREQUESTEVERASKED
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Player|IsPlayerNoSettleRequestEverAsked}}<b>(</b>{{Type5|PlayerID}} activePlayer<b>)</b></code>
<!-- 
ISPLAYERRECKLESSEXPANDER
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Player|IsPlayerRecklessExpander}}<b>(</b>{{Type5|PlayerID}} activePlayer<b>)</b></code>
<!-- 
ISPLAYERSTOPSPYINGREQUESTEVERASKED
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>{{UnknownSignature5}}</code>
|width="100%" |<code>{{FuncLabel5|Player|IsPlayerStopSpyingRequestEverAsked}}<!-- No arguments --></code>
<!-- 
ISPOLICYBLOCKED
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Player|IsPolicyBlocked}}<b>(</b>{{Type5|PolicyType}} i<b>)</b></code>
<!-- 
ISPOLICYBRANCHBLOCKED
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Player|IsPolicyBranchBlocked}}<b>(</b>{{Type5|PolicyBranchType}} policyBranchIndex<b>)</b></code>
<!-- 
ISPOLICYBRANCHFINISHED
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Player|IsPolicyBranchFinished}}<b>(</b>{{Type5|PolicyBranchType}} arg0<b>)</b></code>
<!-- 
ISPOLICYBRANCHUNLOCKED
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|IsPolicyBranchUnlocked}}<b>(</b>{{Type5|PolicyBranchType}} policyBranchIndex<b>)</b></code>
<!-- 
ISPRODUCTIONMAXEDBUILDINGCLASS
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Player|IsProductionMaxedBuildingClass}}<b>(</b>{{Type5|BuildingClassType}} buildingClass, '''bool''' acquireCity<b>)</b></code>
<!-- 
ISPRODUCTIONMAXEDPROJECT
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Player|IsProductionMaxedProject}}<b>(</b>{{Type5|ProjectType}} project<b>)</b></code>
<!-- 
ISPRODUCTIONMAXEDUNITCLASS
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Player|IsProductionMaxedUnitClass}}<b>(</b>{{Type5|UnitClassType}} unitClass<b>)</b></code>
<!-- 
ISPROTECTEDBYMAJOR
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Player|IsProtectedByMajor}}<b>(</b>{{Type5|PlayerID}} activePlayer<b>)</b></code>
<!-- 
ISPROTECTINGMINOR
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|IsProtectingMinor}}<b>(</b>{{Type5|PlayerID}} player<b>)</b></code>
<!-- 
ISRESEARCH
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Player|IsResearch}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ISRESEARCHINGTECH
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Player|IsResearchingTech}}<b>(</b>'''int''' index<b>)</b></code>
<!-- 
ISSTOPSPYINGMESSAGETOOSOON
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Player|IsStopSpyingMessageTooSoon}}<b>(</b>{{Type5|PlayerID}} activePlayer<b>)</b></code>
<!-- 
ISSTRIKE
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Player|IsStrike}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ISTHREATENINGBARBARIANSEVENTACTIVEFORPLAYER
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Player|IsThreateningBarbariansEventActiveForPlayer}}<b>(</b>{{Type5|PlayerID}} major<b>)</b></code>
<!-- 
ISTRAITBONUSRELIGIOUSBELIEF
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Player|IsTraitBonusReligiousBelief}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ISTURNACTIVE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|IsTurnActive}}<b>(</b>'''unknown''' void<b>)</b></code>
<!-- 
ISUNITCLASSMAXEDOUT
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Player|IsUnitClassMaxedOut}}<b>(</b>{{Type5|UnitClassType}} index, '''int''' extra<b>)</b></code>
<!-- 
ISUNTRUSTWORTHYFRIEND
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>{{UnknownSignature5}}</code>
|width="100%" |<code>{{FuncLabel5|Player|IsUntrustworthyFriend}}<!-- No arguments --></code>
<!-- 
ISUSINGMAYACALENDAR
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Player|IsUsingMayaCalendar}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ISVOTINGMEMBER
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Player|IsVotingMember}}<b>(</b>{{Type5|VoteSourceType}} voteSource<b>)</b></code>
<!-- 
ISWHITEFLAG
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Player|IsWhiteFlag}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ISWILLACCEPTPEACEWITHPLAYER
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Player|IsWillAcceptPeaceWithPlayer}}<b>(</b>{{Type5|PlayerID}} player<b>)</b></code>
|}

==K==
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
KILLCITIES
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>{{UnknownSignature5}}</code>
|width="100%" |<code>{{FuncLabel5|Player|KillCities}}<!-- No arguments --></code>
<!-- 
KILLUNITS
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>{{UnknownSignature5}}</code>
|width="100%" |<code>{{FuncLabel5|Player|KillUnits}}<!-- No arguments --></code>
|}

==P==
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
POPRESEARCH
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Player|PopResearch}}<b>(</b>{{Type5|TechType}} tech<b>)</b></code>
<!-- 
PUSHRESEARCH
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Player|PushResearch}}<b>(</b>'''int''' index, '''bool''' clear<b>)</b></code>
|}

==R==
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
RAZE
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Player|Raze}}<b>(</b>{{Type5|City}} city<b>)</b></code>
<!-- 
RECEIVEGOODY
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Player|ReceiveGoody}}<b>(</b>{{Type5|Plot}} plot, {{Type5|GoodyType}} goody, {{Type5|Unit}} unit<b>)</b></code>
<!-- 
REMOVEBUILDINGCLASS
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Player|RemoveBuildingClass}}<b>(</b>{{Type5|BuildingClassType}} buildingClass<b>)</b></code>
|}

==S==
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
SETADVANCEDSTARTPOINTS
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Player|SetAdvancedStartPoints}}<b>(</b>'''int''' newValue<b>)</b></code>
<!-- 
SETALWAYSSEEBARBCAMPSCOUNT
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>{{UnknownSignature5}}</code>
|width="100%" |<code>{{FuncLabel5|Player|SetAlwaysSeeBarbCampsCount}}<!-- No arguments --></code>
<!-- 
SETANARCHYNUMTURNS
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|SetAnarchyNumTurns}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
SETBARBARIANCOMBATBONUS
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>{{UnknownSignature5}}</code>
|width="100%" |<code>{{FuncLabel5|Player|SetBarbarianCombatBonus}}<!-- No arguments --></code>
<!-- 
SETBASEBUILDINGGOLDMAINTENANCE
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|SetBaseBuildingGoldMaintenance}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
SETCOMBATEXPERIENCE
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Player|SetCombatExperience}}<b>(</b>'''int''' experience<b>)</b></code>
<!-- 
SETCONSCRIPTCOUNT
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Player|SetConscriptCount}}<b>(</b>'''int''' newValue<b>)</b></code>
<!-- 
SETEMBARKEDGRAPHICOVERRIDE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Player|SetEmbarkedGraphicOverride}}<b>(</b>'''string''' arg0<b>)</b></code>
<!-- 
SETFAITH
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Player|SetFaith}}<b>(</b>'''int''' arg0<b>)</b></code>
<!-- 
SETFAITHPURCHASEINDEX
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Player|SetFaithPurchaseIndex}}<b>(</b>'''int''' v2<b>)</b></code>
<!-- 
SETFAITHPURCHASETYPE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Player|SetFaithPurchaseType}}<b>(</b>{{Type5|FaithPurchaseType}} v1<b>)</b></code>
<!-- 
SETGOLD
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Player|SetGold}}<b>(</b>'''int''' newValue<b>)</b></code>
<!-- 
SETGOLDENAGEPROGRESSMETER
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>{{UnknownSignature5}}</code>
|width="100%" |<code>{{FuncLabel5|Player|SetGoldenAgeProgressMeter}}<!-- No arguments --></code>
<!-- 
SETHAPPINESS
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Player|SetHappiness}}<b>(</b>'''int''' newValue<b>)</b></code>
<!-- 
SETHAPPINESSPERGARRISONEDUNIT
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Player|SetHappinessPerGarrisonedUnit}}<b>(</b>'''int''' value<b>)</b></code>
<!-- 
SETHAPPINESSPERTRADEROUTE
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Player|SetHappinessPerTradeRoute}}<b>(</b>'''int''' value<b>)</b></code>
<!-- 
SETHASPOLICY
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Player|SetHasPolicy}}<b>(</b>{{Type5|PolicyType}} index, '''bool''' newValue<b>)</b></code>
<!-- 
SETJONSCULTURE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Player|SetJONSCulture}}<b>(</b>'''int''' newValue<b>)</b></code>
<!-- 
SETLOYALMEMBER
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Player|SetLoyalMember}}<b>(</b>{{Type5|PlayerID}} minor, '''bool''' newValue<b>)</b></code>
<!-- 
SETNAVALCOMBATEXPERIENCE
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>{{UnknownSignature5}}</code>
|width="100%" |<code>{{FuncLabel5|Player|SetNavalCombatExperience}}<!-- No arguments --></code>
<!-- 
SETNUMFAITHGREATPEOPLE
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>{{UnknownSignature5}}</code>
|width="100%" |<code>{{FuncLabel5|Player|SetNumFaithGreatPeople}}<!-- No arguments --></code>
<!-- 
SETNUMFREEGREATPEOPLE
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>{{UnknownSignature5}}</code>
|width="100%" |<code>{{FuncLabel5|Player|SetNumFreeGreatPeople}}<!-- No arguments --></code>
<!-- 
SETNUMFREEPOLICIES
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>{{UnknownSignature5}}</code>
|width="100%" |<code>{{FuncLabel5|Player|SetNumFreePolicies}}<!-- No arguments --></code>
<!-- 
SETNUMFREETECHS
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>{{UnknownSignature5}}</code>
|width="100%" |<code>{{FuncLabel5|Player|SetNumFreeTechs}}<!-- No arguments --></code>
<!-- 
SETNUMGOLDENAGES
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>{{UnknownSignature5}}</code>
|width="100%" |<code>{{FuncLabel5|Player|SetNumGoldenAges}}<!-- No arguments --></code>
<!-- 
SETNUMMAYABOOSTS
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>{{UnknownSignature5}}</code>
|width="100%" |<code>{{FuncLabel5|Player|SetNumMayaBoosts}}<!-- No arguments --></code>
<!-- 
SETNUMPLOTSBOUGHT
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Player|SetNumPlotsBought}}<b>(</b>'''int''' value<b>)</b></code>
<!-- 
SETNUMWONDERSBEATENTO
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>{{UnknownSignature5}}</code>
|width="100%" |<code>{{FuncLabel5|Player|SetNumWondersBeatenTo}}<!-- No arguments --></code>
<!-- 
SETOPTION
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Player|SetOption}}<b>(</b>{{Type5|PlayerOptionType}} index, '''bool''' newValue<b>)</b></code>
<!-- 
SETPERSONALITYTYPE
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Player|SetPersonalityType}}<b>(</b>{{Type5|MinorCivPersonalityType}} newValue<b>)</b></code>
<!-- 
SETPLAYABLE
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Player|SetPlayable}}<b>(</b>'''bool''' newValue<b>)</b></code>
<!-- 
SETPOLICYBRANCHUNLOCKED
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Player|SetPolicyBranchUnlocked}}<b>(</b>{{Type5|PolicyBranchType}} arg0, '''bool''' arg1<b>)</b></code>
<!-- 
SETREPLAYDATAVALUE
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>{{UnknownSignature5}}</code>
|width="100%" |<code>{{FuncLabel5|Player|SetReplayDataValue}}<!-- No arguments --></code>
<!-- 
SETRESEARCHINGTECH
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Player|SetResearchingTech}}<b>(</b>{{Type5|TechType}} index, '''bool''' newValue<b>)</b></code>
<!-- 
SETSCRIPTDATA
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Player|SetScriptData}}<b>(</b>'''string''' newValue<b>)</b></code>
<!-- 
SETSTARTINGPLOT
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Player|SetStartingPlot}}<b>(</b>{{Type5|Plot}} plot<b>)</b></code>
<!-- 
SPECIALISTYIELD
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|SpecialistYield}}<b>(</b>{{Type5|SpecialistType}} specialist, {{Type5|YieldType}} yield<b>)</b></code>
<!-- 
STOPTRADINGWITHTEAM
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Player|StopTradingWithTeam}}<b>(</b>{{Type5|TeamID}} team<b>)</b></code>
|}

==U==
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
UNITS
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>iterator({{Type5|Unit}})</code>
|width="100%" |<code>{{FuncLabel5|Player|Units}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
UNITSGOLDENAGECAPABLE
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|UnitsGoldenAgeCapable}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
UNITSGOLDENAGEREADY
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|UnitsGoldenAgeReady}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
UNITSREQUIREDFORGOLDENAGE
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Player|UnitsRequiredForGoldenAge}}<b>(</b><!-- No arguments --><b>)</b></code>
|}

==W==
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
WASRESURRECTEDBY
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>{{UnknownSignature5}}</code>
|width="100%" |<code>{{FuncLabel5|Player|WasResurrectedBy}}<!-- No arguments --></code>
<!-- 
WASRESURRECTEDTHISTURNBY
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Player|WasResurrectedThisTurnBy}}<b>(</b>{{Type5|PlayerID}} player<b>)</b></code>
|}


=Used by=
{|cellspacing="4" cellpadding="0" width="100%" style="background-color:#F0F0F0"
<!-- 
GETCITYSTATESTATUS
-->
|-
|align="right" width="200" |<code>'''string'''</code>
|style="padding-left:6px" |<code>{{Func5|GetCityStateStatus}}<b>(</b>{{Type5|Player}} player, {{Type5|PlayerID}} forPlayer, '''int''' war<b>)</b></code>
<!-- 
GETLOCALIZEDLEADERTITLE
-->
|-
|align="right" width="200" |<code>'''string'''</code>
|style="padding-left:6px" |<code>{{Type5|GameplayUtilities}}.{{Func5|GameplayUtilities|GetLocalizedLeaderTitle}}<b>(</b>{{Type5|Player}} player<b>)</b></code>
<!-- 
GETPLAYERVISIBLEPLOT
-->
|-
|align="right" width="200" |<code>'''unknown'''</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|GetPlayerVisiblePlot}}<b>(</b>{{Type5|Player}} player<b>)</b></code>
|}




{{Civ5 API Footer}}
[[Category:Civ5 Types|Player]]