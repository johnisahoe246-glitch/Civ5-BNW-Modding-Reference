{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



= Usage =
This object exposes events that you can use to modify the gameplay. As opposed to the events defined on {{Type5|Events}} and {{Type5|LuaEvents}}, most of those events are expected to return a value. This value may then be used by the game to prevent or trigger some game actions (such as a declaration of war), or to override some calculations (for example by adding a bonus or a malus to the diplomatic status between two civilizations). Please look at the events' pages to learn more.


=Static Events=
Events can be subscribed by using <code>GameEvents.SomeEvent.Add(SomeFunction)</code>. Regular events can also be fired through a '''dot''' by using <code>GameEvents.SomeEvent(&lt;args&gt;)</code>. This will invoke all subscribers with the provided arguments.<br/>
==C==
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
CANDECLAREWAR
-->
|-
{{FuncInfos5|yes  |maybe|yes|Allows provision of criteria for the ability to declare war. As this is a TestAll event, all listeners must return true for the action to be permitted. As wars are between teams, it is based entirely on teams rather than players (as far as can be inferred from scenario files).}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|GameEvents|CanDeclareWar}}<b>(</b>{{Type5|TeamID}} myTeam, {{Type5|TeamID}} theirTeam<b>)</b></code>
<!-- 
CITYBUILDINGSISBUILDINGSELLABLE
-->
|-
{{FuncInfos5|no   |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|GameEvents|CityBuildingsIsBuildingSellable}}<b>(</b>{{Type5|PlayerID}} player, {{Type5|BuildingType}} building<b>)</b></code>
<!-- 
CITYCANANYBUYPLOT
-->
|-
{{FuncInfos5|yes  |maybe|yes|}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|GameEvents|CityCanBuyAnyPlot}}<b>(</b>{{Type5|PlayerID}} player, {{Type5|CityID}} city<b>)</b></code>
<!-- 
CITYCANBUYPLOT
-->
|-
{{FuncInfos5|yes  |maybe|yes|}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|GameEvents|CityCanBuyPlot}}<b>(</b>{{Type5|PlayerID}} player, {{Type5|CityID}} city, '''int''' x, '''int''' y<b>)</b></code>
<!-- 
CITYCANCONSTRUCT
-->
|-
{{FuncInfos5|yes  |maybe|yes|Similar to CanDeclareWar, this allows provision of critera for the ability to construct a particular building (including Wonders, presumably) in a particular city. Based on the behaviour in the 1066 scenario, it seems that returns of false lead to the building not appearing in the list of buildings available to construct, rather than being greyed out, but this hasn't been specifically checked. It makes some sense, though, as there's no way to provide a tooltip to explain the greying out under this mechanism. As with CanDeclareWar, it's unclear whether multiple listeners' returns are combined with AND or OR; either seems possible according to the detailed explanation of how these events are handled.}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|GameEvents|CityCanConstruct}}<b>(</b>{{Type5|PlayerID}} player, {{Type5|CityID}} city, {{Type5|BuildingType}} buildingType<b>)</b></code>
<!-- 
CityCanCreate
-->
|-
{{FuncInfos5|yes  |maybe|yes|}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|GameEvents|CityCanCreate}}<b>(</b>{{Type5|PlayerID}} player, {{Type5|CityID}} city, {{Type5|ProjectType}} projectType<b>)</b></code>
<!-- 
CityCanMaintain
-->
|-
{{FuncInfos5|yes  |maybe|yes|}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|GameEvents|CityCanMaintain}}<b>(</b>{{Type5|PlayerID}} player, {{Type5|CityID}} city, {{Type5|ProcessType}} processType<b>)</b></code>
<!-- 
CityCanPrepare
-->
|-
{{FuncInfos5|yes  |maybe|yes|}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|GameEvents|CityCanPrepare}}<b>(</b>{{Type5|PlayerID}} player, {{Type5|CityID}} city, {{Type5|SpecialistType}} specialistType<b>)</b></code>
<!-- 
CITYCANTRAIN
-->
|-
{{FuncInfos5|yes  |maybe|yes|}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|GameEvents|CityCanTrain}}<b>(</b>{{Type5|PlayerID}} player, {{Type5|CityID}} city, {{Type5|UnitType}} unitType<b>)</b></code>
<!-- 
CITYCAPTURECOMPLETE
-->
|-
{{FuncInfos5|yes  |yes  |yes|This event is triggered when a city is captured. We may infer from the name that it is triggered when the capture has been completed, the city now shows as owned by the conqueror, and buildings have been destroyed (this has not been confirmed). We might hope that there is a matching event when the capture has been determined, but ownership not yet changed and buildings not yet destroyed, but have no information on this as yet.}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|GameEvents|CityCaptureComplete}}<b>(</b>{{Type5|PlayerID}} player, '''int''' capital, {{Type5|ResourceType}} x, {{Type5|ResourceType}} y, {{Type5|PlayerID}} newPlayer, '''int''' conquest, '''int''' conquest<b>)</b></code>
<!-- 
CITYCONVERTSRELIGION
-->
|-
{{FuncInfos5|no   |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|GameEvents|CityConvertsReligion}}<b>(</b>{{Type5|PlayerID}} owner, {{Type5|ReligionType}} religion, '''int''' x, '''int''' y<b>)</b></code>
|}

