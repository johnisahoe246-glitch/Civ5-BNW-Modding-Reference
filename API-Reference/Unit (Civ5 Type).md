{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



=Instance Methods=
Methods are functions that belong to an object. Instance methods are invoked through a '''colon''', as in <code>caller:SomeMethod(&lt;args&gt;)</code>, where ''caller'' is an instance of Unit.<br/>
A colon implictly passes the caller object as the first argument. That is, the former call is equivalent to this one: <code>caller.SomeMethod(caller, &lt;args&gt;)</code>
==A==
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
AIRSWEEPCOMBATMOD
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|AirSweepCombatMod}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
AT
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|At}}<b>(</b>'''int''' x, '''int''' y<b>)</b></code>
<!-- 
ATPLOT
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|AtPlot}}<b>(</b>{{Type5|Plot}} plot<b>)</b></code>
<!-- 
ATTACKFORTIFIEDMODIFIER
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|AttackFortifiedModifier}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ATTACKWOUNDEDMODIFIER
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|AttackWoundedModifier}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ATTACKXPVALUE
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|AttackXPValue}}<b>(</b><!-- No arguments --><b>)</b></code>
|}

==C==
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
CANACQUIREPROMOTION
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|CanAcquirePromotion}}<b>(</b>{{Type5|PromotionType}} promotion<b>)</b></code>
<!-- 
CANACQUIREPROMOTIONANY
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|CanAcquirePromotionAny}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
CANAIRATTACK
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|CanAirAttack}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
CANAIRDEFEND
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|CanAirDefend}}<b>(</b>{{Type5|Plot}} plot<b>)</b></code>
<!-- 
CANAIRLIFT
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|CanAirlift}}<b>(</b>{{Type5|Plot}} plot<b>)</b></code>
<!-- 
CANAIRLIFTAT
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|CanAirliftAt}}<b>(</b>{{Type5|Plot}} plot, '''int''' x, '''int''' y<b>)</b></code>
<!-- 
CANAIRPATROL
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|CanAirPatrol}}<b>(</b>{{Type5|Plot}} plot<b>)</b></code>
<!-- 
CANAUTOMATE
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|CanAutomate}}<b>(</b>{{Type5|AutomateType}} automate<b>)</b></code>
<!-- 
CANBUILD
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|CanBuild}}<b>(</b>{{Type5|Plot}} plot, {{Type5|BuildActionType}} build, '''bool''' testVisible = false, '''bool''' testGold = true<b>)</b></code>
<!-- 
CANBUILDROUTE
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|CanBuildRoute}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
CANBUILDSPACESHIP
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|CanBuildSpaceship}}<b>(</b>{{Type5|Plot}} plot, '''bool''' visible<b>)</b></code>
<!-- 
CANCARGOALLMOVE
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|CanCargoAllMove}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
CANCOEXISTWITHENEMYUNIT
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|CanCoexistWithEnemyUnit}}<b>(</b>{{Type5|TeamID}} team<b>)</b></code>
<!-- 
CANCONSTRUCT
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|CanConstruct}}<b>(</b>{{Type5|Plot}} plot, {{Type5|BuildingType}} building<b>)</b></code>
<!-- 
CANDISCOVER
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|CanDiscover}}<b>(</b>{{Type5|Plot}} plot<b>)</b></code>
<!-- 
CANDISEMBARK
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|CanDisembark}}<b>(</b>{{Type5|Plot}} plot<b>)</b></code>
<!-- 
CANDISEMBARKONTO
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|CanDisembarkOnto}}<b>(</b>{{Type5|Plot}} plot<b>)</b></code>
<!-- 
CANDISTANCEGIFT
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|CanDistanceGift}}<b>(</b>{{Type5|TaskType}} toPlayer<b>)</b></code>
<!-- 
CANDOCOMMAND
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|CanDoCommand}}<b>(</b>{{Type5|CommandType}} command, '''int''' data1, '''int''' data2, '''bool''' testVisible = false, '''bool''' testBusy = true<b>)</b></code>
<!-- 
CANEMBARK
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|CanEmbark}}<b>(</b>{{Type5|Plot}} plot<b>)</b></code>
<!-- 
CANEMBARKONTO
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|CanEmbarkOnto}}<b>(</b>{{Type5|Plot}} plot, {{Type5|Plot}} targetPlot<b>)</b></code>
<!-- 
CANENTERTERRITORY
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|CanEnterTerritory}}<b>(</b>{{Type5|TeamID}} team, '''bool''' ignoreRightOfPassage = false, '''bool''' isCity = false<b>)</b></code>
<!-- 
CANFORTIFY
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|CanFortify}}<b>(</b>{{Type5|Plot}} plot<b>)</b></code>
<!-- 
CANFOUND
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|CanFound}}<b>(</b>{{Type5|Plot}} plot, '''bool''' testVisible = false<b>)</b></code>
<!-- 
CANGIFT
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|CanGift}}<b>(</b>'''bool''' testVisible = false, '''bool''' testTransport = false<b>)</b></code>
<!-- 
CANGIVEEXPERIENCE
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|CanGiveExperience}}<b>(</b>{{Type5|Plot}} plot<b>)</b></code>
<!-- 
CANGOLDENAGE
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|CanGoldenAge}}<b>(</b>{{Type5|Plot}} plot, '''bool''' testVisible<b>)</b></code>
<!-- 
CANHEAL
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|CanHeal}}<b>(</b>{{Type5|Plot}} plot<b>)</b></code>
<!-- 
CANHOLD
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|CanHold}}<b>(</b>{{Type5|Plot}} plot<b>)</b></code>
<!-- 
CANJOIN
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|CanJoin}}<b>(</b>{{Type5|Plot}} plot, {{Type5|SpecialistType}} specialist<b>)</b></code>
<!-- 
CANLEAD
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|CanLead}}<b>(</b>{{Type5|Plot}} plot, '''int''' unitId<b>)</b></code>
<!-- 
CANLOAD
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|CanLoad}}<b>(</b>{{Type5|Plot}} plot<b>)</b></code>
<!-- 
CANLOADUNIT
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|CanLoadUnit}}<b>(</b>{{Type5|Unit}} unit, {{Type5|Plot}} plot<b>)</b></code>
<!-- 
CANMOVE
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|CanMove}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
CANMOVEALLTERRAIN
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|CanMoveAllTerrain}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
CANMOVEIMPASSABLE
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|CanMoveImpassable}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
CANMOVEORATTACKINTO
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|CanMoveOrAttackInto}}<b>(</b>{{Type5|Plot}} plot, '''bool''' declareWar = false, '''bool''' destination = false<b>)</b></code>
<!-- 
CANMOVETHROUGH
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|CanMoveThrough}}<b>(</b>{{Type5|Plot}} plot<b>)</b></code>
<!-- 
CANNUKE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|CanNuke}}<b>(</b>{{Type5|Plot}} plot<b>)</b></code>
<!-- 
CANNUKEAT
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|CanNukeAt}}<b>(</b>{{Type5|Plot}} plot, '''int''' x, '''int''' y<b>)</b></code>
<!-- 
CANPARADROP
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|CanParadrop}}<b>(</b>{{Type5|Plot}} plot, '''bool''' arg1<b>)</b></code>
<!-- 
CANPARADROPAT
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|CanParadropAt}}<b>(</b>{{Type5|Plot}} plot, '''int''' x, '''int''' y<b>)</b></code>
<!-- 
CANPILLAGE
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|CanPillage}}<b>(</b>{{Type5|Plot}} plot<b>)</b></code>
<!-- 
CANPROMOTE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|CanPromote}}<b>(</b>{{Type5|PromotionType}} promotion, '''int''' leaderUnitId<b>)</b></code>
<!-- 
CANRANGESTRIKE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|CanRangeStrike}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
CANRANGESTRIKEAT
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|CanRangeStrikeAt}}<b>(</b>'''int''' x, '''int''' y, '''bool''' arg2 = nil, '''bool''' noncombatAllowed = nil<b>)</b></code>
<!-- 
CANREBASEAT
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|CanRebaseAt}}<b>(</b>{{Type5|Plot}} sourcePlot, '''int''' targetX, '''int''' targetY<b>)</b></code>
<!-- 
CANREPAIRFLEET
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>{{UnknownSignature5}}</code>
|width="100%" |<code>{{FuncLabel5|Unit|CanRepairFleet}}<!-- No arguments --></code>
<!-- 
CANSCRAP
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|CanScrap}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
CANSENTRY
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|CanSentry}}<b>(</b>{{Type5|Plot}} plot<b>)</b></code>
<!-- 
CANSETUPFORRANGEDATTACK
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|CanSetUpForRangedAttack}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
CANSIEGE
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|CanSiege}}<b>(</b>{{Type5|TeamID}} team<b>)</b></code>
<!-- 
CANSLEEP
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|CanSleep}}<b>(</b>{{Type5|Plot}} plot<b>)</b></code>
<!-- 
CANSTARTMISSION
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|CanStartMission}}<b>(</b>'''int''' mission, '''int''' data1, '''int''' data2, {{Type5|Plot}} plot = nil, '''bool''' testVisible = false<b>)</b></code>
<!-- 
CANTRADE
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|CanTrade}}<b>(</b>{{Type5|Plot}} plot, '''bool''' testVisible<b>)</b></code>
<!-- 
CANUNLOAD
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|CanUnload}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
CANUNLOADALL
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|CanUnloadAll}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
CANUPGRADERIGHTNOW
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|CanUpgradeRightNow}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
CAPITALDEFENSEFALLOFF
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|CapitalDefenseFalloff}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
CAPITALDEFENSEMODIFIER
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|CapitalDefenseModifier}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
CARGOSPACE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|CargoSpace}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
CARGOSPACEAVAILABLE
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|CargoSpaceAvailable}}<b>(</b>{{Type5|SpecialUnitType}} specialCargo, {{Type5|DomainType}} domainCargo<b>)</b></code>
<!-- 
CHANCEFIRSTSTRIKES
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|ChanceFirstStrikes}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
CHANGECARGOSPACE
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Unit|ChangeCargoSpace}}<b>(</b>'''int''' change<b>)</b></code>
<!-- 
CHANGEDAMAGE
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Unit|ChangeDamage}}<b>(</b>'''int''' change, {{Type5|PlayerID}} player<b>)</b></code>
<!-- 
CHANGEEXPERIENCE
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|yes|<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Unit|ChangeExperience}}<b>(</b>'''int''' change, '''int''' max = -1, '''bool''' fromCombat = false, '''bool''' inBorders = false, '''bool''' updateGlobal = false<b>)</b></code>
<!-- 
CHANGELEVEL
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Unit|ChangeLevel}}<b>(</b>'''int''' change<b>)</b></code>
<!-- 
CHANGEMOVES
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Unit|ChangeMoves}}<b>(</b>'''int''' change<b>)</b></code>
<!-- 
CITYATTACKMODIFIER
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|CityAttackModifier}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
CITYDEFENSEMODIFIER
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|CityDefenseModifier}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
CONVERT
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Unit|Convert}}<b>(</b>{{Type5|Unit}} unit<b>)</b></code>
<!-- 
CURRINTERCEPTIONPROBABILITY
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|CurrInterceptionProbability}}<b>(</b><!-- No arguments --><b>)</b></code>
|}

