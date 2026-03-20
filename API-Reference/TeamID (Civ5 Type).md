{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|ID.png|The <code>TeamID</code> pseudo-type is actually a regular '''integer'''. Pseudo-types do not exist in Lua, they only serve a documentation purpose on the wiki!}}


= Usage =
* You can get a team's ID through {{Type5|Team}}.{{Func5|Team|GetID}}(). 
* There is a global '''Teams''' table that stores all teams. Keys are the teams' ID and values are {{Type5|Team}} instances.
* A team's ID is usually the founding player's ID but you should not rely on it.


How to retrieve a {{Type5|Team}} object from an ID:
<syntaxhighlight lang="lua" class="civ5-example">
local pTeam = Teams[teamID]
</syntaxhighlight>


== Enumerating teams ==
As opposed to {{Type5|PlayerID}} there is no special precaution to take for using teams.
<syntaxhighlight lang="lua" class="civ5-example">
for id, team in pairs(Teams) do
	print(id, team:GetName())
end
</syntaxhighlight>


=== Built-in constants ===
You can also use the built-in constants: <code>GameDefines.MAX_TEAMS</code> (64), <code>GameDefines.MAX_CIV_TEAMS</code> (63). See also {{Type5|GameDefines}}<br/>
The following example enumerates non-barbarian teams only:
<syntaxhighlight lang="lua" class="civ5-example">
for i = 0, GameDefines.MAX_CIV_TEAMS - 1 do
	print(i, Teams[i]:GetName())
end
</syntaxhighlight>


== Code snippets ==
Here is a function to check whether a player has a given tech. Indeed, since techs are shared by all team's member, the {{Type5|Player}} has no method to check the techs a player knows.
<syntaxhighlight lang="lua" class="civ5-example">
function HasPlayerTech(pPlayer, techType)
	local teamID = pPlayer:GetTeam();
	local pTeam = Teams[teamID];
	return pTeam:HasTech(techType);
end
</syntaxhighlight>