==D==
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
DORESOLVEVICTORYVOTE
-->
|-
{{FuncInfos5|no   |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|GameEvents|DoResolveVictoryVote}}<b>(</b>'''bool''' preliminaryVote<b>)</b></code>
|}

==G==
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
GAMECORETESTVICTORY
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|GameEvents|GameCoreTestVictory}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GAMECOREUPDATEBEGIN
-->
|-
{{FuncInfos5|maybe|yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|GameEvents|GameCoreUpdateBegin}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GAMECOREUPDATEEND
-->
|-
{{FuncInfos5|maybe|yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|GameEvents|GameCoreUpdateEnd}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETFOUNDERBENEFITSRELIGION
-->
|-
{{FuncInfos5|no   |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|GameEvents|GetFounderBenefitsReligion}}<b>(</b>{{Type5|PlayerID}} player<b>)</b></code>
<!-- 
GETRELIGIONTOSPREAD
-->
|-
{{FuncInfos5|no   |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|GameEvents|GetReligionToSpread}}<b>(</b>{{Type5|PlayerID}} player<b>)</b></code>
<!-- 
GETSCENARIODIPLOMODIFIER1
-->
|-
{{FuncInfos5|no   |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|GameEvents|GetScenarioDiploModifier1}}<b>(</b>{{Type5|PlayerID}} player1, {{Type5|PlayerID}} player2<b>)</b></code>
<!-- 
GETSCENARIODIPLOMODIFIER2
-->
|-
{{FuncInfos5|no   |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|GameEvents|GetScenarioDiploModifier2}}<b>(</b>{{Type5|PlayerID}} player1, {{Type5|PlayerID}} player2<b>)</b></code>
|}

==P==
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
PLAYERADOPTPOLICY
-->
|-
{{FuncInfos5|maybe|yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|GameEvents|PlayerAdoptPolicy}}<b>(</b>{{Type5|PlayerID}} player, '''int''' policyID<b>)</b></code>
<!-- 
PlayerCanConstruct
-->
|-
{{FuncInfos5|maybe|yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|GameEvents|PlayerCanConstruct}}<b>(</b>{{Type5|PlayerID}} player, {{Type5|BuildingType}} buildingType<b>)</b></code>
<!-- 
PlayerCanCreate
-->
|-
{{FuncInfos5|maybe|yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|GameEvents|PlayerCanCreate}}<b>(</b>{{Type5|PlayerID}} player, {{Type5|ProjectType}} projectType<b>)</b></code>
<!-- 
PlayerCanMaintain
-->
|-
{{FuncInfos5|maybe|yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|GameEvents|PlayerCanMaintain}}<b>(</b>{{Type5|PlayerID}} player, {{Type5|ProcessType}} processType<b>)</b></code>
<!-- 
PlayerCanPrepare
-->
|-
{{FuncInfos5|maybe|yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|GameEvents|PlayerCanPrepare}}<b>(</b>{{Type5|PlayerID}} player, {{Type5|SpecialistType}} specialistType<b>)</b></code>
<!-- 
PlayerCanResearch
-->
|-
{{FuncInfos5|maybe|yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|GameEvents|PlayerCanResearch}}<b>(</b>{{Type5|PlayerID}} player, {{Type5|TechType}} techType<b>)</b></code>
<!-- 
PlayerCanEverResearch
-->
|-
{{FuncInfos5|maybe|yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|GameEvents|PlayerCanEverResearch}}<b>(</b>{{Type5|PlayerID}} player, {{Type5|TechType}} techType<b>)</b></code>
<!-- 
PlayerCanTrain
-->
|-
{{FuncInfos5|maybe|yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|GameEvents|PlayerCanTrain}}<b>(</b>{{Type5|PlayerID}} player, {{Type5|UnitType}} unitType<b>)</b></code>
<!-- 
PLAYERCITYFOUNDED
-->
|-
{{FuncInfos5|no   |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|GameEvents|PlayerCityFounded}}<b>(</b>{{Type5|PlayerID}} player, '''int''' cityX, '''int''' cityY<b>)</b></code>
<!-- 
PLAYERDOTURN
-->
|-
{{FuncInfos5|yes  |yes  |yes|Fired once per turn for each player (not just active/human player). Modder experimentation has found that it is fired at the start of turn; also, it seems not to run for the first turn of the game (for all players), runs only for human player on the second turn, and thereafter it runs for all players. There is no indication as to why this is.}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|GameEvents|PlayerDoTurn}}<b>(</b>{{Type5|PlayerID}} player<b>)</b></code>
<!-- 
PLAYERPREAIUNITUPDATE
-->
|-
{{FuncInfos5|maybe|maybe|yes|On list provided by User:Sseckman, but no references yet found in scenario Lua files.}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|GameEvents|PlayerPreAIUnitUpdate}}<b>(</b>{{Type5|PlayerID}} player<b>)</b></code>
<!-- 
PREGAMESTART
-->
|-
{{FuncInfos5|maybe|maybe|yes|Called before most items in the game are initialized. Was once used in scenario scripts, a different strategy was used; unclear how easy it would be to get a listener registered before it fires. Apparently does not pass any parameters.}}
|align="right"  |<code>{{UnknownSignature5}}</code>
|width="100%" |<code>{{FuncLabel5|GameEvents|PreGameStart}}<!-- No arguments --></code>
|}

