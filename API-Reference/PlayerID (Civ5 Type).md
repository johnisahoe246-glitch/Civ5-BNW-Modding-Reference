{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|ID.png|The <code>PlayerID</code> pseudo-type is actually a regular '''integer'''. Pseudo-types do not exist in Lua, they only serve a documentation purpose on the wiki!}}


= Usage =
* You can get a player's ID through {{Type5|Player}}.{{Func5|Player|GetID}}(). 
* There is a global '''Players''' table that stores all players. Keys are the players' ID and values are {{Type5|Player}} instances.
* The majors civs ID start at 0, up to 21. The minor civs ID start at 22, up to 62. The barbarians always have the ID 63. 
* Those numbers may change in the future, so use the constants defined in {{Type5|GameDefines}} (see the constants section below) rather than hard-coded values.


How to retrieve a {{Type5|Player}} object from an ID:
<syntaxhighlight lang="lua" class="civ5-example">
local pPlayer = Players[playerID]
</syntaxhighlight>


== Enumerating players ==
{{Warning}} Before you invoke a method on a player, ensure that {{Func5|Player|IsEverAlive}} is true, otherwise Civilzation V will crash. Do not use {{Func5|Player|IsAlive}}: while it may work sometimes, it does not always prevent a crash.
<syntaxhighlight lang="lua" class="civ5-example">
for id, player in pairs(Players) do
	if player:IsEverAlive() then
		print(id, player:GetName())
	end
end
</syntaxhighlight>

On a map with two players and two city states this will produce the following output:
<pre>
0   Wu Zetian
1   Genghis Khan
22  Monaco
23  Geneva
24  Warsaw
63  Barbarian
</pre>


=== Built-in constants ===
You can also use the built-in constants: <code>GameDefines.MAX_PLAYERS</code> (64), <code>GameDefines.MAX_CIV_PLAYERS</code> (63), <code>GameDefines.MAX_MAJOR_CIVS</code> (22) and <code>GameDefines.MAX_MINOR_CIVS</code> (41). See also {{Type5|GameDefines}}<br/>
The following example enumerates major civs only:
<syntaxhighlight lang="lua" class="civ5-example">
for i = 0, GameDefines.MAX_MAJOR_CIVS - 1 do
	if Players[i]:IsEverAlive() then
		print(i, Players[i]:GetName())
	end
end
</syntaxhighlight>


== Code snippets ==
Here is a function to get a player by its {{Type5|CivilizationType}}. We then use it to print Wu Zeitan's name.
<syntaxhighlight lang="lua" class="civ5-example">
function GetPlayerByCivilization(civilizationType)
	for _, pPlayer in pairs(Players) do
		if pPlayer:GetCivilizationType() == civilizationType then 
			return pPlayer
		end
	end
end

local chineseCivilizationType = GameInfos.Civilizations.CIVILIZATION_CHINA.ID
local chinesePlayer = GetPlayerByCivilization(chineseCivilizationType)
print(chinesePlayer:GetName())	-- print "Wu Zeitan"
</syntaxhighlight>