==D==
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
DEFENSEXPVALUE
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|DefenseXPValue}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
DOCOMMAND
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Unit|DoCommand}}<b>(</b>{{Type5|CommandType}} command, '''int''' data1, '''int''' data2<b>)</b></code>
<!-- 
DOMAINCARGO
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>{{Type5|DomainType}}</code>
|width="100%" |<code>{{FuncLabel5|Unit|DomainCargo}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
DOMAINMODIFIER
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|DomainModifier}}<b>(</b>{{Type5|DomainType}} domain<b>)</b></code>
|}

==E==
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
EMBARK
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Unit|Embark}}<b>(</b>{{Type5|Plot}} plot<b>)</b></code>
<!-- 
EVASIONPROBABILITY
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|EvasionProbability}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
EXECUTESPECIALEXPLOREMOVE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Unit|ExecuteSpecialExploreMove}}<b>(</b>{{Type5|Plot}} targetPlot<b>)</b></code>
<!-- 
EXPERIENCENEEDED
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|ExperienceNeeded}}<b>(</b><!-- No arguments --><b>)</b></code>
|}

==F==
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
FEATUREATTACKMODIFIER
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|FeatureAttackModifier}}<b>(</b>{{Type5|FeatureType}} feature<b>)</b></code>
<!-- 
FEATUREDEFENSEMODIFIER
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|FeatureDefenseModifier}}<b>(</b>{{Type5|FeatureType}} feature<b>)</b></code>
<!-- 
FINISHMOVES
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>{{UnknownSignature5}}</code>
|width="100%" |<code>{{FuncLabel5|Unit|FinishMoves}}<!-- No arguments --></code>
<!-- 
FIRSTSTRIKES
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|FirstStrikes}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
FLANKATTACKMODIFIER
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|FlankAttackModifier}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
FLATMOVEMENTCOST
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|FlatMovementCost}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
FLAVORVALUE
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|FlavorValue}}<b>(</b>{{Type5|FlavorType}} flavor<b>)</b></code>
<!-- 
FORTIFYMODIFIER
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|FortifyModifier}}<b>(</b><!-- No arguments --><b>)</b></code>
|}