==S==
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
SETALLY
-->
|-
{{FuncInfos5|yes  |yes  |yes|Triggered when the ally of a City-State changes (whether it changes from none or from another player).}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|GameEvents|SetAlly}}<b>(</b>{{Type5|PlayerID}} cSPlayer, {{Type5|PlayerID}} oldAlly, {{Type5|PlayerID}} newAlly<b>)</b></code>
<!-- 
SETPOPULATION
-->
|-
{{FuncInfos5|yes  |maybe|yes|Triggered whenever any city changes population. At least, as far as we know. Information provided by User:Sseckman calls this CitySetPopulation, but the scenario Lua files refer to SetPopulation.}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|GameEvents|SetPopulation}}<b>(</b>'''int''' x, '''int''' y, '''unknown''' oldPopulation, '''int''' newPopulation<b>)</b></code>
|}

==T==
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
TEAMMEET
-->
|-
{{FuncInfos5|maybe|maybe|yes|Presumably called when players meet, but referring to teams. Sample usages have not been found.}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|GameEvents|TeamMeet}}<b>(</b>'''unknown''' playeractive, '''unknown''' playermet<b>)</b></code>
<!-- 
TEAMSETHASTECH
-->
|-
{{FuncInfos5|maybe|yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|GameEvents|TeamSetHasTech}}<b>(</b>{{Type5|TeamID}} team, {{Type5|TechType}} tech, '''bool''' adopted<b>)</b></code>
<!-- 
TEAMTECHRESEARCHED
-->
|-
{{FuncInfos5|yes  |yes  |yes|Triggered when a team researches a tech.}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|GameEvents|TeamTechResearched}}<b>(</b>{{Type5|TeamID}} team, {{Type5|TechType}} tech, '''int''' change<b>)</b></code>
|}