=Used by=
{|cellspacing="4" cellpadding="0" width="100%" style="background-color:#F0F0F0"
<!-- 
CIVICONHOOKUP
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Func5|CivIconHookup}}<b>(</b>{{Type5|PlayerID}} player, '''int''' iconSize, {{Type5|Image}} iconControl, {{Type5|Image}} teamColorControl, '''int''' shadowIconControl, '''int''' alwaysUseComposite, '''int''' shadowed<b>)</b></code>
<!-- 
GETCITYSTATESTATUS
-->
|-
|align="right" width="200" |<code>'''string'''</code>
|style="padding-left:6px" |<code>{{Func5|GetCityStateStatus}}<b>(</b>{{Type5|Player}} player, {{Type5|PlayerID}} forPlayer, '''int''' war<b>)</b></code>
<!-- 
GETMOODINFO
-->
|-
|align="right" width="200" |<code>'''string'''</code>
|style="padding-left:6px" |<code>{{Func5|GetMoodInfo}}<b>(</b>{{Type5|PlayerID}} otherPlayer<b>)</b></code>
<!-- 
GETPLAYERANDTEAMINFO
-->
|-
|align="right" width="200" |<code>'''int''', '''int''', table('''int''' => {{Type5|PlayerID}}), '''bool''', table('''int''' => '''int'''), '''table'''</code>
|style="padding-left:6px" |<code>{{Func5|GetPlayerAndTeamInfo}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETSHUFFLEDCOPYOFTABLE
-->
|-
|align="right" width="200" |<code>table('''int''' => {{Type5|PlayerID}})</code>
|style="padding-left:6px" |<code>{{Func5|GetShuffledCopyOfTable}}<b>(</b>table('''int''' => '''int''') incoming_table<b>)</b></code>
<!-- 
GETSTARTREGIONPRIORITYLISTFORCIV_GETIDS
-->
|-
|align="right" width="200" |<code>table('''int''' => '''int''')</code>
|style="padding-left:6px" |<code>{{Func5|GetStartRegionPriorityListForCiv_GetIDs}}<b>(</b>'''string''' civType<b>)</b></code>
<!-- 
IDENTIFYTABLEINDEX
-->
|-
|align="right" width="200" |<code>'''bool''', '''int''', table('''int''' => '''int''')</code>
|style="padding-left:6px" |<code>{{Func5|IdentifyTableIndex}}<b>(</b>table('''int''' => {{Type5|PlayerID}}) incoming_table, {{Type5|PlayerID}} value<b>)</b></code>
<!-- 
SIMPLECIVICONHOOKUP
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Func5|SimpleCivIconHookup}}<b>(</b>{{Type5|PlayerID}} player, '''int''' iconSize, {{Type5|Image}} iconControl<b>)</b></code>
<!-- 
TESTMEMBERSHIP
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Func5|TestMembership}}<b>(</b>table('''int''' => {{Type5|PlayerID}}) table, {{Type5|PlayerID}} value<b>)</b></code>
<!-- 
TOGRIDFROMHEX
-->
|-
|align="right" width="200" |<code>{{Type5|ResourceType}}, {{Type5|PlayerID}}</code>
|style="padding-left:6px" |<code>{{Func5|ToGridFromHex}}<b>(</b>'''float''' i, '''float''' j<b>)</b></code>
<!-- 
UNITMOVING
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Func5|UnitMoving}}<b>(</b>{{Type5|PlayerID}} player, {{Type5|UnitID}} unit<b>)</b></code>
<!-- 
GETCITIESPERPLAYER
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Area}}:{{Func5|Area|GetCitiesPerPlayer}}<b>(</b>{{Type5|PlayerID}} index<b>)</b></code>
<!-- 
GETFREESPECIALIST
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Area}}:{{Func5|Area|GetFreeSpecialist}}<b>(</b>{{Type5|PlayerID}} index<b>)</b></code>
<!-- 
GETPOPULATIONPERPLAYER
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Area}}:{{Func5|Area|GetPopulationPerPlayer}}<b>(</b>{{Type5|PlayerID}} index<b>)</b></code>
<!-- 
GETTARGETCITY
-->
|-
|align="right" width="200" |<code>'''unknown'''</code>
|style="padding-left:6px" |<code>{{Type5|Area}}:{{Func5|Area|GetTargetCity}}<b>(</b>{{Type5|PlayerID}} index<b>)</b></code>
<!-- 
GETUNITSPERPLAYER
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Area}}:{{Func5|Area|GetUnitsPerPlayer}}<b>(</b>{{Type5|PlayerID}} index<b>)</b></code>
<!-- 
GETYIELDRATEMODIFIER
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Area}}:{{Func5|Area|GetYieldRateModifier}}<b>(</b>{{Type5|PlayerID}} index1, {{Type5|YieldType}} index2<b>)</b></code>
<!-- 
ASSIGNLUXURYTOREGION
-->
|-
|align="right" width="200" |<code>{{Type5|ResourceType}}</code>
|style="padding-left:6px" |<code>{{Type5|AssignStartingPlots}}:{{Func5|AssignStartingPlots|AssignLuxuryToRegion}}<b>(</b>{{Type5|PlayerID}} region_number<b>)</b></code>
<!-- 
FINDFALLBACKFORUNMATCHEDREGIONPRIORITY
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|AssignStartingPlots}}:{{Func5|AssignStartingPlots|FindFallbackForUnmatchedRegionPriority}}<b>(</b>'''int''' regionType, table('''int''' => {{Type5|PlayerID}}) regions_still_available<b>)</b></code>
<!-- 
GENERATELUXURYPLOTLISTSINREGION
-->
|-
|align="right" width="200" |<code>'''unknown'''</code>
|style="padding-left:6px" |<code>{{Type5|AssignStartingPlots}}:{{Func5|AssignStartingPlots|GenerateLuxuryPlotListsInRegion}}<b>(</b>{{Type5|PlayerID}} region_number<b>)</b></code>
<!-- 
OBTAINNEXTSECTIONINREGION
-->
|-
|align="right" width="200" |<code>table('''int''' => '''int'''), table('''int''' => '''int'''), '''unknown''', '''unknown''', '''unknown''', '''unknown''', '''unknown'''</code>
|style="padding-left:6px" |<code>{{Type5|AssignStartingPlots}}:{{Func5|AssignStartingPlots|ObtainNextSectionInRegion}}<b>(</b>'''int''' incoming_west_x, '''int''' incoming_south_y, '''int''' incoming_width, '''int''' incoming_height, {{Type5|AreaID}} areaID, '''int''' force_it, '''int''' ignore_collisions<b>)</b></code>
<!-- 
PLACECITYSTATE
-->
|-
|align="right" width="200" |<code>'''int''', '''int''', '''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|AssignStartingPlots}}:{{Func5|AssignStartingPlots|PlaceCityState}}<b>(</b>table('''int''' => '''int''') coastal_plot_list, table('''int''' => '''int''') inland_plot_list, '''bool''' check_proximity, '''bool''' check_collision<b>)</b></code>
<!-- 
PLACECITYSTATEINREGION
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|AssignStartingPlots}}:{{Func5|AssignStartingPlots|PlaceCityStateInRegion}}<b>(</b>'''int''' city_state_number, {{Type5|PlayerID}} region_number<b>)</b></code>
<!-- 
PLACEFISH
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|AssignStartingPlots}}:{{Func5|AssignStartingPlots|PlaceFish}}<b>(</b>'''int''' frequency, table('''int''' => {{Type5|PlayerID}}) plot_list<b>)</b></code>
<!-- 
PLACESMALLQUANTITIESOFSTRATEGICS
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|AssignStartingPlots}}:{{Func5|AssignStartingPlots|PlaceSmallQuantitiesOfStrategics}}<b>(</b>'''int''' frequency, table('''int''' => '''int''') plot_list<b>)</b></code>
<!-- 
PLACESPECIFICNUMBEROFRESOURCES
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|AssignStartingPlots}}:{{Func5|AssignStartingPlots|PlaceSpecificNumberOfResources}}<b>(</b>{{Type5|ResourceType}} resource_, {{Type5|ResourceType}} quantity, '''int''' amount, '''float''' ratio, '''int''' impact_table_number, '''int''' min_radius, '''int''' max_radius, table('''int''' => {{Type5|PlayerID}}) plot_list<b>)</b></code>
<!-- 
PROCESSRESOURCELIST
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|AssignStartingPlots}}:{{Func5|AssignStartingPlots|ProcessResourceList}}<b>(</b>'''int''' frequency, '''int''' impact_table_number, table('''int''' => '''int''') plot_list, table('''int''' => table('''int''' => {{Type5|ResourceType}})) resources_to_place<b>)</b></code>
<!-- 
SETVOIDS
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Button}}:{{Func5|UIElement|SetVoids}}<b>(</b>{{Type5|PlayerID}} building, {{Type5|UnitID}} addToList<b>)</b></code>
<!-- 
SETVOID1
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|CheckBox}}:{{Func5|UIElement|SetVoid1}}<b>(</b>{{Type5|PlayerID}} i<b>)</b></code>
<!-- 
GETORIGINALOWNER
-->
|-
|align="right" width="200" |<code>{{Type5|PlayerID}}</code>
|style="padding-left:6px" |<code>{{Type5|City}}:{{Func5|City|GetOriginalOwner}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETOWNER
-->
|-
|align="right" width="200" |<code>{{Type5|PlayerID}}</code>
|style="padding-left:6px" |<code>{{Type5|City}}:{{Func5|City|GetOwner}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETPREVIOUSOWNER
-->
|-
|align="right" width="200" |<code>{{Type5|PlayerID}}</code>
|style="padding-left:6px" |<code>{{Type5|City}}:{{Func5|City|GetPreviousOwner}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ISEVEROWNED
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|City}}:{{Func5|City|IsEverOwned}}<b>(</b>{{Type5|PlayerID}} index<b>)</b></code>
<!-- 
BUILDINSTANCEFORCONTROL
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Context}}:{{Func5|UIElement|BuildInstanceForControl}}<b>(</b>'''string''' arg0, '''table''' arg1, {{Type5|Stack}} arg2<b>)</b></code>
<!-- 
ADDALLOWEMBASSY
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Deal}}:{{Func5|Deal|AddAllowEmbassy}}<b>(</b>{{Type5|PlayerID}} us<b>)</b></code>
<!-- 
ADDCITYTRADE
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Deal}}:{{Func5|Deal|AddCityTrade}}<b>(</b>{{Type5|PlayerID}} player, {{Type5|ResourceType}} city<b>)</b></code>
<!-- 
ADDDECLARATIONOFFRIENDSHIP
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Deal}}:{{Func5|Deal|AddDeclarationOfFriendship}}<b>(</b>{{Type5|PlayerID}} us<b>)</b></code>
<!-- 
ADDDEFENSIVEPACT
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Deal}}:{{Func5|Deal|AddDefensivePact}}<b>(</b>{{Type5|PlayerID}} us, {{Type5|ResourceType}} dealDuration<b>)</b></code>
<!-- 
ADDGOLDPERTURNTRADE
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Deal}}:{{Func5|Deal|AddGoldPerTurnTrade}}<b>(</b>{{Type5|PlayerID}} us, '''int''' goldPerTurn, {{Type5|ResourceType}} dealDuration<b>)</b></code>
<!-- 
ADDGOLDTRADE
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Deal}}:{{Func5|Deal|AddGoldTrade}}<b>(</b>{{Type5|PlayerID}} us, '''int''' amount<b>)</b></code>
<!-- 
ADDOPENBORDERS
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Deal}}:{{Func5|Deal|AddOpenBorders}}<b>(</b>{{Type5|PlayerID}} us, {{Type5|ResourceType}} dealDuration<b>)</b></code>
<!-- 
ADDPEACETREATY
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Deal}}:{{Func5|Deal|AddPeaceTreaty}}<b>(</b>{{Type5|PlayerID}} us, '''int''' arg1<b>)</b></code>
<!-- 
ADDRESEARCHAGREEMENT
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Deal}}:{{Func5|Deal|AddResearchAgreement}}<b>(</b>{{Type5|PlayerID}} us, {{Type5|ResourceType}} dealDuration<b>)</b></code>
<!-- 
ADDRESOURCETRADE
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Deal}}:{{Func5|Deal|AddResourceTrade}}<b>(</b>{{Type5|PlayerID}} us, {{Type5|ResourceType}} resource, '''int''' amount, {{Type5|ResourceType}} dealDuration<b>)</b></code>
<!-- 
ADDTHIRDPARTYPEACE
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Deal}}:{{Func5|Deal|AddThirdPartyPeace}}<b>(</b>{{Type5|PlayerID}} who, {{Type5|TeamID}} otherPlayer, '''int''' arg2<b>)</b></code>
<!-- 
ADDTHIRDPARTYWAR
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Deal}}:{{Func5|Deal|AddThirdPartyWar}}<b>(</b>{{Type5|PlayerID}} who, {{Type5|TeamID}} otherPlayer<b>)</b></code>
<!-- 
ADDTRADEAGREEMENT
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Deal}}:{{Func5|Deal|AddTradeAgreement}}<b>(</b>{{Type5|PlayerID}} us, {{Type5|ResourceType}} dealDuration<b>)</b></code>
<!-- 
CHANGEGOLDPERTURNTRADE
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Deal}}:{{Func5|Deal|ChangeGoldPerTurnTrade}}<b>(</b>{{Type5|PlayerID}} us, '''int''' goldPerTurn, {{Type5|ResourceType}} dealDuration<b>)</b></code>
<!-- 
CHANGEGOLDTRADE
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Deal}}:{{Func5|Deal|ChangeGoldTrade}}<b>(</b>{{Type5|PlayerID}} us, '''int''' gold<b>)</b></code>
<!-- 
CHANGERESOURCETRADE
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Deal}}:{{Func5|Deal|ChangeResourceTrade}}<b>(</b>{{Type5|PlayerID}} us, {{Type5|ResourceType}} resource, '''int''' numResource, {{Type5|ResourceType}} dealDuration<b>)</b></code>
<!-- 
GETGOLDAVAILABLE
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Deal}}:{{Func5|Deal|GetGoldAvailable}}<b>(</b>{{Type5|PlayerID}} us, {{Type5|TradeableItemType}} itemToBeChanged<b>)</b></code>
<!-- 
GETNEXTITEM
-->
|-
|align="right" width="200" |<code>{{Type5|TradeableItemType}}, '''unknown''', '''unknown''', {{Type5|ResourceType}}, '''int''', {{Type5|PlayerID}}</code>
|style="padding-left:6px" |<code>{{Type5|Deal}}:{{Func5|Deal|GetNextItem}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETNUMRESOURCE
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Deal}}:{{Func5|Deal|GetNumResource}}<b>(</b>{{Type5|PlayerID}} us, {{Type5|ResourceType}} resType<b>)</b></code>
<!-- 
GETOTHERPLAYER
-->
|-
|align="right" width="200" |<code>{{Type5|PlayerID}}</code>
|style="padding-left:6px" |<code>{{Type5|Deal}}:{{Func5|Deal|GetOtherPlayer}}<b>(</b>{{Type5|PlayerID}} player<b>)</b></code>
<!-- 
ISPOSSIBLETOTRADEITEM
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Deal}}:{{Func5|Deal|IsPossibleToTradeItem}}<b>(</b>{{Type5|PlayerID}} us, {{Type5|PlayerID}} them, {{Type5|TradeableItemType}} tradeType, {{Type5|TeamID}} dealDuration, {{Type5|ResourceType}} dealDuration = nil<b>)</b></code>
<!-- 
REMOVEBYTYPE
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Deal}}:{{Func5|Deal|RemoveByType}}<b>(</b>{{Type5|TradeableItemType}} arg0, {{Type5|PlayerID}} us<b>)</b></code>
<!-- 
REMOVETHIRDPARTYPEACE
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Deal}}:{{Func5|Deal|RemoveThirdPartyPeace}}<b>(</b>{{Type5|PlayerID}} firstParty, {{Type5|TeamID}} otherPlayer<b>)</b></code>
<!-- 
REMOVETHIRDPARTYWAR
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Deal}}:{{Func5|Deal|RemoveThirdPartyWar}}<b>(</b>{{Type5|PlayerID}} firstParty, {{Type5|TeamID}} otherPlayer<b>)</b></code>
<!-- 
SETFROMPLAYER
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Deal}}:{{Func5|Deal|SetFromPlayer}}<b>(</b>{{Type5|PlayerID}} us<b>)</b></code>
<!-- 
SETTOPLAYER
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Deal}}:{{Func5|Deal|SetToPlayer}}<b>(</b>{{Type5|PlayerID}} them<b>)</b></code>
<!-- 
AILEADERMESSAGE
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Events}}.{{Func5|Events|AILeaderMessage}}<b>(</b>{{Type5|PlayerID}} player, {{Type5|DiploUIStateType}} diploUIState, '''string''' leaderMessage, '''int''' animationAction, '''int''' data1<b>)</b></code>
<!-- 
CONNECTEDTONETWORKHOST
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Events}}.{{Func5|Events|ConnectedToNetworkHost}}<b>(</b>{{Type5|PlayerID}} player<b>)</b></code>
<!-- 
ENDCOMBATSIM
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Events}}.{{Func5|Events|EndCombatSim}}<b>(</b>{{Type5|PlayerID}} attackingPlayer, {{Type5|UnitID}} attackingUnit, '''int''' attackingUnitDamage, '''int''' attackingUnitFinalDamage, '''int''' attackingUnitMaxHitPoints, {{Type5|PlayerID}} defendingPlayer, {{Type5|UnitID}} defendingUnit, '''int''' defendingUnitDamage, '''int''' defendingUnitFinalDamage, '''int''' defendingUnitMaxHitPoints<b>)</b></code>
<!-- 
GAMEMESSAGECHAT
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Events}}.{{Func5|Events|GameMessageChat}}<b>(</b>{{Type5|PlayerID}} fromPlayer, {{Type5|PlayerID}} toPlayer, '''string''' text, {{Type5|ChatTargetType}} targetType<b>)</b></code>
<!-- 
GAMEPLAYSETACTIVEPLAYER
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Events}}.{{Func5|Events|GameplaySetActivePlayer}}<b>(</b>{{Type5|PlayerID}} activePlayer, '''int''' prevActivePlayer<b>)</b></code>
<!-- 
INITCITYRANGESTRIKE
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Events}}.{{Func5|Events|InitCityRangeStrike}}<b>(</b>{{Type5|PlayerID}} Player, {{Type5|CityID}} CityID<b>)</b></code>
<!-- 
LOCALMACHINEUNITPOSITIONCHANGED
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Events}}.{{Func5|Events|LocalMachineUnitPositionChanged}}<b>(</b>{{Type5|PlayerID}} player, {{Type5|UnitID}} unitID, {{Type5|Vector3}} unitPosition<b>)</b></code>
<!-- 
MULTIPLAYERGAMEPLAYERDISCONNECTED
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Events}}.{{Func5|Events|MultiplayerGamePlayerDisconnected}}<b>(</b>{{Type5|PlayerID}} player<b>)</b></code>
<!-- 
OPENPLAYERDEALSCREENEVENT
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Events}}.{{Func5|Events|OpenPlayerDealScreenEvent}}<b>(</b>{{Type5|PlayerID}} player, '''int''' target = nil<b>)</b></code>
<!-- 
PLAYERVERSIONMISMATCHEVENT
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Events}}.{{Func5|Events|PlayerVersionMismatchEvent}}<b>(</b>{{Type5|PlayerID}} player, '''unknown''' playerName, '''bool''' isHost<b>)</b></code>
<!-- 
RUNCOMBATSIM
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Events}}.{{Func5|Events|RunCombatSim}}<b>(</b>{{Type5|PlayerID}} attackingPlayer, {{Type5|UnitID}} attackingUnit, '''int''' attackingUnitDamage, '''int''' attackingUnitFinalDamage, '''int''' attackingUnitMaxHitPoints, {{Type5|PlayerID}} defendingPlayer, {{Type5|UnitID}} defendingUnit, '''int''' defendingUnitDamage, '''int''' defendingUnitFinalDamage, '''int''' defendingUnitMaxHitPoints<b>)</b></code>
<!-- 
SERIALEVENTCITYCAPTURED
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Events}}.{{Func5|Events|SerialEventCityCaptured}}<b>(</b>{{Type5|Vector2}} hexPos, {{Type5|PlayerID}} player, '''int''' cityID, {{Type5|PlayerID}} newPlayer<b>)</b></code>
<!-- 
SERIALEVENTCITYCREATED
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Events}}.{{Func5|Events|SerialEventCityCreated}}<b>(</b>{{Type5|Vector2}} vHexPos, {{Type5|PlayerID}} player, {{Type5|CityID}} cityID, {{Type5|ArtStyleType}} artStyleType, {{Type5|EraType}} eraType, '''int''' continent, '''int''' populationSize, '''int''' size, '''int''' fogState<b>)</b></code>
<!-- 
SERIALEVENTCITYDESTROYED
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Events}}.{{Func5|Events|SerialEventCityDestroyed}}<b>(</b>{{Type5|Vector2}} hexPos, {{Type5|PlayerID}} player, '''int''' cityID, {{Type5|PlayerID}} newPlayer<b>)</b></code>
<!-- 
SERIALEVENTCITYSETDAMAGE
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Events}}.{{Func5|Events|SerialEventCitySetDamage}}<b>(</b>{{Type5|PlayerID}} player, {{Type5|CityID}} cityID, '''int''' damage, '''int''' previousDamage<b>)</b></code>
<!-- 
SERIALEVENTERACHANGED
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Events}}.{{Func5|Events|SerialEventEraChanged}}<b>(</b>'''int''' arg0, {{Type5|PlayerID}} currPlayer<b>)</b></code>
<!-- 
SERIALEVENTHEXCULTURECHANGED
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Events}}.{{Func5|Events|SerialEventHexCultureChanged}}<b>(</b>'''int''' hexX, '''int''' hexY, {{Type5|PlayerID}} player, '''bool''' unknown<b>)</b></code>
<!-- 
SERIALEVENTIMPROVEMENTCREATED
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Events}}.{{Func5|Events|SerialEventImprovementCreated}}<b>(</b>'''float''' hexX, '''int''' hexY, {{Type5|ArtStyleType}} continent1, {{Type5|ArtStyleType}} continent2, {{Type5|PlayerID}} player, '''int''' createImprovementType, {{Type5|ImprovementType}} createImprovementRRType, '''int''' createImprovementEra, '''int''' createImprovementState, '''unknown''' ImprovementEra = nil<b>)</b></code>
<!-- 
SERIALEVENTRAWRESOURCECREATED
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Events}}.{{Func5|Events|SerialEventRawResourceCreated}}<b>(</b>'''float''' hexX, '''int''' hexY, {{Type5|ArtStyleType}} continent, {{Type5|ArtStyleType}} continent, {{Type5|PlayerID}} player, '''int''' arg5, '''int''' createResourceType, '''int''' arg7, '''int''' arg8<b>)</b></code>
<!-- 
SERIALEVENTROADCREATED
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Events}}.{{Func5|Events|SerialEventRoadCreated}}<b>(</b>'''int''' hexX, '''int''' hexY, {{Type5|PlayerID}} player, '''int''' routeType<b>)</b></code>
<!-- 
SERIALEVENTUNITCREATED
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Events}}.{{Func5|Events|SerialEventUnitCreated}}<b>(</b>{{Type5|PlayerID}} player, {{Type5|UnitID}} unitID, '''int''' hexVec, '''int''' unitType, '''int''' cultureType, '''int''' civID, '''int''' primaryColor, '''int''' secondaryColor, '''int''' unitFlagIndex, '''int''' fogState<b>)</b></code>
<!-- 
SERIALEVENTUNITDESTROYED
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Events}}.{{Func5|Events|SerialEventUnitDestroyed}}<b>(</b>{{Type5|PlayerID}} player, {{Type5|UnitID}} unitID<b>)</b></code>
<!-- 
SERIALEVENTUNITFLAGSELECTED
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Events}}.{{Func5|Events|SerialEventUnitFlagSelected}}<b>(</b>{{Type5|PlayerID}} player, {{Type5|HandicapType}} unit<b>)</b></code>
<!-- 
SERIALEVENTUNITSETDAMAGE
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Events}}.{{Func5|Events|SerialEventUnitSetDamage}}<b>(</b>{{Type5|PlayerID}} player, {{Type5|UnitID}} unitID, '''int''' damage, '''int''' previousDamage<b>)</b></code>
<!-- 
SERIALEVENTUNITTELEPORTEDTOHEX
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Events}}.{{Func5|Events|SerialEventUnitTeleportedToHex}}<b>(</b>'''unknown''' i, '''unknown''' j, {{Type5|PlayerID}} player, {{Type5|UnitID}} unitID<b>)</b></code>
<!-- 
SHOWATTACKTARGETS
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Events}}.{{Func5|Events|ShowAttackTargets}}<b>(</b>{{Type5|PlayerID}} player, {{Type5|UnitID}} arg1<b>)</b></code>
<!-- 
SHOWMOVEMENTRANGE
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Events}}.{{Func5|Events|ShowMovementRange}}<b>(</b>{{Type5|PlayerID}} player, {{Type5|UnitID}} arg1<b>)</b></code>
<!-- 
SPECIFICCITYINFODIRTY
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Events}}.{{Func5|Events|SpecificCityInfoDirty}}<b>(</b>{{Type5|PlayerID}} player, {{Type5|CityID}} cityID, {{Type5|CityUpdateType}} updateType<b>)</b></code>
<!-- 
UNITACTIONCHANGED
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Events}}.{{Func5|Events|UnitActionChanged}}<b>(</b>{{Type5|PlayerID}} player, {{Type5|UnitID}} unitID<b>)</b></code>
<!-- 
UNITEMBARK
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Events}}.{{Func5|Events|UnitEmbark}}<b>(</b>{{Type5|PlayerID}} player, {{Type5|UnitID}} unitID<b>)</b></code>
<!-- 
UNITGARRISON
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Events}}.{{Func5|Events|UnitGarrison}}<b>(</b>{{Type5|PlayerID}} player, {{Type5|UnitID}} unitID, '''int''' garrisoned<b>)</b></code>
<!-- 
UNITMARKTHREATENING
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Events}}.{{Func5|Events|UnitMarkThreatening}}<b>(</b>{{Type5|PlayerID}} player, {{Type5|UnitID}} unitID, '''bool''' mark<b>)</b></code>
<!-- 
UNITMEMBERCOMBATSTATECHANGED
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Events}}.{{Func5|Events|UnitMemberCombatStateChanged}}<b>(</b>{{Type5|PlayerID}} player, {{Type5|UnitID}} unitID, '''int''' memberID, '''unknown''' stateID<b>)</b></code>
<!-- 
UNITMEMBERCOMBATTARGETCHANGED
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Events}}.{{Func5|Events|UnitMemberCombatTargetChanged}}<b>(</b>{{Type5|PlayerID}} player, {{Type5|UnitID}} unitID, '''int''' memberID, '''unknown''' targetPlayerID, '''unknown''' targetUnitID, '''int''' targetMemberID<b>)</b></code>
<!-- 
UNITMEMBEROVERLAYADD
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Events}}.{{Func5|Events|UnitMemberOverlayAdd}}<b>(</b>{{Type5|PlayerID}} player, {{Type5|UnitID}} unitID, '''int''' memberID, '''unknown''' position<b>)</b></code>
<!-- 
UNITMEMBEROVERLAYREMOVE
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Events}}.{{Func5|Events|UnitMemberOverlayRemove}}<b>(</b>{{Type5|PlayerID}} player, {{Type5|UnitID}} unitID, '''int''' memberID<b>)</b></code>
<!-- 
UNITMEMBEROVERLAYSHOWHIDE
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Events}}.{{Func5|Events|UnitMemberOverlayShowHide}}<b>(</b>{{Type5|PlayerID}} player, {{Type5|UnitID}} unitID, '''int''' memberID, '''bool''' show<b>)</b></code>
<!-- 
UNITMEMBERPOSITIONCHANGED
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Events}}.{{Func5|Events|UnitMemberPositionChanged}}<b>(</b>{{Type5|PlayerID}} player, {{Type5|UnitID}} unitID, '''int''' memberID, '''unknown''' unitPosition<b>)</b></code>
<!-- 
UNITMOVEQUEUECHANGED
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Events}}.{{Func5|Events|UnitMoveQueueChanged}}<b>(</b>{{Type5|PlayerID}} player, {{Type5|UnitID}} unitID, '''bool''' remainingMoves<b>)</b></code>
<!-- 
UNITSELECTIONCHANGED
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Events}}.{{Func5|Events|UnitSelectionChanged}}<b>(</b>{{Type5|PlayerID}} player, {{Type5|UnitID}} u, '''float''' hexX, '''float''' hexY, '''int''' k, '''bool''' isSelected, '''bool''' arg6<b>)</b></code>
<!-- 
UNITSHOULDDIMFLAG
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Events}}.{{Func5|Events|UnitShouldDimFlag}}<b>(</b>{{Type5|PlayerID}} player, {{Type5|UnitID}} unitID, '''int''' dim<b>)</b></code>
<!-- 
UNITSTATECHANGEDETECTED
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Events}}.{{Func5|Events|UnitStateChangeDetected}}<b>(</b>{{Type5|PlayerID}} player, {{Type5|UnitID}} unitID, '''int''' fogState<b>)</b></code>
<!-- 
UNITVISIBILITYCHANGED
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Events}}.{{Func5|Events|UnitVisibilityChanged}}<b>(</b>{{Type5|PlayerID}} player, {{Type5|UnitID}} unitID, '''bool''' visible, '''bool''' checkFlag, '''unknown''' blendTime<b>)</b></code>
<!-- 
ADDPLAYER
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Game}}.{{Func5|Game|AddPlayer}}<b>(</b>{{Type5|PlayerID}} newPlayer, {{Type5|LeaderType}} leader, {{Type5|CivilizationType}} civ<b>)</b></code>
<!-- 
DOFROMUIDIPLOEVENT
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Game}}.{{Func5|Game|DoFromUIDiploEvent}}<b>(</b>{{Type5|DiploUIEventType}} event, {{Type5|PlayerID}} aIPlayer, {{Type5|SpecialistType}} button, '''int''' againstPlayer, '''int''' arg3<b>)</b></code>
<!-- 
DOMINORBULLYGOLD
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Game}}.{{Func5|Game|DoMinorBullyGold}}<b>(</b>{{Type5|PlayerID}} activePlayer, {{Type5|PlayerID}} minorCiv<b>)</b></code>
<!-- 
DOMINORBULLYUNIT
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Game}}.{{Func5|Game|DoMinorBullyUnit}}<b>(</b>{{Type5|PlayerID}} activePlayer, {{Type5|PlayerID}} minorCiv<b>)</b></code>
<!-- 
DOMINORBUYOUT
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Game}}.{{Func5|Game|DoMinorBuyout}}<b>(</b>{{Type5|PlayerID}} activePlayer, {{Type5|PlayerID}} minorCiv<b>)</b></code>
<!-- 
DOMINORGIFTTILEIMPROVEMENT
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Game}}.{{Func5|Game|DoMinorGiftTileImprovement}}<b>(</b>{{Type5|PlayerID}} fromPlayer, {{Type5|TaskType}} toPlayer, '''int''' plotX, '''int''' plotY<b>)</b></code>
<!-- 
DOMINORPLEDGEPROTECTION
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Game}}.{{Func5|Game|DoMinorPledgeProtection}}<b>(</b>{{Type5|PlayerID}} activePlayer, {{Type5|PlayerID}} minorCiv, '''bool''' arg2<b>)</b></code>
<!-- 
ENHANCERELIGION
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Game}}.{{Func5|Game|EnhanceReligion}}<b>(</b>{{Type5|PlayerID}} vaticanPlayer, {{Type5|ReligionType}} religion, {{Type5|BeliefType}} belief4, {{Type5|BeliefType}} belief5<b>)</b></code>
<!-- 
FOUNDRELIGION
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Game}}.{{Func5|Game|FoundReligion}}<b>(</b>{{Type5|PlayerID}} vaticanPlayer, {{Type5|ReligionType}} religion, '''unknown''' arg2, {{Type5|BeliefType}} belief2, {{Type5|BeliefType}} belief3, {{Type5|BeliefType}} belief3, '''int''' arg6, {{Type5|City}} vaticanCity<b>)</b></code>
<!-- 
GETACTIVEPLAYER
-->
|-
|align="right" width="200" |<code>{{Type5|PlayerID}}</code>
|style="padding-left:6px" |<code>{{Type5|Game}}.{{Func5|Game|GetActivePlayer}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETFOUNDER
-->
|-
|align="right" width="200" |<code>{{Type5|PlayerID}}</code>
|style="padding-left:6px" |<code>{{Type5|Game}}.{{Func5|Game|GetFounder}}<b>(</b>{{Type5|ReligionType}} arg0, '''int''' arg1<b>)</b></code>
<!-- 
GETFOUNDERBENEFITSRELIGION
-->
|-
|align="right" width="200" |<code>{{Type5|ReligionType}}</code>
|style="padding-left:6px" |<code>{{Type5|Game}}.{{Func5|Game|GetFounderBenefitsReligion}}<b>(</b>{{Type5|PlayerID}} player<b>)</b></code>
<!-- 
GETGAMETURN
-->
|-
|align="right" width="200" |<code>{{Type5|PlayerID}}</code>
|style="padding-left:6px" |<code>{{Type5|Game}}.{{Func5|Game|GetGameTurn}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETHOLYCITYFORRELIGION
-->
|-
|align="right" width="200" |<code>{{Type5|City}}</code>
|style="padding-left:6px" |<code>{{Type5|Game}}.{{Func5|Game|GetHolyCityForReligion}}<b>(</b>{{Type5|ReligionType}} religion, {{Type5|PlayerID}} player<b>)</b></code>
<!-- 
GETNONUKESCOUNT
-->
|-
|align="right" width="200" |<code>{{Type5|PlayerID}}</code>
|style="padding-left:6px" |<code>{{Type5|Game}}.{{Func5|Game|GetNoNukesCount}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETPLAYERRANK
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Game}}.{{Func5|Game|GetPlayerRank}}<b>(</b>{{Type5|PlayerID}} index<b>)</b></code>
<!-- 
GETPLAYERSCORE
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Game}}.{{Func5|Game|GetPlayerScore}}<b>(</b>{{Type5|PlayerID}} index<b>)</b></code>
<!-- 
GETPLAYERVOTE
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Game}}.{{Func5|Game|GetPlayerVote}}<b>(</b>{{Type5|PlayerID}} ownerIndex, '''int''' voteId<b>)</b></code>
<!-- 
GETRANKPLAYER
-->
|-
|align="right" width="200" |<code>{{Type5|PlayerID}}</code>
|style="padding-left:6px" |<code>{{Type5|Game}}.{{Func5|Game|GetRankPlayer}}<b>(</b>'''int''' rank<b>)</b></code>
<!-- 
GETRESEARCHAGREEMENTCOST
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Game}}.{{Func5|Game|GetResearchAgreementCost}}<b>(</b>{{Type5|PlayerID}} us, {{Type5|PlayerID}} them<b>)</b></code>
<!-- 
GETSTARTTURN
-->
|-
|align="right" width="200" |<code>{{Type5|PlayerID}}</code>
|style="padding-left:6px" |<code>{{Type5|Game}}.{{Func5|Game|GetStartTurn}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
SAVEREPLAY
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Game}}.{{Func5|Game|SaveReplay}}<b>(</b>{{Type5|PlayerID}} player<b>)</b></code>
<!-- 
SETACTIVEPLAYER
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Game}}.{{Func5|Game|SetActivePlayer}}<b>(</b>{{Type5|PlayerID}} newValue, '''bool''' forceHotSeat<b>)</b></code>
<!-- 
SETADVISORRECOMMENDERTECH
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Game}}.{{Func5|Game|SetAdvisorRecommenderTech}}<b>(</b>{{Type5|PlayerID}} player<b>)</b></code>
<!-- 
SETFOUNDER
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Game}}.{{Func5|Game|SetFounder}}<b>(</b>{{Type5|ReligionType}} arg0, {{Type5|PlayerID}} newOwner<b>)</b></code>
<!-- 
SETPAUSEPLAYER
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Game}}.{{Func5|Game|SetPausePlayer}}<b>(</b>{{Type5|PlayerID}} arg0<b>)</b></code>
<!-- 
CITYBUILDINGSISBUILDINGSELLABLE
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|GameEvents}}.{{Func5|GameEvents|CityBuildingsIsBuildingSellable}}<b>(</b>{{Type5|PlayerID}} player, {{Type5|BuildingType}} building<b>)</b></code>
<!-- 
CITYCANCONSTRUCT
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|GameEvents}}.{{Func5|GameEvents|CityCanConstruct}}<b>(</b>{{Type5|PlayerID}} player, {{Type5|CityID}} city, {{Type5|BuildingType}} buildingType<b>)</b></code>
<!-- 
CITYCAPTURECOMPLETE
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|GameEvents}}.{{Func5|GameEvents|CityCaptureComplete}}<b>(</b>{{Type5|PlayerID}} player, '''int''' capital, {{Type5|ResourceType}} x, {{Type5|ResourceType}} y, {{Type5|PlayerID}} newPlayer, '''int''' conquest, '''int''' conquest<b>)</b></code>
<!-- 
CITYCONVERTSRELIGION
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|GameEvents}}.{{Func5|GameEvents|CityConvertsReligion}}<b>(</b>{{Type5|PlayerID}} owner, {{Type5|ReligionType}} religion, '''int''' x, '''int''' y<b>)</b></code>
<!-- 
GETFOUNDERBENEFITSRELIGION
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|GameEvents}}.{{Func5|GameEvents|GetFounderBenefitsReligion}}<b>(</b>{{Type5|PlayerID}} player<b>)</b></code>
<!-- 
GETRELIGIONTOSPREAD
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|GameEvents}}.{{Func5|GameEvents|GetReligionToSpread}}<b>(</b>{{Type5|PlayerID}} player<b>)</b></code>
<!-- 
GETSCENARIODIPLOMODIFIER1
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|GameEvents}}.{{Func5|GameEvents|GetScenarioDiploModifier1}}<b>(</b>{{Type5|PlayerID}} player1, {{Type5|PlayerID}} player2<b>)</b></code>
<!-- 
GETSCENARIODIPLOMODIFIER2
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|GameEvents}}.{{Func5|GameEvents|GetScenarioDiploModifier2}}<b>(</b>{{Type5|PlayerID}} player1, {{Type5|PlayerID}} player2<b>)</b></code>
<!-- 
PLAYERADOPTPOLICY
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|GameEvents}}.{{Func5|GameEvents|PlayerAdoptPolicy}}<b>(</b>{{Type5|PlayerID}} player, '''int''' policyID<b>)</b></code>
<!-- 
PLAYERCANADOPTPOLICYBRANCH
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|GameEvents}}.{{Func5|GameEvents|PlayerCanAdoptPolicyBranch}}<b>(</b>{{Type5|PlayerID}} player, '''int''' policyBranch<b>)</b></code>
<!-- 
PLAYERCITYFOUNDED
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|GameEvents}}.{{Func5|GameEvents|PlayerCityFounded}}<b>(</b>{{Type5|PlayerID}} player, '''int''' cityX, '''int''' cityY<b>)</b></code>
<!-- 
PLAYERDOTURN
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|GameEvents}}.{{Func5|GameEvents|PlayerDoTurn}}<b>(</b>{{Type5|PlayerID}} player<b>)</b></code>
<!-- 
PLAYERPREAIUNITUPDATE
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|GameEvents}}.{{Func5|GameEvents|PlayerPreAIUnitUpdate}}<b>(</b>{{Type5|PlayerID}} player<b>)</b></code>
<!-- 
SETALLY
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|GameEvents}}.{{Func5|GameEvents|SetAlly}}<b>(</b>{{Type5|PlayerID}} cSPlayer, {{Type5|PlayerID}} oldAlly, {{Type5|PlayerID}} newAlly<b>)</b></code>
<!-- 
UNITGETSPECIALEXPLORETARGET
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|GameEvents}}.{{Func5|GameEvents|UnitGetSpecialExploreTarget}}<b>(</b>{{Type5|PlayerID}} player, {{Type5|UnitID}} unitID<b>)</b></code>
<!-- 
UNITSETXY
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|GameEvents}}.{{Func5|GameEvents|UnitSetXY}}<b>(</b>{{Type5|PlayerID}} player, {{Type5|UnitID}} unit, '''int''' x, '''int''' y<b>)</b></code>
<!-- 
REGISTERCALLBACK
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Grid}}:{{Func5|UIElement|RegisterCallback}}<b>(</b>{{Type5|MouseType}} thisEvent, ('''void''' func<b>(</b>{{Type5|PlayerID}} void1, {{Type5|ResourceType}} void2, {{Type5|Button}} button<b>)</b>) OnContinueButtonClicked<b>)</b></code>
<!-- 
SETVOIDS
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|GridButton}}:{{Func5|UIElement|SetVoids}}<b>(</b>{{Type5|PlayerID}} player, '''int''' id<b>)</b></code>
<!-- 
PASSWORDCHANGED
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|LuaEvents}}.{{Func5|LuaEvents|PasswordChanged}}<b>(</b>{{Type5|PlayerID}} player<b>)</b></code>
<!-- 
SCENARIOPLAYERSTATUSCHANGED
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|LuaEvents}}.{{Func5|LuaEvents|ScenarioPlayerStatusChanged}}<b>(</b>table({{Type5|PlayerID}} => table('''string''' => '''table''')) tPlayerStatus, {{Type5|PlayerID}} turn, '''int''' year, {{Type5|PlayerID}} playerAboutToWin, '''int''' turnsControlHeld<b>)</b></code>
<!-- 
SCENARIOUNITTIERSCHANGED
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|LuaEvents}}.{{Func5|LuaEvents|ScenarioUnitTiersChanged}}<b>(</b>table('''string''' => {{Type5|PlayerID}}) tUnitTiers<b>)</b></code>
<!-- 
SETCIVNAMEEDITSLOT
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|LuaEvents}}.{{Func5|LuaEvents|SetCivNameEditSlot}}<b>(</b>{{Type5|PlayerID}} slot<b>)</b></code>
<!-- 
GETHOSTID
-->
|-
|align="right" width="200" |<code>{{Type5|PlayerID}}</code>
|style="padding-left:6px" |<code>{{Type5|Matchmaking}}.{{Func5|Matchmaking|GetHostID}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETLOCALID
-->
|-
|align="right" width="200" |<code>{{Type5|PlayerID}}</code>
|style="padding-left:6px" |<code>{{Type5|Matchmaking}}.{{Func5|Matchmaking|GetLocalID}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETPLAYERLIST
-->
|-
|align="right" width="200" |<code>table({{Type5|PlayerID}} => '''table''')</code>
|style="padding-left:6px" |<code>{{Type5|Matchmaking}}.{{Func5|Matchmaking|GetPlayerList}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
KICKPLAYER
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Matchmaking}}.{{Func5|Matchmaking|KickPlayer}}<b>(</b>{{Type5|PlayerID}} player<b>)</b></code>
<!-- 
GETPINGTIME
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Network}}.{{Func5|Network|GetPingTime}}<b>(</b>{{Type5|PlayerID}} player<b>)</b></code>
<!-- 
SENDBARBARIANRANSOM
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Network}}.{{Func5|Network|SendBarbarianRansom}}<b>(</b>'''int''' arg0, {{Type5|PlayerID}} unit<b>)</b></code>
<!-- 
SENDENHANCERELIGION
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Network}}.{{Func5|Network|SendEnhanceReligion}}<b>(</b>{{Type5|PlayerID}} arg0, {{Type5|ReligionType}} CurrentReligion, '''unknown''' customName, '''unknown''' arg3, '''int''' arg4, '''int''' cityX, '''int''' cityY<b>)</b></code>
<!-- 
SENDFAITHGREATPERSONCHOICE
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Network}}.{{Func5|Network|SendFaithGreatPersonChoice}}<b>(</b>{{Type5|PlayerID}} player, '''unknown''' arg1<b>)</b></code>
<!-- 
SENDFAITHPURCHASE
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Network}}.{{Func5|Network|SendFaithPurchase}}<b>(</b>{{Type5|PlayerID}} arg0, {{Type5|FaithPurchaseType}} v1, '''int''' v2<b>)</b></code>
<!-- 
SENDFOUNDPANTHEON
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Network}}.{{Func5|Network|SendFoundPantheon}}<b>(</b>{{Type5|PlayerID}} arg0, {{Type5|BeliefType}} Belief<b>)</b></code>
<!-- 
SENDFOUNDRELIGION
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Network}}.{{Func5|Network|SendFoundReligion}}<b>(</b>{{Type5|PlayerID}} arg0, {{Type5|ReligionType}} CurrentReligion, '''unknown''' customName, '''unknown''' arg3, '''unknown''' arg4, {{Type5|BeliefType}} arg5, {{Type5|BeliefType}} arg6, '''int''' cityX, '''int''' cityY<b>)</b></code>
<!-- 
SENDGREATPERSONCHOICE
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Network}}.{{Func5|Network|SendGreatPersonChoice}}<b>(</b>{{Type5|PlayerID}} player, '''unknown''' arg1<b>)</b></code>
<!-- 
SENDMAYABONUSCHOICE
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Network}}.{{Func5|Network|SendMayaBonusChoice}}<b>(</b>{{Type5|PlayerID}} player, '''unknown''' arg1<b>)</b></code>
<!-- 
SENDMINORNOUNITSPAWNING
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Network}}.{{Func5|Network|SendMinorNoUnitSpawning}}<b>(</b>{{Type5|PlayerID}} minorCiv, '''bool''' arg1<b>)</b></code>
<!-- 
SENDMOVESPY
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Network}}.{{Func5|Network|SendMoveSpy}}<b>(</b>{{Type5|PlayerID}} arg0, '''unknown''' SelectedAgentID, {{Type5|PlayerID}} arg2, '''int''' arg3<b>)</b></code>
<!-- 
SENDPLEDGEMINORPROTECTION
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Network}}.{{Func5|Network|SendPledgeMinorProtection}}<b>(</b>{{Type5|PlayerID}} minorCiv, '''bool''' arg1<b>)</b></code>
<!-- 
SENDRESEARCH
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Network}}.{{Func5|Network|SendResearch}}<b>(</b>{{Type5|PlayerID}} tech, {{Type5|ResourceType}} discover, '''int''' value, '''bool''' arg3 = nil<b>)</b></code>
<!-- 
SENDSTAGECOUP
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Network}}.{{Func5|Network|SendStageCoup}}<b>(</b>{{Type5|PlayerID}} arg0, '''unknown''' arg1<b>)</b></code>
<!-- 
ADDNOTIFICATION
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|AddNotification}}<b>(</b>{{Type5|NotificationType}} notificationType, '''string''' description, '''string''' title, '''int''' x = -1, '''int''' y = -1, {{Type5|PlayerID}} extra1 = -1, '''int''' extra2 = -1<b>)</b></code>
<!-- 
CANCONTACT
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|CanContact}}<b>(</b>{{Type5|PlayerID}} player<b>)</b></code>
<!-- 
CANMAJORBULLYGOLD
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|CanMajorBullyGold}}<b>(</b>{{Type5|PlayerID}} major<b>)</b></code>
<!-- 
CANMAJORBULLYUNIT
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|CanMajorBullyUnit}}<b>(</b>{{Type5|PlayerID}} activePlayer<b>)</b></code>
<!-- 
CANMAJORBUYOUT
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|CanMajorBuyout}}<b>(</b>{{Type5|PlayerID}} activePlayer<b>)</b></code>
<!-- 
CANMAJORGIFTTILEIMPROVEMENT
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|CanMajorGiftTileImprovement}}<b>(</b>{{Type5|PlayerID}} activePlayer<b>)</b></code>
<!-- 
CANMAJORGIFTTILEIMPROVEMENTATPLOT
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|CanMajorGiftTileImprovementAtPlot}}<b>(</b>{{Type5|PlayerID}} fromPlayer, '''int''' plotX, '''int''' plotY<b>)</b></code>
<!-- 
CANMAJORSTARTPROTECTION
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|CanMajorStartProtection}}<b>(</b>{{Type5|PlayerID}} activePlayer<b>)</b></code>
<!-- 
CANMAJORWITHDRAWPROTECTION
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|CanMajorWithdrawProtection}}<b>(</b>{{Type5|PlayerID}} activePlayer<b>)</b></code>
<!-- 
CANTRADEWITH
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|CanTradeWith}}<b>(</b>{{Type5|PlayerID}} whoTo<b>)</b></code>
<!-- 
CHANGEMINORCIVFRIENDSHIPWITHMAJOR
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|ChangeMinorCivFriendshipWithMajor}}<b>(</b>{{Type5|PlayerID}} player<b>)</b></code>
<!-- 
CONTACT
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|Contact}}<b>(</b>{{Type5|PlayerID}} player<b>)</b></code>
<!-- 
DOFORCEDENOUNCE
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|DoForceDenounce}}<b>(</b>{{Type5|PlayerID}} player<b>)</b></code>
<!-- 
DOFORCEDOF
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|DoForceDoF}}<b>(</b>{{Type5|PlayerID}} player<b>)</b></code>
<!-- 
DOMINORLIBERATIONBYMAJOR
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|DoMinorLiberationByMajor}}<b>(</b>{{Type5|PlayerID}} player<b>)</b></code>
<!-- 
DOUPDATEPROXIMITYTOPLAYER
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|DoUpdateProximityToPlayer}}<b>(</b>{{Type5|PlayerID}} player<b>)</b></code>
<!-- 
FORCEPEACE
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|ForcePeace}}<b>(</b>{{Type5|PlayerID}} player<b>)</b></code>
<!-- 
GETACTIVEQUESTFORPLAYER
-->
|-
|align="right" width="200" |<code>{{Type5|MinorCivQuestType}}</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|GetActiveQuestForPlayer}}<b>(</b>{{Type5|PlayerID}} player<b>)</b></code>
<!-- 
GETALLY
-->
|-
|align="right" width="200" |<code>{{Type5|PlayerID}}</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|GetAlly}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETAPPROACHTOWARDSUSGUESS
-->
|-
|align="right" width="200" |<code>{{Type5|MajorCivApproachType}}</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|GetApproachTowardsUsGuess}}<b>(</b>{{Type5|PlayerID}} player<b>)</b></code>
<!-- 
GETBUYOUTCOST
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|GetBuyoutCost}}<b>(</b>{{Type5|PlayerID}} activePlayer<b>)</b></code>
<!-- 
GETCOMMONFOEVALUE
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|GetCommonFoeValue}}<b>(</b>{{Type5|PlayerID}} activePlayer<b>)</b></code>
<!-- 
GETCOOPWARACCEPTEDSTATE
-->
|-
|align="right" width="200" |<code>{{Type5|CoopWarState}}</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|GetCoopWarAcceptedState}}<b>(</b>{{Type5|PlayerID}} withPlayer, {{Type5|PlayerID}} againstPlayer<b>)</b></code>
<!-- 
GETCURRENTCAPITALFOODBONUS
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|GetCurrentCapitalFoodBonus}}<b>(</b>{{Type5|PlayerID}} major<b>)</b></code>
<!-- 
GETCURRENTCULTUREBONUS
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|GetCurrentCultureBonus}}<b>(</b>{{Type5|PlayerID}} activePlayer<b>)</b></code>
<!-- 
GETCURRENTOTHERCITYFOODBONUS
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|GetCurrentOtherCityFoodBonus}}<b>(</b>{{Type5|PlayerID}} major<b>)</b></code>
<!-- 
GETCURRENTSCIENCEFRIENDSHIPBONUSTIMES100
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|GetCurrentScienceFriendshipBonusTimes100}}<b>(</b>{{Type5|PlayerID}} major<b>)</b></code>
<!-- 
GETCURRENTSPAWNESTIMATE
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|GetCurrentSpawnEstimate}}<b>(</b>{{Type5|PlayerID}} major<b>)</b></code>
<!-- 
GETEXTRABUILDINGHAPPINESSFROMPOLICIES
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|GetExtraBuildingHappinessFromPolicies}}<b>(</b>{{Type5|PlayerID}} building<b>)</b></code>
<!-- 
GETFRIENDSHIPCHANGEPERTURNTIMES100
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|GetFriendshipChangePerTurnTimes100}}<b>(</b>{{Type5|PlayerID}} major<b>)</b></code>
<!-- 
GETFRIENDSHIPFROMGOLDGIFT
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|GetFriendshipFromGoldGift}}<b>(</b>{{Type5|PlayerID}} activePlayer, '''int''' gold<b>)</b></code>
<!-- 
GETGIFTTILEIMPROVEMENTCOST
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|GetGiftTileImprovementCost}}<b>(</b>{{Type5|PlayerID}} activePlayer<b>)</b></code>
<!-- 
GETHAPPINESSFROMMINOR
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|GetHappinessFromMinor}}<b>(</b>{{Type5|PlayerID}} minor<b>)</b></code>
<!-- 
GETID
-->
|-
|align="right" width="200" |<code>{{Type5|PlayerID}}</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|GetID}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETLANDDISPUTELEVEL
-->
|-
|align="right" width="200" |<code>{{Type5|DisputeLevelType}}</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|GetLandDisputeLevel}}<b>(</b>{{Type5|PlayerID}} activePlayer<b>)</b></code>
<!-- 
GETMINORCIVBULLYGOLDAMOUNT
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|GetMinorCivBullyGoldAmount}}<b>(</b>{{Type5|PlayerID}} activePlayer<b>)</b></code>
<!-- 
GETMINORCIVCONTESTVALUEFORPLAYER
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|GetMinorCivContestValueForPlayer}}<b>(</b>{{Type5|PlayerID}} major, {{Type5|MinorCivQuestType}} arg1<b>)</b></code>
<!-- 
GETMINORCIVCURRENTCULTUREBONUS
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|GetMinorCivCurrentCultureBonus}}<b>(</b>{{Type5|PlayerID}} major<b>)</b></code>
<!-- 
GETMINORCIVCURRENTFAITHBONUS
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|GetMinorCivCurrentFaithBonus}}<b>(</b>{{Type5|PlayerID}} major<b>)</b></code>
<!-- 
GETMINORCIVCURRENTHAPPINESSBONUS
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|GetMinorCivCurrentHappinessBonus}}<b>(</b>{{Type5|PlayerID}} major<b>)</b></code>
<!-- 
GETMINORCIVDISPUTELEVEL
-->
|-
|align="right" width="200" |<code>{{Type5|DisputeLevelType}}</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|GetMinorCivDisputeLevel}}<b>(</b>{{Type5|PlayerID}} activePlayer<b>)</b></code>
<!-- 
GETMINORCIVFRIENDSHIPANCHORWITHMAJOR
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|GetMinorCivFriendshipAnchorWithMajor}}<b>(</b>{{Type5|PlayerID}} major<b>)</b></code>
<!-- 
GETMINORCIVFRIENDSHIPLEVELWITHMAJOR
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|GetMinorCivFriendshipLevelWithMajor}}<b>(</b>{{Type5|PlayerID}} arg0<b>)</b></code>
<!-- 
GETMINORCIVFRIENDSHIPWITHMAJOR
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|GetMinorCivFriendshipWithMajor}}<b>(</b>{{Type5|PlayerID}} major<b>)</b></code>
<!-- 
GETMINORCIVNUMACTIVEQUESTSFORPLAYER
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|GetMinorCivNumActiveQuestsForPlayer}}<b>(</b>{{Type5|PlayerID}} player<b>)</b></code>
<!-- 
GETNUMCIVILIANSRETURNEDTOME
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|GetNumCiviliansReturnedToMe}}<b>(</b>{{Type5|PlayerID}} activePlayer<b>)</b></code>
<!-- 
GETNUMREQUESTSREFUSED
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|GetNumRequestsRefused}}<b>(</b>{{Type5|PlayerID}} activePlayer<b>)</b></code>
<!-- 
GETNUMTIMESCULTUREBOMBED
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|GetNumTimesCultureBombed}}<b>(</b>{{Type5|PlayerID}} activePlayer<b>)</b></code>
<!-- 
GETNUMTRADERESOURCEIMPORTS
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|GetNumTradeResourceImports}}<b>(</b>{{Type5|PlayerID}} player<b>)</b></code>
<!-- 
GETNUMWARSFOUGHT
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|GetNumWarsFought}}<b>(</b>{{Type5|PlayerID}} otherPlayer<b>)</b></code>
<!-- 
GETOPINIONTABLE
-->
|-
|align="right" width="200" |<code>table('''unknown''' => '''unknown''')</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|GetOpinionTable}}<b>(</b>{{Type5|PlayerID}} activePlayer<b>)</b></code>
<!-- 
GETOTHERPLAYERNUMPROTECTEDMINORSATTACKED
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|GetOtherPlayerNumProtectedMinorsAttacked}}<b>(</b>{{Type5|PlayerID}} activePlayer<b>)</b></code>
<!-- 
GETOTHERPLAYERNUMPROTECTEDMINORSKILLED
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|GetOtherPlayerNumProtectedMinorsKilled}}<b>(</b>{{Type5|PlayerID}} activePlayer<b>)</b></code>
<!-- 
GETPROXIMITYTOPLAYER
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|GetProximityToPlayer}}<b>(</b>{{Type5|PlayerID}} index<b>)</b></code>
<!-- 
GETQUESTDATA1
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|GetQuestData1}}<b>(</b>{{Type5|PlayerID}} major, {{Type5|MinorCivQuestType}} type = nil<b>)</b></code>
<!-- 
GETQUESTDATA2
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|GetQuestData2}}<b>(</b>{{Type5|PlayerID}} major, {{Type5|MinorCivQuestType}} type = nil<b>)</b></code>
<!-- 
GETQUESTTURNSREMAINING
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|GetQuestTurnsRemaining}}<b>(</b>{{Type5|PlayerID}} major, {{Type5|MinorCivQuestType}} type, {{Type5|PlayerID}} arg2<b>)</b></code>
<!-- 
GETRECENTASSISTVALUE
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|GetRecentAssistValue}}<b>(</b>{{Type5|PlayerID}} activePlayer<b>)</b></code>
<!-- 
GETRECENTINTRIGUEINFO
-->
|-
|align="right" width="200" |<code>{{Type5|SpecialistType}}, '''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|GetRecentIntrigueInfo}}<b>(</b>{{Type5|PlayerID}} aIPlayer<b>)</b></code>
<!-- 
GETRECENTTRADEVALUE
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|GetRecentTradeValue}}<b>(</b>{{Type5|PlayerID}} activePlayer<b>)</b></code>
<!-- 
GETTEAM
-->
|-
|align="right" width="200" |<code>{{Type5|PlayerID}}</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|GetTeam}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETTURNLASTPLEDGEBROKENBYMAJOR
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|GetTurnLastPledgeBrokenByMajor}}<b>(</b>{{Type5|PlayerID}} activePlayer<b>)</b></code>
<!-- 
GETTURNLASTPLEDGEDPROTECTIONBYMAJOR
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|GetTurnLastPledgedProtectionByMajor}}<b>(</b>{{Type5|PlayerID}} activePlayer<b>)</b></code>
<!-- 
GETWARMONGERTHREAT
-->
|-
|align="right" width="200" |<code>{{Type5|ThreatType}}</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|GetWarmongerThreat}}<b>(</b>{{Type5|PlayerID}} activePlayer<b>)</b></code>
<!-- 
GETWONDERDISPUTELEVEL
-->
|-
|align="right" width="200" |<code>{{Type5|DisputeLevelType}}</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|GetWonderDisputeLevel}}<b>(</b>{{Type5|PlayerID}} activePlayer<b>)</b></code>
<!-- 
HASRECENTINTRIGUEABOUT
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|HasRecentIntrigueAbout}}<b>(</b>{{Type5|PlayerID}} player<b>)</b></code>
<!-- 
ISALLIES
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|IsAllies}}<b>(</b>{{Type5|PlayerID}} major<b>)</b></code>
<!-- 
ISCAPITALCAPTUREDBY
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|IsCapitalCapturedBy}}<b>(</b>{{Type5|PlayerID}} activePlayer<b>)</b></code>
<!-- 
ISDEMANDEVERMADE
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|IsDemandEverMade}}<b>(</b>{{Type5|PlayerID}} activePlayer<b>)</b></code>
<!-- 
ISDENOUNCEDPLAYER
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|IsDenouncedPlayer}}<b>(</b>{{Type5|PlayerID}} otherPlayer<b>)</b></code>
<!-- 
ISDENOUNCINGPLAYER
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|IsDenouncingPlayer}}<b>(</b>{{Type5|PlayerID}} player<b>)</b></code>
<!-- 
ISDOF
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|IsDoF}}<b>(</b>{{Type5|PlayerID}} otherPlayer<b>)</b></code>
<!-- 
ISDOFMESSAGETOOSOON
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|IsDoFMessageTooSoon}}<b>(</b>{{Type5|PlayerID}} activePlayer<b>)</b></code>
<!-- 
ISDONTSETTLEMESSAGETOOSOON
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|IsDontSettleMessageTooSoon}}<b>(</b>{{Type5|PlayerID}} withPlayer<b>)</b></code>
<!-- 
ISFRIENDDECLAREDWARONUS
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|IsFriendDeclaredWarOnUs}}<b>(</b>{{Type5|PlayerID}} activePlayer<b>)</b></code>
<!-- 
ISFRIENDDENOUNCEDUS
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|IsFriendDenouncedUs}}<b>(</b>{{Type5|PlayerID}} activePlayer<b>)</b></code>
<!-- 
ISFRIENDS
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|IsFriends}}<b>(</b>{{Type5|PlayerID}} major = nil<b>)</b></code>
<!-- 
ISGAVEASSISTANCETO
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|IsGaveAssistanceTo}}<b>(</b>{{Type5|PlayerID}} activePlayer<b>)</b></code>
<!-- 
ISHASPAIDTRIBUTETO
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|IsHasPaidTributeTo}}<b>(</b>{{Type5|PlayerID}} activePlayer<b>)</b></code>
<!-- 
ISLIBERATEDCAPITAL
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|IsLiberatedCapital}}<b>(</b>{{Type5|PlayerID}} activePlayer<b>)</b></code>
<!-- 
ISLIBERATEDCITY
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|IsLiberatedCity}}<b>(</b>{{Type5|PlayerID}} activePlayer<b>)</b></code>
<!-- 
ISLOYALMEMBER
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|IsLoyalMember}}<b>(</b>{{Type5|PlayerID}} minor<b>)</b></code>
<!-- 
ISMINORCIVACTIVEQUESTFORPLAYER
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|IsMinorCivActiveQuestForPlayer}}<b>(</b>{{Type5|PlayerID}} major, {{Type5|MinorCivQuestType}} type<b>)</b></code>
<!-- 
ISMINORCIVCONTESTLEADER
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|IsMinorCivContestLeader}}<b>(</b>{{Type5|PlayerID}} major, {{Type5|MinorCivQuestType}} arg1<b>)</b></code>
<!-- 
ISMINORCIVUNITSPAWNINGDISABLED
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|IsMinorCivUnitSpawningDisabled}}<b>(</b>{{Type5|PlayerID}} activePlayer<b>)</b></code>
<!-- 
ISMINORWARQUESTWITHMAJORACTIVE
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|IsMinorWarQuestWithMajorActive}}<b>(</b>{{Type5|PlayerID}} playerLoop = nil<b>)</b></code>
<!-- 
ISNUKEDBY
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|IsNukedBy}}<b>(</b>{{Type5|PlayerID}} activePlayer<b>)</b></code>
<!-- 
ISPLAYERBROKENBORDERPROMISE
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|IsPlayerBrokenBorderPromise}}<b>(</b>{{Type5|PlayerID}} activePlayer<b>)</b></code>
<!-- 
ISPLAYERBROKENCITYSTATEPROMISE
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|IsPlayerBrokenCityStatePromise}}<b>(</b>{{Type5|PlayerID}} activePlayer<b>)</b></code>
<!-- 
ISPLAYERBROKENCOOPWARPROMISE
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|IsPlayerBrokenCoopWarPromise}}<b>(</b>{{Type5|PlayerID}} activePlayer<b>)</b></code>
<!-- 
ISPLAYERBROKENEXPANSIONPROMISE
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|IsPlayerBrokenExpansionPromise}}<b>(</b>{{Type5|PlayerID}} activePlayer<b>)</b></code>
<!-- 
ISPLAYERBROKENMILITARYPROMISE
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|IsPlayerBrokenMilitaryPromise}}<b>(</b>{{Type5|PlayerID}} activePlayer<b>)</b></code>
<!-- 
ISPLAYERDENOUNCEDENEMY
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|IsPlayerDenouncedEnemy}}<b>(</b>{{Type5|PlayerID}} otherPlayer<b>)</b></code>
<!-- 
ISPLAYERDENOUNCEDFRIEND
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|IsPlayerDenouncedFriend}}<b>(</b>{{Type5|PlayerID}} activePlayer<b>)</b></code>
<!-- 
ISPLAYERDOFWITHANYENEMY
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|IsPlayerDoFwithAnyEnemy}}<b>(</b>{{Type5|PlayerID}} activePlayer<b>)</b></code>
<!-- 
ISPLAYERDOFWITHANYFRIEND
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|IsPlayerDoFwithAnyFriend}}<b>(</b>{{Type5|PlayerID}} otherPlayer<b>)</b></code>
<!-- 
ISPLAYERHASOPENBORDERS
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|IsPlayerHasOpenBorders}}<b>(</b>{{Type5|PlayerID}} major<b>)</b></code>
<!-- 
ISPLAYERHASOPENBORDERSAUTOMATICALLY
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|IsPlayerHasOpenBordersAutomatically}}<b>(</b>{{Type5|PlayerID}} major<b>)</b></code>
<!-- 
ISPLAYERIGNOREDBORDERPROMISE
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|IsPlayerIgnoredBorderPromise}}<b>(</b>{{Type5|PlayerID}} activePlayer<b>)</b></code>
<!-- 
ISPLAYERIGNOREDCITYSTATEPROMISE
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|IsPlayerIgnoredCityStatePromise}}<b>(</b>{{Type5|PlayerID}} activePlayer<b>)</b></code>
<!-- 
ISPLAYERIGNOREDEXPANSIONPROMISE
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|IsPlayerIgnoredExpansionPromise}}<b>(</b>{{Type5|PlayerID}} activePlayer<b>)</b></code>
<!-- 
ISPLAYERIGNOREDMILITARYPROMISE
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|IsPlayerIgnoredMilitaryPromise}}<b>(</b>{{Type5|PlayerID}} activePlayer<b>)</b></code>
<!-- 
ISPLAYERNOSETTLEREQUESTEVERASKED
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|IsPlayerNoSettleRequestEverAsked}}<b>(</b>{{Type5|PlayerID}} activePlayer<b>)</b></code>
<!-- 
ISPLAYERRECKLESSEXPANDER
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|IsPlayerRecklessExpander}}<b>(</b>{{Type5|PlayerID}} activePlayer<b>)</b></code>
<!-- 
ISPROTECTEDBYMAJOR
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|IsProtectedByMajor}}<b>(</b>{{Type5|PlayerID}} activePlayer<b>)</b></code>
<!-- 
ISPROTECTINGMINOR
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|IsProtectingMinor}}<b>(</b>{{Type5|PlayerID}} player<b>)</b></code>
<!-- 
ISSTOPSPYINGMESSAGETOOSOON
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|IsStopSpyingMessageTooSoon}}<b>(</b>{{Type5|PlayerID}} activePlayer<b>)</b></code>
<!-- 
ISTHREATENINGBARBARIANSEVENTACTIVEFORPLAYER
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|IsThreateningBarbariansEventActiveForPlayer}}<b>(</b>{{Type5|PlayerID}} major<b>)</b></code>
<!-- 
ISWILLACCEPTPEACEWITHPLAYER
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|IsWillAcceptPeaceWithPlayer}}<b>(</b>{{Type5|PlayerID}} player<b>)</b></code>
<!-- 
ISWORKINGAGAINSTPLAYERACCEPTED
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|IsWorkingAgainstPlayerAccepted}}<b>(</b>{{Type5|PlayerID}} withPlayer, {{Type5|PlayerID}} againstPlayer<b>)</b></code>
<!-- 
ISWORKINGWITHPLAYER
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|IsWorkingWithPlayer}}<b>(</b>{{Type5|PlayerID}} withPlayer<b>)</b></code>
<!-- 
ISWORKINGWITHPLAYERMESSAGETOOSOON
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|IsWorkingWithPlayerMessageTooSoon}}<b>(</b>{{Type5|PlayerID}} withPlayer<b>)</b></code>
<!-- 
SETLOYALMEMBER
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|SetLoyalMember}}<b>(</b>{{Type5|PlayerID}} minor, '''bool''' newValue<b>)</b></code>
<!-- 
WASRESURRECTEDTHISTURNBY
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|WasResurrectedThisTurnBy}}<b>(</b>{{Type5|PlayerID}} player<b>)</b></code>
<!-- 
CALCULATEIMPROVEMENTYIELDCHANGE
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Plot}}:{{Func5|Plot|CalculateImprovementYieldChange}}<b>(</b>{{Type5|ImprovementType}} improvement, {{Type5|YieldType}} yield, {{Type5|PlayerID}} player, '''bool''' optimal, {{Type5|RouteType}} assumeThisRoute<b>)</b></code>
<!-- 
CANBUILD
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|Plot}}:{{Func5|Plot|CanBuild}}<b>(</b>{{Type5|BuildActionType}} build, {{Type5|PlayerID}} player, '''bool''' testVisible<b>)</b></code>
<!-- 
COUNTNUMAIRUNITS
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Plot}}:{{Func5|Plot|CountNumAirUnits}}<b>(</b>{{Type5|PlayerID}} player<b>)</b></code>
<!-- 
GETBESTDEFENDER
-->
|-
|align="right" width="200" |<code>'''unknown'''</code>
|style="padding-left:6px" |<code>{{Type5|Plot}}:{{Func5|Plot|GetBestDefender}}<b>(</b>{{Type5|PlayerID}} owner, {{Type5|PlayerID}} attackingPlayer, {{Type5|Unit}} attacker, '''bool''' testAtWar, '''bool''' testPotentialEnemy, '''bool''' testCanMove<b>)</b></code>
<!-- 
GETFOUNDVALUE
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Plot}}:{{Func5|Plot|GetFoundValue}}<b>(</b>{{Type5|PlayerID}} index<b>)</b></code>
<!-- 
GETNUMDEFENDERS
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Plot}}:{{Func5|Plot|GetNumDefenders}}<b>(</b>{{Type5|PlayerID}} player<b>)</b></code>
<!-- 
GETOWNER
-->
|-
|align="right" width="200" |<code>{{Type5|PlayerID}}</code>
|style="padding-left:6px" |<code>{{Type5|Plot}}:{{Func5|Plot|GetOwner}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETPLAYERCITYRADIUSCOUNT
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Plot}}:{{Func5|Plot|GetPlayerCityRadiusCount}}<b>(</b>{{Type5|PlayerID}} index<b>)</b></code>
<!-- 
GETREVEALEDOWNER
-->
|-
|align="right" width="200" |<code>{{Type5|PlayerID}}</code>
|style="padding-left:6px" |<code>{{Type5|Plot}}:{{Func5|Plot|GetRevealedOwner}}<b>(</b>{{Type5|TeamID}} team, '''bool''' debug<b>)</b></code>
<!-- 
GETUNITPOWER
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Plot}}:{{Func5|Plot|GetUnitPower}}<b>(</b>{{Type5|PlayerID}} owner<b>)</b></code>
<!-- 
GETUPGRADETIMELEFT
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Plot}}:{{Func5|Plot|GetUpgradeTimeLeft}}<b>(</b>{{Type5|ImprovementType}} improvement, {{Type5|PlayerID}} player<b>)</b></code>
<!-- 
GETYIELDWITHBUILD
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Plot}}:{{Func5|Plot|GetYieldWithBuild}}<b>(</b>{{Type5|BuildActionType}} build, {{Type5|YieldType}} yield, '''bool''' arg2, {{Type5|PlayerID}} activePlayer<b>)</b></code>
<!-- 
ISADJACENTPLAYER
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|Plot}}:{{Func5|Plot|IsAdjacentPlayer}}<b>(</b>{{Type5|PlayerID}} player, '''bool''' landOnly<b>)</b></code>
<!-- 
ISBESTADJACENTFOUND
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|Plot}}:{{Func5|Plot|IsBestAdjacentFound}}<b>(</b>{{Type5|PlayerID}} index<b>)</b></code>
<!-- 
ISFRIENDLYTERRITORY
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|Plot}}:{{Func5|Plot|IsFriendlyTerritory}}<b>(</b>{{Type5|PlayerID}} player<b>)</b></code>
<!-- 
ISPLAYERCITYRADIUS
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|Plot}}:{{Func5|Plot|IsPlayerCityRadius}}<b>(</b>{{Type5|PlayerID}} index<b>)</b></code>
<!-- 
ISVISIBLEENEMYUNIT
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Plot}}:{{Func5|Plot|IsVisibleEnemyUnit}}<b>(</b>{{Type5|PlayerID}} player<b>)</b></code>
<!-- 
ISVISIBLEOTHERUNIT
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|Plot}}:{{Func5|Plot|IsVisibleOtherUnit}}<b>(</b>{{Type5|PlayerID}} player<b>)</b></code>
<!-- 
ISWITHINTEAMCITYRADIUS
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|Plot}}:{{Func5|Plot|IsWithinTeamCityRadius}}<b>(</b>{{Type5|TeamID}} team, {{Type5|PlayerID}} ignorePlayer<b>)</b></code>
<!-- 
SETOWNER
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Plot}}:{{Func5|Plot|SetOwner}}<b>(</b>{{Type5|PlayerID}} newValue, '''int''' acquiringCityID, '''bool''' checkUnits = true, '''bool''' updateResources = true<b>)</b></code>
<!-- 
GETCIVILIZATION
-->
|-
|align="right" width="200" |<code>{{Type5|CivilizationType}}</code>
|style="padding-left:6px" |<code>{{Type5|PreGame}}.{{Func5|PreGame|GetCivilization}}<b>(</b>{{Type5|PlayerID}} i = nil<b>)</b></code>
<!-- 
GETCIVILIZATIONCOLOR
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|PreGame}}.{{Func5|PreGame|GetCivilizationColor}}<b>(</b>{{Type5|PlayerID}} player<b>)</b></code>
<!-- 
GETCIVILIZATIONDESCRIPTION
-->
|-
|align="right" width="200" |<code>'''string'''</code>
|style="padding-left:6px" |<code>{{Type5|PreGame}}.{{Func5|PreGame|GetCivilizationDescription}}<b>(</b>{{Type5|PlayerID}} player<b>)</b></code>
<!-- 
GETCIVILIZATIONPACKAGETEXTKEY
-->
|-
|align="right" width="200" |<code>'''unknown'''</code>
|style="padding-left:6px" |<code>{{Type5|PreGame}}.{{Func5|PreGame|GetCivilizationPackageTextKey}}<b>(</b>{{Type5|PlayerID}} player<b>)</b></code>
<!-- 
GETCIVILIZATIONSHORTDESCRIPTION
-->
|-
|align="right" width="200" |<code>'''string'''</code>
|style="padding-left:6px" |<code>{{Type5|PreGame}}.{{Func5|PreGame|GetCivilizationShortDescription}}<b>(</b>{{Type5|PlayerID}} player<b>)</b></code>
<!-- 
GETHANDICAP
-->
|-
|align="right" width="200" |<code>{{Type5|HandicapType}}</code>
|style="padding-left:6px" |<code>{{Type5|PreGame}}.{{Func5|PreGame|GetHandicap}}<b>(</b>{{Type5|PlayerID}} player = nil<b>)</b></code>
<!-- 
GETLEADERNAME
-->
|-
|align="right" width="200" |<code>'''string'''</code>
|style="padding-left:6px" |<code>{{Type5|PreGame}}.{{Func5|PreGame|GetLeaderName}}<b>(</b>{{Type5|PlayerID}} player<b>)</b></code>
<!-- 
GETNICKNAME
-->
|-
|align="right" width="200" |<code>'''string'''</code>
|style="padding-left:6px" |<code>{{Type5|PreGame}}.{{Func5|PreGame|GetNickName}}<b>(</b>{{Type5|PlayerID}} activePlayer<b>)</b></code>
<!-- 
GETSLOTCLAIM
-->
|-
|align="right" width="200" |<code>{{Type5|SlotClaim}}</code>
|style="padding-left:6px" |<code>{{Type5|PreGame}}.{{Func5|PreGame|GetSlotClaim}}<b>(</b>{{Type5|PlayerID}} player<b>)</b></code>
<!-- 
GETSLOTSTATUS
-->
|-
|align="right" width="200" |<code>{{Type5|SlotStatus}}</code>
|style="padding-left:6px" |<code>{{Type5|PreGame}}.{{Func5|PreGame|GetSlotStatus}}<b>(</b>{{Type5|PlayerID}} player<b>)</b></code>
<!-- 
GETTEAM
-->
|-
|align="right" width="200" |<code>{{Type5|TeamID}}</code>
|style="padding-left:6px" |<code>{{Type5|PreGame}}.{{Func5|PreGame|GetTeam}}<b>(</b>{{Type5|PlayerID}} player<b>)</b></code>
<!-- 
HASPASSWORD
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|PreGame}}.{{Func5|PreGame|HasPassword}}<b>(</b>{{Type5|PlayerID}} player<b>)</b></code>
<!-- 
ISCIVILIZATIONKEYAVAILABLE
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|PreGame}}.{{Func5|PreGame|IsCivilizationKeyAvailable}}<b>(</b>{{Type5|PlayerID}} player<b>)</b></code>
<!-- 
ISREADY
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|PreGame}}.{{Func5|PreGame|IsReady}}<b>(</b>{{Type5|PlayerID}} player<b>)</b></code>
<!-- 
SETCIVILIZATION
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|PreGame}}.{{Func5|PreGame|SetCivilization}}<b>(</b>{{Type5|PlayerID}} player, {{Type5|CivilizationType}} civ = nil<b>)</b></code>
<!-- 
SETCIVILIZATIONADJECTIVE
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|PreGame}}.{{Func5|PreGame|SetCivilizationAdjective}}<b>(</b>{{Type5|PlayerID}} EditSlot, '''string''' arg1<b>)</b></code>
<!-- 
SETCIVILIZATIONDESCRIPTION
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|PreGame}}.{{Func5|PreGame|SetCivilizationDescription}}<b>(</b>{{Type5|PlayerID}} EditSlot, '''string''' arg1<b>)</b></code>
<!-- 
SETCIVILIZATIONSHORTDESCRIPTION
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|PreGame}}.{{Func5|PreGame|SetCivilizationShortDescription}}<b>(</b>{{Type5|PlayerID}} EditSlot, '''string''' arg1<b>)</b></code>
<!-- 
SETHANDICAP
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|PreGame}}.{{Func5|PreGame|SetHandicap}}<b>(</b>{{Type5|PlayerID}} player, {{Type5|HandicapType}} id<b>)</b></code>
<!-- 
SETLEADERNAME
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|PreGame}}.{{Func5|PreGame|SetLeaderName}}<b>(</b>{{Type5|PlayerID}} EditSlot, '''string''' arg1<b>)</b></code>
<!-- 
SETNICKNAME
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|PreGame}}.{{Func5|PreGame|SetNickName}}<b>(</b>{{Type5|PlayerID}} EditSlot, '''string''' arg1<b>)</b></code>
<!-- 
SETPASSWORD
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|PreGame}}.{{Func5|PreGame|SetPassword}}<b>(</b>{{Type5|PlayerID}} player, '''string''' arg1, '''string''' arg2 = nil<b>)</b></code>
<!-- 
SETREADY
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|PreGame}}.{{Func5|PreGame|SetReady}}<b>(</b>{{Type5|PlayerID}} arg0, '''bool''' checked = nil<b>)</b></code>
<!-- 
SETSLOTCLAIM
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|PreGame}}.{{Func5|PreGame|SetSlotClaim}}<b>(</b>{{Type5|PlayerID}} player, {{Type5|SlotClaim}} arg1<b>)</b></code>
<!-- 
SETSLOTSTATUS
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|PreGame}}.{{Func5|PreGame|SetSlotStatus}}<b>(</b>{{Type5|PlayerID}} i, {{Type5|SlotStatus}} arg1<b>)</b></code>
<!-- 
SETTEAM
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|PreGame}}.{{Func5|PreGame|SetTeam}}<b>(</b>{{Type5|PlayerID}} player, {{Type5|PlayerID}} playerChoice<b>)</b></code>
<!-- 
TESTPASSWORD
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|PreGame}}.{{Func5|PreGame|TestPassword}}<b>(</b>{{Type5|PlayerID}} player, '''string''' arg1<b>)</b></code>
<!-- 
REGISTERSELECTIONCALLBACK
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|PullDown}}:{{Func5|UIElement|RegisterSelectionCallback}}<b>(</b>('''void''' func<b>(</b>{{Type5|PlayerID}} playerID, {{Type5|HandicapType}} id, '''unknown''' control<b>)</b>) OnChatTarget<b>)</b></code>
<!-- 
SETVALUE
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Slider}}:{{Func5|UIElement|SetValue}}<b>(</b>'''string''' sliderValue, {{Type5|PlayerID}} value = nil<b>)</b></code>
<!-- 
GETPLAYERSTEAMID
-->
|-
|align="right" width="200" |<code>table('''unknown''' => '''unknown''')</code>
|style="padding-left:6px" |<code>{{Type5|Steam}}.{{Func5|Steam|GetPlayerSteamID}}<b>(</b>{{Type5|PlayerID}} player<b>)</b></code>
<!-- 
GETLEADERID
-->
|-
|align="right" width="200" |<code>{{Type5|PlayerID}}</code>
|style="padding-left:6px" |<code>{{Type5|Team}}:{{Func5|Team|GetLeaderID}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETSECRETARYID
-->
|-
|align="right" width="200" |<code>{{Type5|PlayerID}}</code>
|style="padding-left:6px" |<code>{{Type5|Team}}:{{Func5|Team|GetSecretaryID}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
SETHASTECH
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Team}}:{{Func5|Team|SetHasTech}}<b>(</b>{{Type5|TechType}} index, '''bool''' newValue, {{Type5|PlayerID}} player, '''bool''' first, '''bool''' announce<b>)</b></code>
<!-- 
CHANGERESEARCHPROGRESS
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|TeamTechs}}:{{Func5|TeamTechs|ChangeResearchProgress}}<b>(</b>{{Type5|TechType}} index, '''int''' change, {{Type5|PlayerID}} player<b>)</b></code>
<!-- 
CHANGERESEARCHPROGRESSPERCENT
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|TeamTechs}}:{{Func5|TeamTechs|ChangeResearchProgressPercent}}<b>(</b>{{Type5|TechType}} index, '''int''' percent, {{Type5|PlayerID}} player<b>)</b></code>
<!-- 
CHANGERESEARCHPROGRESSTIMES100
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|TeamTechs}}:{{Func5|TeamTechs|ChangeResearchProgressTimes100}}<b>(</b>{{Type5|TechType}} index, '''int''' change, {{Type5|PlayerID}} player<b>)</b></code>
<!-- 
SETRESEARCHPROGRESS
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|TeamTechs}}:{{Func5|TeamTechs|SetResearchProgress}}<b>(</b>{{Type5|TechType}} index, '''int''' newValue, {{Type5|PlayerID}} player<b>)</b></code>
<!-- 
SETWRAPWIDTH
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>TextBase:{{Func5|UIElement|SetWrapWidth}}<b>(</b>{{Type5|PlayerID}} arg0<b>)</b></code>
<!-- 
SETVOID1
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|TextButton}}:{{Func5|UIElement|SetVoid1}}<b>(</b>{{Type5|PlayerID}} playerLoop<b>)</b></code>
<!-- 
ACTIVATENOTIFICATION
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|UI}}.{{Func5|UI|ActivateNotification}}<b>(</b>{{Type5|PlayerID}} blockingNotificationIndex<b>)</b></code>
<!-- 
DOFINALIZEPLAYERDEAL
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|UI}}.{{Func5|UI|DoFinalizePlayerDeal}}<b>(</b>{{Type5|PlayerID}} them, {{Type5|PlayerID}} us, '''bool''' arg2<b>)</b></code>
<!-- 
GETNUMCURRENTDEALS
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|UI}}.{{Func5|UI|GetNumCurrentDeals}}<b>(</b>{{Type5|PlayerID}} player<b>)</b></code>
<!-- 
GETNUMHISTORICDEALS
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|UI}}.{{Func5|UI|GetNumHistoricDeals}}<b>(</b>{{Type5|PlayerID}} player<b>)</b></code>
<!-- 
HASMADEPROPOSAL
-->
|-
|align="right" width="200" |<code>{{Type5|PlayerID}}</code>
|style="padding-left:6px" |<code>{{Type5|UI}}.{{Func5|UI|HasMadeProposal}}<b>(</b>{{Type5|PlayerID}} us<b>)</b></code>
<!-- 
LOADCURRENTDEAL
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|UI}}.{{Func5|UI|LoadCurrentDeal}}<b>(</b>{{Type5|PlayerID}} player, {{Type5|SpecialistType}} i<b>)</b></code>
<!-- 
LOADHISTORICDEAL
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|UI}}.{{Func5|UI|LoadHistoricDeal}}<b>(</b>{{Type5|PlayerID}} player, {{Type5|SpecialistType}} i<b>)</b></code>
<!-- 
LOADPROPOSEDDEAL
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|UI}}.{{Func5|UI|LoadProposedDeal}}<b>(</b>{{Type5|PlayerID}} us, {{Type5|PlayerID}} them<b>)</b></code>
<!-- 
ONHUMANDEMAND
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|UI}}.{{Func5|UI|OnHumanDemand}}<b>(</b>{{Type5|PlayerID}} aIPlayer<b>)</b></code>
<!-- 
ONHUMANOPENEDTRADESCREEN
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|UI}}.{{Func5|UI|OnHumanOpenedTradeScreen}}<b>(</b>{{Type5|PlayerID}} aIPlayer<b>)</b></code>
<!-- 
PROPOSEDDEALEXISTS
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|UI}}.{{Func5|UI|ProposedDealExists}}<b>(</b>{{Type5|PlayerID}} them, {{Type5|PlayerID}} us<b>)</b></code>
<!-- 
SETINTERFACEMODEVALUE
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|UI}}.{{Func5|UI|SetInterfaceModeValue}}<b>(</b>{{Type5|PlayerID}} minorCiv<b>)</b></code>
<!-- 
SETREPEATACTIONPLAYER
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|UI}}.{{Func5|UI|SetRepeatActionPlayer}}<b>(</b>{{Type5|PlayerID}} player<b>)</b></code>
<!-- 
CHANGEDAMAGE
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Unit}}:{{Func5|Unit|ChangeDamage}}<b>(</b>'''int''' change, {{Type5|PlayerID}} player<b>)</b></code>
<!-- 
GETFIRESUPPORTUNIT
-->
|-
|align="right" width="200" |<code>{{Type5|Unit}}</code>
|style="padding-left:6px" |<code>{{Type5|Unit}}:{{Func5|Unit|GetFireSupportUnit}}<b>(</b>{{Type5|PlayerID}} defender, '''int''' x, '''int''' y<b>)</b></code>
<!-- 
GETOWNER
-->
|-
|align="right" width="200" |<code>{{Type5|PlayerID}}</code>
|style="padding-left:6px" |<code>{{Type5|Unit}}:{{Func5|Unit|GetOwner}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
KILL
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Unit}}:{{Func5|Unit|Kill}}<b>(</b>'''bool''' delay, {{Type5|PlayerID}} player = NO_PLAYER<b>)</b></code>
<!-- 
SETDAMAGE
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Unit}}:{{Func5|Unit|SetDamage}}<b>(</b>'''int''' newValue, {{Type5|PlayerID}} player, '''bool''' notifyEntity = true<b>)</b></code>
<!-- 
SETORIGINALOWNER
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Unit}}:{{Func5|Unit|SetOriginalOwner}}<b>(</b>{{Type5|PlayerID}} oldOwner<b>)</b></code>
|}




{{Civ5 API Footer}}
[[Category:Civ5 Types|PlayerID]]