==G==
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
GENERATEPATH
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|GeneratePath}}<b>(</b>{{Type5|Plot}} toPlot, '''int''' flags = 0, '''bool''' reuse = false, '''unknown''' piPathTurns = nil<b>)</b></code>
<!-- 
GETACTIVITYTYPE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>{{Type5|ActivityType}}</code>
|width="100%" |<code>{{FuncLabel5|Unit|GetActivityType}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETADJACENTMODIFIER
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|GetAdjacentModifier}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETADJACENTTILEHEAL
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|GetAdjacentTileHeal}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETAIRCOMBATDAMAGE
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|GetAirCombatDamage}}<b>(</b>{{Type5|Unit}} defender<b>)</b></code>
<!-- 
GETAMPHIBCOUNT
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|GetAmphibCount}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETAREA
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>{{Type5|Area}}</code>
|width="100%" |<code>{{FuncLabel5|Unit|GetArea}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETATTACKMODIFIER
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|GetAttackModifier}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETBASECOMBATSTRENGTH
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|GetBaseCombatStrength}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETBASERANGEDCOMBATSTRENGTH
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|GetBaseRangedCombatStrength}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETBESTINTERCEPTOR
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''unknown'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|GetBestInterceptor}}<b>(</b>{{Type5|Plot}} plot<b>)</b></code>
<!-- 
GETBESTSEAPILLAGEINTERCEPTOR
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''unknown'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|GetBestSeaPillageInterceptor}}<b>(</b>{{Type5|Plot}} plot<b>)</b></code>
<!-- 
GETBLITZCOUNT
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|GetBlitzCount}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETBUILDTYPE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>{{Type5|BuildActionType}}</code>
|width="100%" |<code>{{FuncLabel5|Unit|GetBuildType}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETCAPTUREUNITTYPE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>{{Type5|UnitType}}</code>
|width="100%" |<code>{{FuncLabel5|Unit|GetCaptureUnitType}}<b>(</b>{{Type5|CivilizationType}} civilization<b>)</b></code>
<!-- 
GETCARGO
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|GetCargo}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETCIVILIZATIONTYPE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>{{Type5|CivilizationType}}</code>
|width="100%" |<code>{{FuncLabel5|Unit|GetCivilizationType}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETCOMBATDAMAGE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|GetCombatDamage}}<b>(</b>'''int''' strength, '''int''' opponentStrength, '''int''' currentDamage, '''bool''' includeRand = true, '''bool''' attackerIsCity = false, '''bool''' defenderIsCity = false<b>)</b></code>
<!-- 
GETCOMBATLIMIT
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|GetCombatLimit}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETCOMBATOWNER
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|GetCombatOwner}}<b>(</b>{{Type5|TeamID}} forTeam<b>)</b></code>
<!-- 
GETCONVERSIONSTRENGTH
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''unknown'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|GetConversionStrength}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETCURRHITPOINTS
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|GetCurrHitPoints}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETDAMAGE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|GetDamage}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETDECLAREWARRANGESTRIKE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>{{Type5|TeamID}}</code>
|width="100%" |<code>{{FuncLabel5|Unit|GetDeclareWarRangeStrike}}<b>(</b>{{Type5|Plot}} plot<b>)</b></code>
<!-- 
GETDEFENSEMODIFIER
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|GetDefenseModifier}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETDOMAINTYPE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>{{Type5|DomainType}}</code>
|width="100%" |<code>{{FuncLabel5|Unit|GetDomainType}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETDROPRANGE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|GetDropRange}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETEMBARKEDUNITDEFENSE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|GetEmbarkedUnitDefense}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETEXPERIENCE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|GetExperience}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETEXPERIENCEPERCENT
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|GetExperiencePercent}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETEXTRAATTACKFORTIFIEDMOD
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|GetExtraAttackFortifiedMod}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETEXTRAATTACKWOUNDEDMOD
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|GetExtraAttackWoundedMod}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETEXTRACHANCEFIRSTSTRIKES
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|GetExtraChanceFirstStrikes}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETEXTRACITYATTACKPERCENT
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|GetExtraCityAttackPercent}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETEXTRACITYDEFENSEPERCENT
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|GetExtraCityDefensePercent}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETEXTRACOMBATPERCENT
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|GetExtraCombatPercent}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETEXTRADOMAINMODIFIER
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|GetExtraDomainModifier}}<b>(</b>{{Type5|DomainType}} index<b>)</b></code>
<!-- 
GETEXTRAENEMYHEAL
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|GetExtraEnemyHeal}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETEXTRAEVASION
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|GetExtraEvasion}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETEXTRAFEATUREATTACKPERCENT
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|GetExtraFeatureAttackPercent}}<b>(</b>{{Type5|FeatureType}} index<b>)</b></code>
<!-- 
GETEXTRAFEATUREDEFENSEPERCENT
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|GetExtraFeatureDefensePercent}}<b>(</b>{{Type5|FeatureType}} index<b>)</b></code>
<!-- 
GETEXTRAFIRSTSTRIKES
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|GetExtraFirstStrikes}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETEXTRAFRIENDLYHEAL
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|GetExtraFriendlyHeal}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETEXTRAHILLSATTACKPERCENT
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|GetExtraHillsAttackPercent}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETEXTRAHILLSDEFENSEPERCENT
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|GetExtraHillsDefensePercent}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETEXTRAINTERCEPT
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|GetExtraIntercept}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETEXTRAMOVEDISCOUNT
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|GetExtraMoveDiscount}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETEXTRAMOVES
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|GetExtraMoves}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETEXTRANEUTRALHEAL
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|GetExtraNeutralHeal}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETEXTRAOPENATTACKPERCENT
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|GetExtraOpenAttackPercent}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETEXTRAOPENDEFENSEPERCENT
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|GetExtraOpenDefensePercent}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETEXTRAOPENRANGEDATTACKMOD
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|GetExtraOpenRangedAttackMod}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETEXTRARANGE
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|GetExtraRange}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETEXTRAROUGHATTACKPERCENT
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|GetExtraRoughAttackPercent}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETEXTRAROUGHRANGEDATTACKMOD
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|GetExtraRoughRangedAttackMod}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETEXTRATERRAINATTACKPERCENT
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|GetExtraTerrainAttackPercent}}<b>(</b>{{Type5|TerrainType}} index<b>)</b></code>
<!-- 
GETEXTRATERRAINDEFENSEPERCENT
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|GetExtraTerrainDefensePercent}}<b>(</b>{{Type5|TerrainType}} index<b>)</b></code>
<!-- 
GETEXTRAUNITCOMBATMODIFIER
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|GetExtraUnitCombatModifier}}<b>(</b>{{Type5|UnitCombatType}} index<b>)</b></code>
<!-- 
GETEXTRAVISIBILITYRANGE
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|GetExtraVisibilityRange}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETEXTRAWITHDRAWAL
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|GetExtraWithdrawal}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETFACINGDIRECTION
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|GetFacingDirection}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETFIRESUPPORTUNIT
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>{{Type5|Unit}}</code>
|width="100%" |<code>{{FuncLabel5|Unit|GetFireSupportUnit}}<b>(</b>{{Type5|PlayerID}} defender, '''int''' x, '''int''' y<b>)</b></code>
<!-- 
GETFORTIFYTURNS
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|GetFortifyTurns}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETFRIENDLYLANDSATTACKMODIFIER
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|GetFriendlyLandsAttackModifier}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETFRIENDLYLANDSMODIFIER
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|GetFriendlyLandsModifier}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETGAMETURNCREATED
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|GetGameTurnCreated}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETGARRISONEDCITY
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|GetGarrisonedCity}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETGOLDENAGETURNS
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|GetGoldenAgeTurns}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETGREATGENERALCOMBATMODIFIER
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|GetGreatGeneralCombatModifier}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETHANDICAPTYPE
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>{{Type5|HandicapType}}</code>
|width="100%" |<code>{{FuncLabel5|Unit|GetHandicapType}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETHOTKEYNUMBER
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|GetHotKeyNumber}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETID
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>{{Type5|UnitID}}</code>
|width="100%" |<code>{{FuncLabel5|Unit|GetID}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETINVISIBLETYPE
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>{{Type5|InvisibilityScopeType}}</code>
|width="100%" |<code>{{FuncLabel5|Unit|GetInvisibleType}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETKAMIKAZEPERCENT
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|GetKamikazePercent}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETLASTMOVETURN
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|GetLastMoveTurn}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETLEADERUNITTYPE
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''unknown'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|GetLeaderUnitType}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETLEVEL
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|GetLevel}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETMAJORITYRELIGIONAFTERSPREAD
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>{{Type5|ReligionType}}</code>
|width="100%" |<code>{{FuncLabel5|Unit|GetMajorityReligionAfterSpread}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETMAXATTACKSTRENGTH
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|GetMaxAttackStrength}}<b>(</b>{{Type5|Plot}} fromPlot, {{Type5|Plot}} toPlot, {{Type5|Unit}} defender<b>)</b></code>
<!-- 
GETMAXDEFENSESTRENGTH
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|GetMaxDefenseStrength}}<b>(</b>{{Type5|Plot}} inPlot, {{Type5|Unit}} attacker, '''bool''' arg2 = nil<b>)</b></code>
<!-- 
GETMAXHITPOINTS
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|GetMaxHitPoints}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETMAXRANGEDCOMBATSTRENGTH
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|GetMaxRangedCombatStrength}}<b>(</b>{{Type5|Unit}} other, '''int''' attacking, '''bool''' arg2, '''bool''' arg3<b>)</b></code>
<!-- 
GETMOVES
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|GetMoves}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETNAME
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''string'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|GetName}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETNAMEKEY
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''string'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|GetNameKey}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETNAMENODESC
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''unknown'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|GetNameNoDesc}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETNEARBYIMPROVEMENTMODIFIER
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|GetNearbyImprovementModifier}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETNUMENEMYUNITSADJACENT
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|GetNumEnemyUnitsAdjacent}}<b>(</b>{{Type5|Unit}} otherUnit<b>)</b></code>
<!-- 
GETNUMFOLLOWERSAFTERSPREAD
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|GetNumFollowersAfterSpread}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETNUMRESOURCENEEDEDTOUPGRADE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|GetNumResourceNeededToUpgrade}}<b>(</b>{{Type5|ResourceType}} resourceLoop<b>)</b></code>
<!-- 
GETORIGINALOWNER
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|GetOriginalOwner}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETOUTSIDEFRIENDLYLANDSMODIFIER
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|GetOutsideFriendlyLandsModifier}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETOWNER
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>{{Type5|PlayerID}}</code>
|width="100%" |<code>{{FuncLabel5|Unit|GetOwner}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETPATHENDTURNPLOT
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''unknown'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|GetPathEndTurnPlot}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETPILLAGECHANGE
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|GetPillageChange}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETPLOT
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>{{Type5|Plot}}</code>
|width="100%" |<code>{{FuncLabel5|Unit|GetPlot}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETRANGECOMBATDAMAGE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|GetRangeCombatDamage}}<b>(</b>{{Type5|Unit}} defender, {{Type5|City}} city, '''bool''' includeRand<b>)</b></code>
<!-- 
GETRANGEDATTACKMODIFIER
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|GetRangedAttackModifier}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETRANGEDCOMBATLIMIT
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|GetRangedCombatLimit}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETRECONPLOT
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''unknown'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|GetReconPlot}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETRELIGION
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>{{Type5|ReligionType}}</code>
|width="100%" |<code>{{FuncLabel5|Unit|GetReligion}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETREVERSEGREATGENERALMODIFIER
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|GetReverseGreatGeneralModifier}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETRIVERCROSSINGNOPENALTYCOUNT
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|GetRiverCrossingNoPenaltyCount}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETSAMETILEHEAL
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|GetSameTileHeal}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETSCENARIODATA
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>{{UnknownSignature5}}</code>
|width="100%" |<code>{{FuncLabel5|Unit|GetScenarioData}}<!-- No arguments --></code>
<!-- 
GETSCRAPGOLD
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|GetScrapGold}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETSCRIPTDATA
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''string'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|GetScriptData}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETSEEINVISIBLETYPE
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>{{Type5|InvisibilityScopeType}}</code>
|width="100%" |<code>{{FuncLabel5|Unit|GetSeeInvisibleType}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETSPECIALUNITTYPE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>{{Type5|SpecialUnitType}}</code>
|width="100%" |<code>{{FuncLabel5|Unit|GetSpecialUnitType}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETSPREADSLEFT
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|GetSpreadsLeft}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETSTRATEGICRESOURCECOMBATPENALTY
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|GetStrategicResourceCombatPenalty}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETTEAM
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>{{Type5|TeamID}}</code>
|width="100%" |<code>{{FuncLabel5|Unit|GetTeam}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETTRADEGOLD
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|GetTradeGold}}<b>(</b>{{Type5|Plot}} plot<b>)</b></code>
<!-- 
GETTRANSPORTUNIT
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''unknown'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|GetTransportUnit}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETUNITAICARGO
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|GetUnitAICargo}}<b>(</b>{{Type5|UnitAIType}} unitAI<b>)</b></code>
<!-- 
GETUNITAITYPE
-->
|-
{{FuncInfos5|yes  |yes  |yes|<!-- No comment -->}}
|align="right"  |<code>{{Type5|UnitAIType}}</code>
|width="100%" |<code>{{FuncLabel5|Unit|GetUnitAIType}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETUNITCLASSMODIFIER
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|GetUnitClassModifier}}<b>(</b>{{Type5|UnitClassType}} index<b>)</b></code>
<!-- 
GETUNITCLASSTYPE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>{{Type5|UnitClassType}}</code>
|width="100%" |<code>{{FuncLabel5|Unit|GetUnitClassType}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETUNITCOMBATTYPE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>{{Type5|UnitCombatType}}</code>
|width="100%" |<code>{{FuncLabel5|Unit|GetUnitCombatType}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETUNITFLAGICONOFFSET
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''unknown'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|GetUnitFlagIconOffset}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETUNITPORTRAITOFFSET
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''unknown'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|GetUnitPortraitOffset}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETUNITTYPE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>{{Type5|UnitType}}</code>
|width="100%" |<code>{{FuncLabel5|Unit|GetUnitType}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETUPGRADEDISCOUNT
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|GetUpgradeDiscount}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETUPGRADEUNITFROMPLOT
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>{{Type5|Unit}}</code>
|width="100%" |<code>{{FuncLabel5|Unit|GetUpgradeUnitFromPlot}}<b>(</b>{{Type5|Plot}} adjacentPlot<b>)</b></code>
<!-- 
GETUPGRADEUNITTYPE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>{{Type5|UnitType}}</code>
|width="100%" |<code>{{FuncLabel5|Unit|GetUpgradeUnitType}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETVISUALOWNER
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|GetVisualOwner}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETX
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|GetX}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETY
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|GetY}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GIVEEXPERIENCE
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|GiveExperience}}<b>(</b><!-- No arguments --><b>)</b></code>
|}