==U==
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
UNITGETSPECIALEXPLORETARGET
-->
|-
{{FuncInfos5|yes  |maybe|yes|Appears to be triggered when the 'explore' order is given, or some subset thereof. The unit structure for the relevant unit is manipulated to set the explore target. ====Listener Prototype==== listener(iPlayerID, iUnitID) *iPlayerID The ID of the player who issued the explore order. *iUnitID The ID of the unit the order was issued to.}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|GameEvents|UnitGetSpecialExploreTarget}}<b>(</b>{{Type5|PlayerID}} player, {{Type5|UnitID}} unitID<b>)</b></code>
<!-- 
UnitKilledInCombat
-->
|-
{{FuncInfos5|yes  |maybe|yes|}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|GameEvents|UnitKilledInCombat}}<b>(</b>{{Type5|PlayerID}} killer, {{Type5|PlayerID}} killee, {{Type5|UnitType}} killeeUnitType<b>)</b></code>
<!-- 
UNITSETXY
-->
|-
{{FuncInfos5|yes  |yes  |yes|Triggered whenever any unit moves by any means, for every tile they move into.}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|GameEvents|UnitSetXY}}<b>(</b>{{Type5|PlayerID}} player, {{Type5|UnitID}} unit, '''int''' x, '''int''' y<b>)</b></code>
|}


=Static Methods=
Methods are functions that belong to an object. Static methods are invoked through a '''dot''', as in <code>GameEvents.SomeMethod(&lt;args&gt;)</code>. When a dot is used the caller object is not implicitly provided as the first argument.
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
ACCUMULATE
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>{{UnknownSignature5}}</code>
|width="100%" |<code>{{FuncLabel5|GameEvents|Accumulate}}<!-- No arguments --></code>
<!-- 
ACCUMULATEINT
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>{{UnknownSignature5}}</code>
|width="100%" |<code>{{FuncLabel5|GameEvents|AccumulateINT}}<!-- No arguments --></code>
<!-- 
ADD
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>{{UnknownSignature5}}</code>
|width="100%" |<code>{{FuncLabel5|GameEvents|Add}}<!-- No arguments --></code>
<!-- 
CALL
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>{{UnknownSignature5}}</code>
|width="100%" |<code>{{FuncLabel5|GameEvents|Call}}<!-- No arguments --></code>
<!-- 
COUNT
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>{{UnknownSignature5}}</code>
|width="100%" |<code>{{FuncLabel5|GameEvents|Count}}<!-- No arguments --></code>
<!-- 
REMOVE
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>{{UnknownSignature5}}</code>
|width="100%" |<code>{{FuncLabel5|GameEvents|Remove}}<!-- No arguments --></code>
<!-- 
REMOVEALL
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>{{UnknownSignature5}}</code>
|width="100%" |<code>{{FuncLabel5|GameEvents|RemoveAll}}<!-- No arguments --></code>
<!-- 
TESTALL
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>{{UnknownSignature5}}</code>
|width="100%" |<code>{{FuncLabel5|GameEvents|TestAll}}<!-- No arguments --></code>
<!-- 
TESTANY
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>{{UnknownSignature5}}</code>
|width="100%" |<code>{{FuncLabel5|GameEvents|TestAny}}<!-- No arguments --></code>
|}




{{Civ5 API Footer}}
[[Category:Civ5 Types|GameEvents]]