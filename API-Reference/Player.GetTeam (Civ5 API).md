{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Player}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>{{Type5|PlayerID}} Player:GetTeam<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
''Too many occurences. Only 50 out of 391 are listed.''

{{PseudoH4|CityBannerManager.lua}}
:<code>UI/InGame/CityBannerManager.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0459}}<syntaxhighlight lang="lua">if (Teams[Game.GetActiveTeam()]:IsHasMet(player:GetTeam())) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0581}}<syntaxhighlight lang="lua">local team = Players[playerID]:GetTeam();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0657}}<syntaxhighlight lang="lua">local cityTeam = Players[instance.playerID]:GetTeam();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0814}}<syntaxhighlight lang="lua">local active_team = Players[Game.GetActivePlayer()]:GetTeam();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1113}}<syntaxhighlight lang="lua">elseif (Teams[Game.GetActiveTeam()]:IsHasMet(player:GetTeam())) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CityBannerManager.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/CityBannerManager.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0193}}<syntaxhighlight lang="lua">elseif (not Teams[Game.GetActiveTeam()]:IsHasMet(player:GetTeam())) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CityStateDiploPopup.lua}}
:<code>UI/InGame/Popups/CityStateDiploPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0265}}<syntaxhighlight lang="lua">if (Teams[Players[iAlly]:GetTeam()]:IsHasMet(Game.GetActiveTeam())) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CityStateStatusHelper.lua (G&K)}}
:<code>DLC/Expansion/UI/CityStateStatusHelper.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0054}}<syntaxhighlight lang="lua">local iMajorTeam = pMajor:GetTeam();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CivilopediaScreen.lua}}
:<code>UI/Civilopedia/CivilopediaScreen.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1996}}<syntaxhighlight lang="lua">local pTeam = Teams[pPlayer:GetTeam()];</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CivsAlive.lua - DLC_01 DLC}}
:<code>DLC/DLC_01/Scenarios/Mongol Scenario/CivsAlive.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0137}}<syntaxhighlight lang="lua">local eDestroyedTeam = Players[playerID]:GetTeam();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|Demographics.lua}}
:<code>UI/InGame/Popups/Demographics.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0328}}<syntaxhighlight lang="lua">local iTeam = pPlayer:GetTeam();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DiploCorner.lua}}
:<code>UI/InGame/WorldView/DiploCorner.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0273}}<syntaxhighlight lang="lua">local iOtherTeam = Players[iOtherPlayer]:GetTeam();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0440}}<syntaxhighlight lang="lua">g_iLocalTeam = g_pLocalPlayer:GetTeam();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DiploGlobalRelationships.lua}}
:<code>UI/InGame/Popups/DiploGlobalRelationships.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0182}}<syntaxhighlight lang="lua">local iThirdTeam = pThirdPlayer:GetTeam();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DiploList.lua}}
:<code>UI/InGame/DiploList.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0019}}<syntaxhighlight lang="lua">local g_iTeam = g_pPlayer:GetTeam();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DiploRelationships.lua}}
:<code>UI/InGame/Popups/DiploRelationships.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0054}}<syntaxhighlight lang="lua">if (pPlayer:GetTeam() ~= iOtherTeam and pOtherPlayer:IsAlive()) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0376}}<syntaxhighlight lang="lua">local bWar = Teams[Game.GetActiveTeam()]:IsAtWar(pPlayer:GetTeam());</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DiscussionDialog.lua}}
:<code>UI/InGame/LeaderHead/DiscussionDialog.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0187}}<syntaxhighlight lang="lua">if (pAIPlayer:GetTeam() ~= Players[iActivePlayer]:GetTeam()) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|InGame.lua}}
:<code>UI/InGame/InGame.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0236}}<syntaxhighlight lang="lua">if (plot:IsVisible(player:GetTeam(), false) and (plot:IsVisibleEnemyDefender(pUnit) or plot:IsEnemyCity(pUnit))) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|MPList.lua}}
:<code>UI/InGame/WorldView/MPList.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0007}}<syntaxhighlight lang="lua">local g_pLocalTeam = Teams[ Players[ Game.GetActivePlayer() ]:GetTeam() ];</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0382}}<syntaxhighlight lang="lua">g_pLocalTeam = Teams[ Players[ Game.GetActivePlayer() ]:GetTeam() ];</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|North_vs_South.lua}}
:<code>Maps/North_vs_South.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0602}}<syntaxhighlight lang="lua">local team_ID = player:GetTeam()</syntaxhighlight>
{{CodeLine5|0603}}<syntaxhighlight lang="lua">if team_ID == teamNorthID then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|PlotMouseoverInclude.lua}}
:<code>UI/InGame/PlotMouseoverInclude.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0359}}<syntaxhighlight lang="lua">local plotTeam = pPlayer:GetTeam();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|Ranking.lua}}
:<code>UI/InGame/Popups/Ranking.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0019}}<syntaxhighlight lang="lua">if (pPlayer:GetTeam() == Game:GetWinner()) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ReligionOverview.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/Popups/ReligionOverview.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0485}}<syntaxhighlight lang="lua">local activeTeam = Teams[activePlayer:GetTeam()];</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ResourceIconManager.lua}}
:<code>UI/InGame/ResourceIconManager.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0084}}<syntaxhighlight lang="lua">if( plot:IsRevealed( pPlayer:GetTeam(), false ) ) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0088}}<syntaxhighlight lang="lua">if( not bIsBuilt and pPlayer:GetTeam() == Game.GetActiveTeam() ) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TechPopup.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/TechPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0139}}<syntaxhighlight lang="lua">local opponentTeam = Teams[opponentPlayer:GetTeam()];</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TradeLogic.lua}}
:<code>UI/InGame/WorldView/TradeLogic.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0103}}<syntaxhighlight lang="lua">g_iThemTeam = g_pThem:GetTeam();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0464}}<syntaxhighlight lang="lua">iLoopTeam = pLoopPlayer:GetTeam();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|2557}}<syntaxhighlight lang="lua">local iFromTeam = Players[iFromPlayer]:GetTeam();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TradeLogic.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/WorldView/TradeLogic.lua</code>
:{{CodeBegin5}}
{{CodeLine5|2003}}<syntaxhighlight lang="lua">local iTeam = player:GetTeam();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TurnsRemaining.lua - DLC_02 DLC}}
:<code>DLC/DLC_02/Scenarios/NewWorldScenario/TurnsRemaining.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0020}}<syntaxhighlight lang="lua">Game.SetWinner(player:GetTeam(), GameInfo.Victories["VICTORY_DOMINATION"].ID);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0261}}<syntaxhighlight lang="lua">if (pLoopPlayer:GetTeam() == myTeam) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TurnsRemaining.lua (G&K)}}
:<code>DLC/Expansion/Scenarios/MedievalScenario/TurnsRemaining.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0108}}<syntaxhighlight lang="lua">Game.SetWinner(Players[Game.GetActivePlayer()]:GetTeam(), GameInfo.Victories["VICTORY_TIME"].ID);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0434}}<syntaxhighlight lang="lua">iRecipient = pAlly:GetTeam();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0973}}<syntaxhighlight lang="lua">local vaticanTeamID = Players[iVaticanPlayer]:GetTeam();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0975}}<syntaxhighlight lang="lua">local jerusalemTeamID = Players[iJerusalemPlayer]:GetTeam();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1236}}<syntaxhighlight lang="lua">pTeam = Teams[pPlayer:GetTeam()];</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TurnsRemaining.lua (G&K)}}
:<code>DLC/Expansion/Scenarios/SteampunkScenario/TurnsRemaining.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0528}}<syntaxhighlight lang="lua">if (Players[iPlayer]:GetTeam() == iTeam) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TutorialChecks.lua}}
:<code>Tutorial/TutorialChecks.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1064}}<syntaxhighlight lang="lua">if (player:GetTeam() ~= iOtherTeam and pOtherPlayer:IsAlive()) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|UnitFlagManager.lua}}
:<code>UI/InGame/UnitFlagManager.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0849}}<syntaxhighlight lang="lua">if( Game.GetActiveTeam() == Players[ self.m_PlayerID ]:GetTeam() ) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|VictoryProgress.lua}}
:<code>UI/InGame/Popups/VictoryProgress.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0270}}<syntaxhighlight lang="lua">local pTeam = Teams[ pPlayer:GetTeam() ];</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0374}}<syntaxhighlight lang="lua">not pPlayer:IsAlive() or Teams[pPlayer:GetTeam()]:GetLiberatedByTeam() ~= -1,</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0440}}<syntaxhighlight lang="lua">if(Teams[pPlayer:GetTeam()]:GetProjectCount(proj) > 0)then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0604}}<syntaxhighlight lang="lua">local pTeamB = Teams[ playerB:GetTeam() ];</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|VictoryProgress.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/Popups/VictoryProgress.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0669}}<syntaxhighlight lang="lua">table.sort(sortedPlayerList, function(a, b) return Teams[Players[b]:GetTeam()]:GetTotalProjectedVotes() <</syntaxhighlight>
{{CodeLine5|0670}}<syntaxhighlight lang="lua">Teams[Players[a]:GetTeam()]:GetTotalProjectedVotes() end );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|VoteResultsPopup.lua}}
:<code>UI/InGame/Popups/VoteResultsPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0043}}<syntaxhighlight lang="lua">if ((pPlayer:GetID() == activePlayer:GetID()) or (activePlayer:GetTeam() == pTeam:GetID())) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|VoteResultsPopup.lua (G&K)}}
:<code>DLC/Expansion/Scenarios/MedievalScenario/VoteResultsPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0237}}<syntaxhighlight lang="lua">iTeamLoop = Players[iPlayerLoop]:GetTeam();</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetTeam]]
[[Category:Civ5 Diplomacy API|GetTeam]]