==H==
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
HASCARGO
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|HasCargo}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
HASMOVED
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|HasMoved}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
HASNAME
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|HasName}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
HILLSATTACKMODIFIER
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|HillsAttackModifier}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
HILLSDEFENSEMODIFIER
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|HillsDefenseModifier}}<b>(</b><!-- No arguments --><b>)</b></code>
|}

==I==
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
IGNOREBUILDINGDEFENSE
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|IgnoreBuildingDefense}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
IGNORETERRAINCOST
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|IgnoreTerrainCost}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
IMMUNETOFIRSTSTRIKES
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|ImmuneToFirstStrikes}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ISACTIONRECOMMENDED
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|IsActionRecommended}}<b>(</b>{{Type5|ActionType}} action<b>)</b></code>
<!-- 
ISALWAYSHEAL
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|IsAlwaysHeal}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ISAMPHIB
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|IsAmphib}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ISATTACKING
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|IsAttacking}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ISAUTOMATED
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|IsAutomated}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ISBARBARIAN
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|IsBarbarian}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ISBETTERDEFENDERTHAN
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|IsBetterDefenderThan}}<b>(</b>{{Type5|Unit}} defender, {{Type5|Unit}} attacker<b>)</b></code>
<!-- 
ISBLITZ
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|IsBlitz}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ISBUSY
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|IsBusy}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ISCANATTACK
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|IsCanAttack}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ISCANATTACKRANGED
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|IsCanAttackRanged}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ISCANATTACKWITHMOVE
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|IsCanAttackWithMove}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ISCANATTACKWITHMOVENOW
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|IsCanAttackWithMoveNow}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ISCANDEFEND
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|IsCanDefend}}<b>(</b>{{Type5|Plot}} plot<b>)</b></code>
<!-- 
ISCARGO
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|IsCargo}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ISCITYATTACKONLY
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|IsCityAttackOnly}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ISCOMBATUNIT
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|IsCombatUnit}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ISDEAD
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|IsDead}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ISDEFENDING
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|IsDefending}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ISDELAYEDDEATH
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|IsDelayedDeath}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ISEMBARKED
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|IsEmbarked}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ISENEMYCITYADJACENT
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|IsEnemyCityAdjacent}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ISENEMYINMOVEMENTRANGE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|IsEnemyInMovementRange}}<b>(</b>'''bool''' arg0, '''bool''' arg1<b>)</b></code>
<!-- 
ISENEMYROUTE
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|IsEnemyRoute}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ISEVERFORTIFYABLE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|IsEverFortifyable}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ISFEATUREDOUBLEMOVE
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|IsFeatureDoubleMove}}<b>(</b>{{Type5|FeatureType}} index<b>)</b></code>
<!-- 
ISFIGHTING
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|IsFighting}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ISFORTIFYABLE
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|IsFortifyable}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ISFOUND
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|IsFound}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ISFRIENDLYUNITADJACENT
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|IsFriendlyUnitAdjacent}}<b>(</b>'''bool''' combatUnit<b>)</b></code>
<!-- 
ISFULL
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|IsFull}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ISGARRISONED
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|IsGarrisoned}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ISGOLDENAGE
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|IsGoldenAge}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ISGREATPERSON
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>{{UnknownSignature5}}</code>
|width="100%" |<code>{{FuncLabel5|Unit|IsGreatPerson}}<!-- No arguments --></code>
<!-- 
ISHASPROMOTION
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|IsHasPromotion}}<b>(</b>{{Type5|PromotionType}} promotion<b>)</b></code>
<!-- 
ISHEALOUTSIDEFRIENDLY
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|IsHealOutsideFriendly}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ISHIGHERTECHTHAN
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|IsHigherTechThan}}<b>(</b>{{Type5|UnitType}} arg0<b>)</b></code>
<!-- 
ISHILLSDOUBLEMOVE
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|IsHillsDoubleMove}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ISHUMAN
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|IsHuman}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ISHURT
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|IsHurt}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ISIMMOBILE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|IsImmobile}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ISINCOMBAT
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|IsInCombat}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ISINVISIBLE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|IsInvisible}}<b>(</b>{{Type5|TeamID}} team, '''bool''' debug, '''bool''' checkCargo = false<b>)</b></code>
<!-- 
ISLARGERCIVTHAN
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|IsLargerCivThan}}<b>(</b>{{Type5|Unit}} myUnit<b>)</b></code>
<!-- 
ISMUSTSETUPTORANGEDATTACK
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|IsMustSetUpToRangedAttack}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ISNEARGREATGENERAL
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|IsNearGreatGeneral}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ISNEVERINVISIBLE
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|IsNeverInvisible}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ISNOBADGOODIES
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|IsNoBadGoodies}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ISNOCAPTURE
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|IsNoCapture}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ISNONE
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|IsNone}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ISNUKEIMMUNE
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|IsNukeImmune}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ISNUKEVICTIM
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|IsNukeVictim}}<b>(</b>{{Type5|Plot}} plot, {{Type5|TeamID}} team<b>)</b></code>
<!-- 
ISONLYDEFENSIVE
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|IsOnlyDefensive}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ISOUTOFATTACKS
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|IsOutOfAttacks}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ISOUTOFINTERCEPTIONS
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|isOutOfInterceptions}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ISPROMOTIONREADY
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|IsPromotionReady}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ISPROMOTIONVALID
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|IsPromotionValid}}<b>(</b>{{Type5|PromotionType}} promotion<b>)</b></code>
<!-- 
ISRANGEATTACKIGNORELOS
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|IsRangeAttackIgnoreLOS}}<b>(</b>{{Type5|Plot}} plot<b>)</b></code>
<!-- 
ISRANGEATTACKONLYINDOMAIN
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|IsRangeAttackOnlyInDomain}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ISRANGED
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|IsRanged}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ISREADYTOMOVE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|IsReadyToMove}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ISRIVALTERRITORY
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|IsRivalTerritory}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ISRIVERCROSSINGNOPENALTY
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|IsRiverCrossingNoPenalty}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ISSELECTED
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|IsSelected}}<b>(</b>'''unknown''' void<b>)</b></code>
<!-- 
ISSETUPFORRANGEDATTACK
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|IsSetUpForRangedAttack}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ISSTACKEDGREATGENERAL
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|IsStackedGreatGeneral}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ISTERRAINDOUBLEMOVE
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|IsTerrainDoubleMove}}<b>(</b>{{Type5|TerrainType}} index<b>)</b></code>
<!-- 
ISWAITING
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|IsWaiting}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ISWORK
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|IsWork}}<b>(</b><!-- No arguments --><b>)</b></code>
|}