=Used by=
{|cellspacing="4" cellpadding="0" width="100%" style="background-color:#F0F0F0"
<!-- 
GETNUMREVEALEDTILES
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Area}}:{{Func5|Area|GetNumRevealedTiles}}<b>(</b>{{Type5|TeamID}} index<b>)</b></code>
<!-- 
GETNUMUNREVEALEDTILES
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Area}}:{{Func5|Area|GetNumUnrevealedTiles}}<b>(</b>{{Type5|TeamID}} index<b>)</b></code>
<!-- 
GETTEAM
-->
|-
|align="right" width="200" |<code>{{Type5|TeamID}}</code>
|style="padding-left:6px" |<code>{{Type5|City}}:{{Func5|City|GetTeam}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ISREVEALED
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|City}}:{{Func5|City|IsRevealed}}<b>(</b>{{Type5|TeamID}} index, '''bool''' debug<b>)</b></code>
<!-- 
ISVISIBLE
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|City}}:{{Func5|City|IsVisible}}<b>(</b>{{Type5|TeamID}} team, '''bool''' debug<b>)</b></code>
<!-- 
SETREVEALED
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|City}}:{{Func5|City|SetRevealed}}<b>(</b>{{Type5|TeamID}} index, '''bool''' newValue<b>)</b></code>
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
ISPOSSIBLETOTRADEITEM
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Deal}}:{{Func5|Deal|IsPossibleToTradeItem}}<b>(</b>{{Type5|PlayerID}} us, {{Type5|PlayerID}} them, {{Type5|TradeableItemType}} tradeType, {{Type5|TeamID}} dealDuration, {{Type5|ResourceType}} dealDuration = nil<b>)</b></code>
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
ENDGAMESHOW
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Events}}.{{Func5|Events|EndGameShow}}<b>(</b>{{Type5|EndGameType}} type, {{Type5|TeamID}} team<b>)</b></code>
<!-- 
WARSTATECHANGED
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Events}}.{{Func5|Events|WarStateChanged}}<b>(</b>{{Type5|TeamID}} team1, {{Type5|TeamID}} team2, '''bool''' war<b>)</b></code>
<!-- 
CHANGENUMVOTESFORTEAM
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Game}}.{{Func5|Game|ChangeNumVotesForTeam}}<b>(</b>{{Type5|TeamID}} team, '''int''' kiVaticanExtraVotes<b>)</b></code>
<!-- 
DOMINORGOLDGIFT
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Game}}.{{Func5|Game|DoMinorGoldGift}}<b>(</b>{{Type5|TeamID}} gold, '''int''' goldGiftSmall<b>)</b></code>
<!-- 
GETACTIVETEAM
-->
|-
|align="right" width="200" |<code>{{Type5|TeamID}}</code>
|style="padding-left:6px" |<code>{{Type5|Game}}.{{Func5|Game|GetActiveTeam}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETNUMVOTESFORTEAM
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Game}}.{{Func5|Game|GetNumVotesForTeam}}<b>(</b>{{Type5|TeamID}} teamLoop<b>)</b></code>
<!-- 
GETPREVIOUSVOTECAST
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Game}}.{{Func5|Game|GetPreviousVoteCast}}<b>(</b>{{Type5|TeamID}} teamLoop<b>)</b></code>
<!-- 
GETRANKTEAM
-->
|-
|align="right" width="200" |<code>{{Type5|TeamID}}</code>
|style="padding-left:6px" |<code>{{Type5|Game}}.{{Func5|Game|GetRankTeam}}<b>(</b>'''int''' rank<b>)</b></code>
<!-- 
GETTEAMRANK
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Game}}.{{Func5|Game|GetTeamRank}}<b>(</b>{{Type5|TeamID}} index<b>)</b></code>
<!-- 
GETTEAMSCORE
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Game}}.{{Func5|Game|GetTeamScore}}<b>(</b>{{Type5|TeamID}} index<b>)</b></code>
<!-- 
GETVOTECAST
-->
|-
|align="right" width="200" |<code>{{Type5|TeamID}}</code>
|style="padding-left:6px" |<code>{{Type5|Game}}.{{Func5|Game|GetVoteCast}}<b>(</b>{{Type5|TeamID}} team<b>)</b></code>
<!-- 
GETWINNER
-->
|-
|align="right" width="200" |<code>{{Type5|TeamID}}</code>
|style="padding-left:6px" |<code>{{Type5|Game}}.{{Func5|Game|GetWinner}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ISTEAMVOTEELIGIBLE
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|Game}}.{{Func5|Game|IsTeamVoteEligible}}<b>(</b>{{Type5|TeamID}} team, {{Type5|VoteSourceType}} voteSource<b>)</b></code>
<!-- 
SETWINNER
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Game}}.{{Func5|Game|SetWinner}}<b>(</b>{{Type5|TeamID}} newWinner, {{Type5|VictoryType}} newVictory<b>)</b></code>
<!-- 
CANDECLAREWAR
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|GameEvents}}.{{Func5|GameEvents|CanDeclareWar}}<b>(</b>{{Type5|TeamID}} myTeam, {{Type5|TeamID}} theirTeam<b>)</b></code>
<!-- 
TEAMSETHASTECH
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|GameEvents}}.{{Func5|GameEvents|TeamSetHasTech}}<b>(</b>{{Type5|TeamID}} team, {{Type5|TechType}} tech, '''bool''' adopted<b>)</b></code>
<!-- 
TEAMTECHRESEARCHED
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|GameEvents}}.{{Func5|GameEvents|TeamTechResearched}}<b>(</b>{{Type5|TeamID}} team, {{Type5|TechType}} tech, '''int''' change<b>)</b></code>
<!-- 
SENDCHANGEWAR
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Network}}.{{Func5|Network|SendChangeWar}}<b>(</b>{{Type5|TeamID}} minorCivTeam, '''bool''' arg1<b>)</b></code>
<!-- 
SENDLIBERATEMINOR
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Network}}.{{Func5|Network|SendLiberateMinor}}<b>(</b>{{Type5|TeamID}} minor, {{Type5|TeamID}} city<b>)</b></code>
<!-- 
SENDMINORCIVENTERTERRITORY
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Network}}.{{Func5|Network|SendMinorCivEnterTerritory}}<b>(</b>{{Type5|TeamID}} rivalTeam<b>)</b></code>
<!-- 
CANSTOPTRADINGWITHTEAM
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|CanStopTradingWithTeam}}<b>(</b>{{Type5|TeamID}} team<b>)</b></code>
<!-- 
ISMINORPERMANENTWAR
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|IsMinorPermanentWar}}<b>(</b>{{Type5|TeamID}} activeTeam<b>)</b></code>
<!-- 
ISPEACEBLOCKED
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|IsPeaceBlocked}}<b>(</b>{{Type5|TeamID}} activeTeam<b>)</b></code>
<!-- 
STOPTRADINGWITHTEAM
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|StopTradingWithTeam}}<b>(</b>{{Type5|TeamID}} team<b>)</b></code>
<!-- 
CALCULATEBESTNATUREYIELD
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Plot}}:{{Func5|Plot|CalculateBestNatureYield}}<b>(</b>{{Type5|YieldType}} index, {{Type5|TeamID}} team<b>)</b></code>
<!-- 
CALCULATENATUREYIELD
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Plot}}:{{Func5|Plot|CalculateNatureYield}}<b>(</b>{{Type5|YieldType}} index, {{Type5|TeamID}} team, '''bool''' ignoreFeature = false<b>)</b></code>
<!-- 
CALCULATETOTALBESTNATUREYIELD
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Plot}}:{{Func5|Plot|CalculateTotalBestNatureYield}}<b>(</b>{{Type5|TeamID}} team<b>)</b></code>
<!-- 
CANHAVEIMPROVEMENT
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|Plot}}:{{Func5|Plot|CanHaveImprovement}}<b>(</b>{{Type5|ImprovementType}} improvement, {{Type5|TeamID}} team, '''bool''' potential<b>)</b></code>
<!-- 
CANSEEPLOT
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|Plot}}:{{Func5|Plot|CanSeePlot}}<b>(</b>{{Type5|Plot}} target, {{Type5|TeamID}} team, '''int''' range<b>)</b></code>
<!-- 
CHANGEBUILDPROGRESS
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|Plot}}:{{Func5|Plot|ChangeBuildProgress}}<b>(</b>{{Type5|BuildActionType}} build, '''int''' change, {{Type5|TeamID}} team<b>)</b></code>
<!-- 
CHANGEINVISIBLEVISIBILITYCOUNT
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Plot}}:{{Func5|Plot|ChangeInvisibleVisibilityCount}}<b>(</b>{{Type5|TeamID}} team, {{Type5|InvisibilityScopeType}} invisible, '''int''' change<b>)</b></code>
<!-- 
CHANGEVISIBILITYCOUNT
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Plot}}:{{Func5|Plot|ChangeVisibilityCount}}<b>(</b>{{Type5|TeamID}} team, '''int''' change, {{Type5|InvisibilityScopeType}} seeInvisibleType, '''bool''' informExplorationTracking, '''bool''' alwaysSeeInvisible<b>)</b></code>
<!-- 
DEFENSEMODIFIER
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Plot}}:{{Func5|Plot|DefenseModifier}}<b>(</b>{{Type5|TeamID}} defendTeam, '''bool''' ignoreBuilding, '''bool''' help<b>)</b></code>
<!-- 
GETFEATUREPRODUCTION
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Plot}}:{{Func5|Plot|GetFeatureProduction}}<b>(</b>{{Type5|BuildActionType}} build, {{Type5|TeamID}} team, {{Type5|City}} city<b>)</b></code>
<!-- 
GETINVISIBLEVISIBILITYCOUNT
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Plot}}:{{Func5|Plot|GetInvisibleVisibilityCount}}<b>(</b>{{Type5|TeamID}} team, {{Type5|InvisibilityScopeType}} invisible<b>)</b></code>
<!-- 
GETNONOBSOLETERESOURCETYPE
-->
|-
|align="right" width="200" |<code>{{Type5|ResourceType}}</code>
|style="padding-left:6px" |<code>{{Type5|Plot}}:{{Func5|Plot|GetNonObsoleteResourceType}}<b>(</b>{{Type5|TeamID}} team<b>)</b></code>
<!-- 
GETRESOURCETYPE
-->
|-
|align="right" width="200" |<code>{{Type5|ResourceType}}</code>
|style="padding-left:6px" |<code>{{Type5|Plot}}:{{Func5|Plot|GetResourceType}}<b>(</b>{{Type5|TeamID}} team<b>)</b></code>
<!-- 
GETREVEALEDIMPROVEMENTTYPE
-->
|-
|align="right" width="200" |<code>{{Type5|ImprovementType}}</code>
|style="padding-left:6px" |<code>{{Type5|Plot}}:{{Func5|Plot|GetRevealedImprovementType}}<b>(</b>{{Type5|TeamID}} team, '''bool''' debug<b>)</b></code>
<!-- 
GETREVEALEDOWNER
-->
|-
|align="right" width="200" |<code>{{Type5|PlayerID}}</code>
|style="padding-left:6px" |<code>{{Type5|Plot}}:{{Func5|Plot|GetRevealedOwner}}<b>(</b>{{Type5|TeamID}} team, '''bool''' debug<b>)</b></code>
<!-- 
GETREVEALEDROUTETYPE
-->
|-
|align="right" width="200" |<code>{{Type5|RouteType}}</code>
|style="padding-left:6px" |<code>{{Type5|Plot}}:{{Func5|Plot|GetRevealedRouteType}}<b>(</b>{{Type5|TeamID}} team, '''bool''' debug<b>)</b></code>
<!-- 
GETREVEALEDTEAM
-->
|-
|align="right" width="200" |<code>{{Type5|TeamID}}</code>
|style="padding-left:6px" |<code>{{Type5|Plot}}:{{Func5|Plot|GetRevealedTeam}}<b>(</b>{{Type5|TeamID}} team, '''bool''' debug<b>)</b></code>
<!-- 
GETTEAM
-->
|-
|align="right" width="200" |<code>{{Type5|TeamID}}</code>
|style="padding-left:6px" |<code>{{Type5|Plot}}:{{Func5|Plot|GetTeam}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETVISIBILITYCOUNT
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Plot}}:{{Func5|Plot|GetVisibilityCount}}<b>(</b>{{Type5|TeamID}} team<b>)</b></code>
<!-- 
ISADJACENTNONREVEALED
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|Plot}}:{{Func5|Plot|IsAdjacentNonrevealed}}<b>(</b>{{Type5|TeamID}} team<b>)</b></code>
<!-- 
ISADJACENTNONVISIBLE
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|Plot}}:{{Func5|Plot|IsAdjacentNonvisible}}<b>(</b>{{Type5|TeamID}} team<b>)</b></code>
<!-- 
ISADJACENTREVEALED
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|Plot}}:{{Func5|Plot|IsAdjacentRevealed}}<b>(</b>{{Type5|TeamID}} team<b>)</b></code>
<!-- 
ISADJACENTTEAM
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|Plot}}:{{Func5|Plot|IsAdjacentTeam}}<b>(</b>{{Type5|TeamID}} team, '''bool''' landOnly<b>)</b></code>
<!-- 
ISADJACENTVISIBLE
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|Plot}}:{{Func5|Plot|IsAdjacentVisible}}<b>(</b>{{Type5|TeamID}} team, '''bool''' debug<b>)</b></code>
<!-- 
ISINVISIBLEVISIBLE
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|Plot}}:{{Func5|Plot|IsInvisibleVisible}}<b>(</b>{{Type5|TeamID}} team, {{Type5|InvisibilityScopeType}} invisible<b>)</b></code>
<!-- 
ISREVEALED
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Plot}}:{{Func5|Plot|IsRevealed}}<b>(</b>{{Type5|TeamID}} team, '''bool''' debug<b>)</b></code>
<!-- 
ISREVEALEDGOODY
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|Plot}}:{{Func5|Plot|IsRevealedGoody}}<b>(</b>{{Type5|TeamID}} team<b>)</b></code>
<!-- 
ISVISIBLE
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Plot}}:{{Func5|Plot|IsVisible}}<b>(</b>{{Type5|TeamID}} team, '''bool''' debug<b>)</b></code>
<!-- 
ISWITHINTEAMCITYRADIUS
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|Plot}}:{{Func5|Plot|IsWithinTeamCityRadius}}<b>(</b>{{Type5|TeamID}} team, {{Type5|PlayerID}} ignorePlayer<b>)</b></code>
<!-- 
SEEFROMLEVEL
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Plot}}:{{Func5|Plot|SeeFromLevel}}<b>(</b>{{Type5|TeamID}} team<b>)</b></code>
<!-- 
SETREVEALED
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Plot}}:{{Func5|Plot|SetRevealed}}<b>(</b>{{Type5|TeamID}} team, '''bool''' newValue, '''bool''' terrainOnly, {{Type5|TeamID}} fromTeam<b>)</b></code>
<!-- 
GETTEAM
-->
|-
|align="right" width="200" |<code>{{Type5|TeamID}}</code>
|style="padding-left:6px" |<code>{{Type5|PreGame}}.{{Func5|PreGame|GetTeam}}<b>(</b>{{Type5|PlayerID}} player<b>)</b></code>
<!-- 
ADDTEAM
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Team}}:{{Func5|Team|AddTeam}}<b>(</b>{{Type5|TeamID}} team<b>)</b></code>
<!-- 
CANCHANGEWARPEACE
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|Team}}:{{Func5|Team|CanChangeWarPeace}}<b>(</b>{{Type5|TeamID}} team<b>)</b></code>
<!-- 
CANCONTACT
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|Team}}:{{Func5|Team|CanContact}}<b>(</b>{{Type5|TeamID}} team<b>)</b></code>
<!-- 
CANDECLAREWAR
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Team}}:{{Func5|Team|CanDeclareWar}}<b>(</b>{{Type5|TeamID}} team<b>)</b></code>
<!-- 
DECLAREWAR
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Team}}:{{Func5|Team|DeclareWar}}<b>(</b>{{Type5|TeamID}} team<b>)</b></code>
<!-- 
GETID
-->
|-
|align="right" width="200" |<code>{{Type5|TeamID}}</code>
|style="padding-left:6px" |<code>{{Type5|Team}}:{{Func5|Team|GetID}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETLIBERATEDBYTEAM
-->
|-
|align="right" width="200" |<code>{{Type5|TeamID}}</code>
|style="padding-left:6px" |<code>{{Type5|Team}}:{{Func5|Team|GetLiberatedByTeam}}<b>(</b>{{Type5|TeamID}} index<b>)</b></code>
<!-- 
GETNUMTURNSLOCKEDINTOWAR
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Team}}:{{Func5|Team|GetNumTurnsLockedIntoWar}}<b>(</b>{{Type5|TeamID}} team<b>)</b></code>
<!-- 
GETTEAMVOTINGFORINDIPLO
-->
|-
|align="right" width="200" |<code>{{Type5|TeamID}}</code>
|style="padding-left:6px" |<code>{{Type5|Team}}:{{Func5|Team|GetTeamVotingForInDiplo}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
HASEMBASSYATTEAM
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|Team}}:{{Func5|Team|HasEmbassyAtTeam}}<b>(</b>{{Type5|TeamID}} themTeam<b>)</b></code>
<!-- 
ISALLOWSOPENBORDERSTOTEAM
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|Team}}:{{Func5|Team|IsAllowsOpenBordersToTeam}}<b>(</b>{{Type5|TeamID}} index<b>)</b></code>
<!-- 
ISATWAR
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Team}}:{{Func5|Team|IsAtWar}}<b>(</b>{{Type5|TeamID}} index<b>)</b></code>
<!-- 
ISDEFENSIVEPACT
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|Team}}:{{Func5|Team|IsDefensivePact}}<b>(</b>{{Type5|TeamID}} index<b>)</b></code>
<!-- 
ISFORCEPEACE
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|Team}}:{{Func5|Team|IsForcePeace}}<b>(</b>{{Type5|TeamID}} index<b>)</b></code>
<!-- 
ISHASMET
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Team}}:{{Func5|Team|IsHasMet}}<b>(</b>{{Type5|TeamID}} index<b>)</b></code>
<!-- 
ISHASRESEARCHAGREEMENT
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|Team}}:{{Func5|Team|IsHasResearchAgreement}}<b>(</b>{{Type5|TeamID}} team<b>)</b></code>
<!-- 
ISHASTRADEAGREEMENT
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|Team}}:{{Func5|Team|IsHasTradeAgreement}}<b>(</b>{{Type5|TeamID}} team<b>)</b></code>
<!-- 
ISOPENBORDERSTRADINGALLOWEDWITHTEAM
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Team}}:{{Func5|Team|IsOpenBordersTradingAllowedWithTeam}}<b>(</b>{{Type5|TeamID}} arg0<b>)</b></code>
<!-- 
ISPERMANENTWARPEACE
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|Team}}:{{Func5|Team|IsPermanentWarPeace}}<b>(</b>{{Type5|TeamID}} index<b>)</b></code>
<!-- 
MAKEPEACE
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Team}}:{{Func5|Team|MakePeace}}<b>(</b>{{Type5|TeamID}} team<b>)</b></code>
<!-- 
MEET
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Team}}:{{Func5|Team|Meet}}<b>(</b>{{Type5|TeamID}} team, '''bool''' newDiplo<b>)</b></code>
<!-- 
SETPERMANENTWARPEACE
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Team}}:{{Func5|Team|SetPermanentWarPeace}}<b>(</b>{{Type5|TeamID}} index, '''bool''' newValue<b>)</b></code>
<!-- 
CANCOEXISTWITHENEMYUNIT
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|Unit}}:{{Func5|Unit|CanCoexistWithEnemyUnit}}<b>(</b>{{Type5|TeamID}} team<b>)</b></code>
<!-- 
CANENTERTERRITORY
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|Unit}}:{{Func5|Unit|CanEnterTerritory}}<b>(</b>{{Type5|TeamID}} team, '''bool''' ignoreRightOfPassage = false, '''bool''' isCity = false<b>)</b></code>
<!-- 
CANSIEGE
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|Unit}}:{{Func5|Unit|CanSiege}}<b>(</b>{{Type5|TeamID}} team<b>)</b></code>
<!-- 
GETCOMBATOWNER
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Unit}}:{{Func5|Unit|GetCombatOwner}}<b>(</b>{{Type5|TeamID}} forTeam<b>)</b></code>
<!-- 
GETDECLAREWARRANGESTRIKE
-->
|-
|align="right" width="200" |<code>{{Type5|TeamID}}</code>
|style="padding-left:6px" |<code>{{Type5|Unit}}:{{Func5|Unit|GetDeclareWarRangeStrike}}<b>(</b>{{Type5|Plot}} plot<b>)</b></code>
<!-- 
GETTEAM
-->
|-
|align="right" width="200" |<code>{{Type5|TeamID}}</code>
|style="padding-left:6px" |<code>{{Type5|Unit}}:{{Func5|Unit|GetTeam}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ISINVISIBLE
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|Unit}}:{{Func5|Unit|IsInvisible}}<b>(</b>{{Type5|TeamID}} team, '''bool''' debug, '''bool''' checkCargo = false<b>)</b></code>
<!-- 
ISNUKEVICTIM
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|Unit}}:{{Func5|Unit|IsNukeVictim}}<b>(</b>{{Type5|Plot}} plot, {{Type5|TeamID}} team<b>)</b></code>
|}




{{Civ5 API Footer}}
[[Category:Civ5 Types|TeamID]]