==J==
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
JUMPTONEARESTVALIDPLOT
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Unit|JumpToNearestValidPlot}}<b>(</b><!-- No arguments --><b>)</b></code>
|}

==K==
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
KILL
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Unit|Kill}}<b>(</b>'''bool''' delay, {{Type5|PlayerID}} player = NO_PLAYER<b>)</b></code>
|}

==L==
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
LASTMISSIONPLOT
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>{{UnknownSignature5}}</code>
|width="100%" |<code>{{FuncLabel5|Unit|LastMissionPlot}}<!-- No arguments --></code>
<!-- 
LEAD
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|Lead}}<b>(</b>'''int''' unitId<b>)</b></code>
|}

==M==
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
MAXFIRSTSTRIKES
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|MaxFirstStrikes}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
MAXINTERCEPTIONPROBABILITY
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|MaxInterceptionProbability}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
MAXMOVES
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|MaxMoves}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
MAXXPVALUE
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|MaxXPValue}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
MOVESLEFT
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|MovesLeft}}<b>(</b><!-- No arguments --><b>)</b></code>
|}

==N==
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
NODEFENSIVEBONUS
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|NoDefensiveBonus}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
NUKEDAMAGELEVEL
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|NukeDamageLevel}}<b>(</b><!-- No arguments --><b>)</b></code>
|}

==O==
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
OPENATTACKMODIFIER
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|OpenAttackModifier}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
OPENDEFENSEMODIFIER
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|OpenDefenseModifier}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
OPENRANGEDATTACKMODIFIER
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|OpenRangedAttackModifier}}<b>(</b><!-- No arguments --><b>)</b></code>
|}

==P==
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
POPMISSION
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>{{UnknownSignature5}}</code>
|width="100%" |<code>{{FuncLabel5|Unit|PopMission}}<!-- No arguments --></code>
<!-- 
PROMOTE
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Unit|Promote}}<b>(</b>{{Type5|PromotionType}} promotion, '''int''' leaderUnitId<b>)</b></code>
<!-- 
PUSHMISSION
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Unit|PushMission}}<b>(</b>{{Type5|MissionType}} mission, '''int''' data1 = -1, '''int''' data2 = -1, '''int''' flags = 0, '''bool''' append = false, '''bool''' manual = fa;se, {{Type5|MissionType}} missionAI = NO_MISSIONAI, {{Type5|Plot}} missionAIPlot = nil, {{Type5|Unit}} missionAIUnit = nil<b>)</b></code>
|}

==R==
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
RANGE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|Range}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
RANGESTRIKE
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Unit|RangeStrike}}<b>(</b>'''int''' x, '''int''' y<b>)</b></code>
<!-- 
ROTATEFACINGDIRECTIONCLOCKWISE
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>{{UnknownSignature5}}</code>
|width="100%" |<code>{{FuncLabel5|Unit|RotateFacingDirectionClockwise}}<!-- No arguments --></code>
<!-- 
ROTATEFACINGDIRECTIONCOUNTERCLOCKWISE
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>{{UnknownSignature5}}</code>
|width="100%" |<code>{{FuncLabel5|Unit|RotateFacingDirectionCounterClockwise}}<!-- No arguments --></code>
<!-- 
ROUGHATTACKMODIFIER
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|RoughAttackModifier}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ROUGHDEFENSEMODIFIER
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|RoughDefenseModifier}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ROUGHRANGEDATTACKMODIFIER
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|RoughRangedAttackModifier}}<b>(</b><!-- No arguments --><b>)</b></code>
|}

==S==
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
SETBASECOMBATSTRENGTH
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Unit|SetBaseCombatStrength}}<b>(</b>'''int''' combat<b>)</b></code>
<!-- 
SETDAMAGE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Unit|SetDamage}}<b>(</b>'''int''' newValue, {{Type5|PlayerID}} player, '''bool''' notifyEntity = true<b>)</b></code>
<!-- 
SETDEPLOYFROMOPERATIONTURN
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Unit|SetDeployFromOperationTurn}}<b>(</b>'''int''' arg0<b>)</b></code>
<!-- 
SETEMBARKED
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Unit|SetEmbarked}}<b>(</b>'''bool''' newValue<b>)</b></code>
<!-- 
SETEXPERIENCE
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Unit|SetExperience}}<b>(</b>'''int''' newValue, '''int''' max = -1<b>)</b></code>
<!-- 
SETHASPROMOTION
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Unit|SetHasPromotion}}<b>(</b>{{Type5|PromotionType}} index, '''bool''' newValue<b>)</b></code>
<!-- 
SETHOTKEYNUMBER
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Unit|SetHotKeyNumber}}<b>(</b>'''int''' newValue<b>)</b></code>
<!-- 
SETLEADERUNITTYPE
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Unit|SetLeaderUnitType}}<b>(</b>{{Type5|UnitType}} leaderUnitType<b>)</b></code>
<!-- 
SETLEVEL
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Unit|SetLevel}}<b>(</b>'''int''' newLevel<b>)</b></code>
<!-- 
SETMADEATTACK
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Unit|SetMadeAttack}}<b>(</b>'''bool''' newValue<b>)</b></code>
<!-- 
SETMADEINTERCEPTION
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Unit|SetMadeInterception}}<b>(</b>'''bool''' newValue<b>)</b></code>
<!-- 
SETMOVES
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Unit|SetMoves}}<b>(</b>'''int''' newValue<b>)</b></code>
<!-- 
SETNAME
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Unit|SetName}}<b>(</b>'''string''' newValue<b>)</b></code>
<!-- 
SETORIGINALOWNER
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Unit|SetOriginalOwner}}<b>(</b>{{Type5|PlayerID}} oldOwner<b>)</b></code>
<!-- 
SETPROMOTIONREADY
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Unit|SetPromotionReady}}<b>(</b>'''bool''' newValue<b>)</b></code>
<!-- 
SETRECONPLOT
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Unit|SetReconPlot}}<b>(</b>{{Type5|Plot}} newValue<b>)</b></code>
<!-- 
SETSCENARIODATA
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>{{UnknownSignature5}}</code>
|width="100%" |<code>{{FuncLabel5|Unit|SetScenarioData}}<!-- No arguments --></code>
<!-- 
SETSCRIPTDATA
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Unit|SetScriptData}}<b>(</b>'''string''' newValue<b>)</b></code>
<!-- 
SETXY
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Unit|SetXY}}<b>(</b>'''int''' x, '''int''' y, '''bool''' group = false, '''bool''' update = true, '''bool''' show = false, '''bool''' checkPlotVisible = false<b>)</b></code>
<!-- 
SPECIALCARGO
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>{{UnknownSignature5}}</code>
|width="100%" |<code>{{FuncLabel5|Unit|SpecialCargo}}<!-- No arguments --></code>
|}

==T==
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
TERRAINATTACKMODIFIER
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|TerrainAttackModifier}}<b>(</b>{{Type5|TerrainType}} terrain<b>)</b></code>
<!-- 
TERRAINDEFENSEMODIFIER
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|TerrainDefenseModifier}}<b>(</b>{{Type5|TerrainType}} terrain<b>)</b></code>
|}

==U==
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
UNITCLASSATTACKMODIFIER
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|UnitClassAttackModifier}}<b>(</b>{{Type5|UnitClassType}} unitClass<b>)</b></code>
<!-- 
UNITCLASSDEFENSEMODIFIER
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|UnitClassDefenseModifier}}<b>(</b>{{Type5|UnitClassType}} unitClass<b>)</b></code>
<!-- 
UNITCOMBATMODIFIER
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|UnitCombatModifier}}<b>(</b>{{Type5|UnitCombatType}} unitCombat<b>)</b></code>
<!-- 
UPGRADEPRICE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|UpgradePrice}}<b>(</b>{{Type5|UnitType}} unit<b>)</b></code>
|}

==V==
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
VISIBILITYRANGE
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|VisibilityRange}}<b>(</b><!-- No arguments --><b>)</b></code>
|}

==W==
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
WITHDRAWALPROBABILITY
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|WithdrawalProbability}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
WORKRATE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Unit|WorkRate}}<b>(</b>'''bool''' max, {{Type5|BuildActionType}} build = nil<b>)</b></code>
|}


=Used by=
{|cellspacing="4" cellpadding="0" width="100%" style="background-color:#F0F0F0"
<!-- 
ADDPRODUCTIONEXPERIENCE
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|City}}:{{Func5|City|AddProductionExperience}}<b>(</b>{{Type5|Unit}} unit, '''bool''' conscript = false<b>)</b></code>
<!-- 
GETGARRISONEDUNIT
-->
|-
|align="right" width="200" |<code>{{Type5|Unit}}</code>
|style="padding-left:6px" |<code>{{Type5|City}}:{{Func5|City|GetGarrisonedUnit}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
RANGECOMBATDAMAGE
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|City}}:{{Func5|City|RangeCombatDamage}}<b>(</b>{{Type5|Unit}} theirUnit, '''unknown''' arg1<b>)</b></code>
<!-- 
RANGECOMBATUNITDEFENSE
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|City}}:{{Func5|City|RangeCombatUnitDefense}}<b>(</b>{{Type5|Unit}} theirUnit<b>)</b></code>
<!-- 
GETCOMBATPREDICTION
-->
|-
|align="right" width="200" |<code>{{Type5|CombatPredictionType}}</code>
|style="padding-left:6px" |<code>{{Type5|Game}}.{{Func5|Game|GetCombatPrediction}}<b>(</b>{{Type5|Unit}} myUnit, {{Type5|Unit}} theirUnit<b>)</b></code>
<!-- 
CANRECEIVEGOODY
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|CanReceiveGoody}}<b>(</b>{{Type5|Plot}} plot, {{Type5|GoodyType}} goody, {{Type5|Unit}} unit<b>)</b></code>
<!-- 
CREATEGREATGENERAL
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|CreateGreatGeneral}}<b>(</b>{{Type5|Unit}} eGreatPersonUnit, '''bool''' incrementThreshold, '''bool''' incrementExperience, '''int''' x, '''int''' y<b>)</b></code>
<!-- 
DOGOODY
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|DoGoody}}<b>(</b>{{Type5|Plot}} plot, {{Type5|Unit}} unit<b>)</b></code>
<!-- 
GETFIRSTREADYUNIT
-->
|-
|align="right" width="200" |<code>{{Type5|Unit}}</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|GetFirstReadyUnit}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETUNITBYID
-->
|-
|align="right" width="200" |<code>{{Type5|Unit}}</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|GetUnitByID}}<b>(</b>{{Type5|UnitID}} unit<b>)</b></code>
<!-- 
INITUNIT
-->
|-
|align="right" width="200" |<code>{{Type5|Unit}}</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|InitUnit}}<b>(</b>{{Type5|UnitType}} unit, {{Type5|ResourceType}} x, {{Type5|ResourceType}} y, {{Type5|UnitAIType}} unitAI = NO_UNITAI, {{Type5|DirectionType}} facingDirection = NO_DIRECTION<b>)</b></code>
<!-- 
RECEIVEGOODY
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|ReceiveGoody}}<b>(</b>{{Type5|Plot}} plot, {{Type5|GoodyType}} goody, {{Type5|Unit}} unit<b>)</b></code>
<!-- 
UNITS
-->
|-
|align="right" width="200" |<code>iterator({{Type5|Unit}})</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|Units}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETBESTDEFENDER
-->
|-
|align="right" width="200" |<code>'''unknown'''</code>
|style="padding-left:6px" |<code>{{Type5|Plot}}:{{Func5|Plot|GetBestDefender}}<b>(</b>{{Type5|PlayerID}} owner, {{Type5|PlayerID}} attackingPlayer, {{Type5|Unit}} attacker, '''bool''' testAtWar, '''bool''' testPotentialEnemy, '''bool''' testCanMove<b>)</b></code>
<!-- 
GETNUMFRIENDLYUNITSOFTYPE
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Plot}}:{{Func5|Plot|GetNumFriendlyUnitsOfType}}<b>(</b>{{Type5|Unit}} unit<b>)</b></code>
<!-- 
GETNUMVISIBLEENEMYDEFENDERS
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Plot}}:{{Func5|Plot|GetNumVisibleEnemyDefenders}}<b>(</b>{{Type5|Unit}} unit<b>)</b></code>
<!-- 
GETNUMVISIBLEPOTENTIALENEMYDEFENDERS
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Plot}}:{{Func5|Plot|GetNumVisiblePotentialEnemyDefenders}}<b>(</b>{{Type5|Unit}} unit<b>)</b></code>
<!-- 
GETUNIT
-->
|-
|align="right" width="200" |<code>{{Type5|Unit}}</code>
|style="padding-left:6px" |<code>{{Type5|Plot}}:{{Func5|Plot|GetUnit}}<b>(</b>{{Type5|UnitID}} id<b>)</b></code>
<!-- 
ISENEMYCITY
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Plot}}:{{Func5|Plot|IsEnemyCity}}<b>(</b>{{Type5|Unit}} unit<b>)</b></code>
<!-- 
ISFRIENDLYCITY
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|Plot}}:{{Func5|Plot|IsFriendlyCity}}<b>(</b>{{Type5|Unit}} unit, '''bool''' checkImprovement<b>)</b></code>
<!-- 
ISVALIDDOMAINFORACTION
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|Plot}}:{{Func5|Plot|IsValidDomainForAction}}<b>(</b>{{Type5|Unit}} unit<b>)</b></code>
<!-- 
ISVALIDDOMAINFORLOCATION
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|Plot}}:{{Func5|Plot|IsValidDomainForLocation}}<b>(</b>{{Type5|Unit}} unit<b>)</b></code>
<!-- 
ISVISIBLEENEMYDEFENDER
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Plot}}:{{Func5|Plot|IsVisibleEnemyDefender}}<b>(</b>{{Type5|Unit}} unit<b>)</b></code>
<!-- 
MOVEMENTCOST
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Plot}}:{{Func5|Plot|MovementCost}}<b>(</b>{{Type5|Unit}} unit, {{Type5|Plot}} fromPlot<b>)</b></code>
<!-- 
NUKEEXPLOSION
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Plot}}:{{Func5|Plot|NukeExplosion}}<b>(</b>'''int''' range, {{Type5|Unit}} nukeUnit<b>)</b></code>
<!-- 
GETHEADSELECTEDUNIT
-->
|-
|align="right" width="200" |<code>{{Type5|Unit}}</code>
|style="padding-left:6px" |<code>{{Type5|UI}}.{{Func5|UI|GetHeadSelectedUnit}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
HIGHLIGHTCANPLACEPLOTS
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|UI}}.{{Func5|UI|HighlightCanPlacePlots}}<b>(</b>{{Type5|Unit}} unit, {{Type5|Plot}} arg1<b>)</b></code>
<!-- 
SELECTUNIT
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|UI}}.{{Func5|UI|SelectUnit}}<b>(</b>{{Type5|Unit}} v<b>)</b></code>
<!-- 
SETPLACEUNIT
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|UI}}.{{Func5|UI|SetPlaceUnit}}<b>(</b>{{Type5|Unit}} unit<b>)</b></code>
<!-- 
CANLOADUNIT
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|Unit}}:{{Func5|Unit|CanLoadUnit}}<b>(</b>{{Type5|Unit}} unit, {{Type5|Plot}} plot<b>)</b></code>
<!-- 
CONVERT
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Unit}}:{{Func5|Unit|Convert}}<b>(</b>{{Type5|Unit}} unit<b>)</b></code>
<!-- 
GETAIRCOMBATDAMAGE
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Unit}}:{{Func5|Unit|GetAirCombatDamage}}<b>(</b>{{Type5|Unit}} defender<b>)</b></code>
<!-- 
GETFIRESUPPORTUNIT
-->
|-
|align="right" width="200" |<code>{{Type5|Unit}}</code>
|style="padding-left:6px" |<code>{{Type5|Unit}}:{{Func5|Unit|GetFireSupportUnit}}<b>(</b>{{Type5|PlayerID}} defender, '''int''' x, '''int''' y<b>)</b></code>
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
GETMAXRANGEDCOMBATSTRENGTH
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Unit}}:{{Func5|Unit|GetMaxRangedCombatStrength}}<b>(</b>{{Type5|Unit}} other, '''int''' attacking, '''bool''' arg2, '''bool''' arg3<b>)</b></code>
<!-- 
GETNUMENEMYUNITSADJACENT
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Unit}}:{{Func5|Unit|GetNumEnemyUnitsAdjacent}}<b>(</b>{{Type5|Unit}} otherUnit<b>)</b></code>
<!-- 
GETRANGECOMBATDAMAGE
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Unit}}:{{Func5|Unit|GetRangeCombatDamage}}<b>(</b>{{Type5|Unit}} defender, {{Type5|City}} city, '''bool''' includeRand<b>)</b></code>
<!-- 
GETUPGRADEUNITFROMPLOT
-->
|-
|align="right" width="200" |<code>{{Type5|Unit}}</code>
|style="padding-left:6px" |<code>{{Type5|Unit}}:{{Func5|Unit|GetUpgradeUnitFromPlot}}<b>(</b>{{Type5|Plot}} adjacentPlot<b>)</b></code>
<!-- 
ISBETTERDEFENDERTHAN
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|Unit}}:{{Func5|Unit|IsBetterDefenderThan}}<b>(</b>{{Type5|Unit}} defender, {{Type5|Unit}} attacker<b>)</b></code>
<!-- 
ISLARGERCIVTHAN
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Unit}}:{{Func5|Unit|IsLargerCivThan}}<b>(</b>{{Type5|Unit}} myUnit<b>)</b></code>
<!-- 
PUSHMISSION
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Unit}}:{{Func5|Unit|PushMission}}<b>(</b>{{Type5|MissionType}} mission, '''int''' data1 = -1, '''int''' data2 = -1, '''int''' flags = 0, '''bool''' append = false, '''bool''' manual = fa;se, {{Type5|MissionType}} missionAI = NO_MISSIONAI, {{Type5|Plot}} missionAIPlot = nil, {{Type5|Unit}} missionAIUnit = nil<b>)</b></code>
|}




{{Civ5 API Footer}}
[[Category:Civ5 Types|Unit]]