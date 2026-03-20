{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Game}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>{{Type5|TeamID}} Game.GetActiveTeam<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|CityBannerManager.lua}}
:<code>UI/InGame/CityBannerManager.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0459}}<syntaxhighlight lang="lua">if (Teams[Game.GetActiveTeam()]:IsHasMet(player:GetTeam())) then</syntaxhighlight>
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
{{CodeLine5|0061}}<syntaxhighlight lang="lua">local iActiveTeam = Game.GetActiveTeam();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0265}}<syntaxhighlight lang="lua">if (Teams[Players[iAlly]:GetTeam()]:IsHasMet(Game.GetActiveTeam())) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0311}}<syntaxhighlight lang="lua">local iResourceType = pTargetPlot:GetResourceType(Game.GetActiveTeam());</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CivsAlive.lua - DLC_01 DLC}}
:<code>DLC/DLC_01/Scenarios/Mongol Scenario/CivsAlive.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0049}}<syntaxhighlight lang="lua">Game.SetWinner(Game.GetActiveTeam(), GameInfo.Victories["VICTORY_DOMINATION"].ID);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DeclareWarMovePopup.lua}}
:<code>UI/InGame/PopupsGeneric/DeclareWarMovePopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0019}}<syntaxhighlight lang="lua">if (not owner:IsMinorCiv() and Teams[Game.GetActiveTeam()]:IsOpenBordersTradingAllowed()) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DeclareWarMovePopup.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/PopupsGeneric/DeclareWarMovePopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0019}}<syntaxhighlight lang="lua">if (not owner:IsMinorCiv() and Teams[Game.GetActiveTeam()]:IsOpenBordersTradingAllowedWithTeam(plot:GetTeam())) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|Demographics.lua}}
:<code>UI/InGame/Popups/Demographics.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0335}}<syntaxhighlight lang="lua">elseif (not pTeam:IsHasMet(Game.GetActiveTeam())) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DiploList.lua}}
:<code>UI/InGame/DiploList.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0469}}<syntaxhighlight lang="lua">local bWar = Teams[Game.GetActiveTeam()]:IsAtWar(pOtherPlayer:GetTeam());</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DiploRelationships.lua}}
:<code>UI/InGame/Popups/DiploRelationships.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0376}}<syntaxhighlight lang="lua">local bWar = Teams[Game.GetActiveTeam()]:IsAtWar(pPlayer:GetTeam());</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DiscussionDialog.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/LeaderHead/DiscussionDialog.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0226}}<syntaxhighlight lang="lua">if (not pAIPlayer:IsStopSpyingMessageTooSoon(iActivePlayer) and bHasAgents and (g_iAITeam ~= Game.GetActiveTeam())) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|EndGameMenu.lua}}
:<code>UI/InGame/Popups/EndGameMenu.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0122}}<syntaxhighlight lang="lua">if( team == Game.GetActiveTeam() ) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|EnemyUnitPanel.lua}}
:<code>UI/InGame/WorldView/EnemyUnitPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1798}}<syntaxhighlight lang="lua">local iTeam = Game.GetActiveTeam()</syntaxhighlight>
{{CodeLine5|1799}}<syntaxhighlight lang="lua">local pTeam = Teams[iTeam]</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1922}}<syntaxhighlight lang="lua">local myTeamID = Game.GetActiveTeam();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|GenericWorldAnchor.lua}}
:<code>UI/InGame/GenericWorldAnchor.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0242}}<syntaxhighlight lang="lua">local iResource = pPlot:GetResourceType(Game.GetActiveTeam());</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|InfoTooltipInclude.lua}}
:<code>UI/InGame/InfoTooltipInclude.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0010}}<syntaxhighlight lang="lua">local pActiveTeam = Teams[Game.GetActiveTeam()];</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|InGame.lua}}
:<code>UI/InGame/InGame.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0085}}<syntaxhighlight lang="lua">local team = Game.GetActiveTeam();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|LeaderHeadRoot.lua}}
:<code>UI/InGame/LeaderHead/LeaderHeadRoot.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0151}}<syntaxhighlight lang="lua">if (Game.GetActiveTeam() == g_iAITeam) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0267}}<syntaxhighlight lang="lua">local bAtWar = Teams[Game.GetActiveTeam()]:IsAtWar(g_iAITeam);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0288}}<syntaxhighlight lang="lua">if (iTeam1 == Game.GetActiveTeam() and iTeam2 == g_iAITeam) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|PathHelpManager.lua}}
:<code>UI/InGame/WorldView/PathHelpManager.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0039}}<syntaxhighlight lang="lua">if( plot:IsRevealed( Game.GetActiveTeam(), false ) ) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ResourceIconManager.lua}}
:<code>UI/InGame/ResourceIconManager.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0088}}<syntaxhighlight lang="lua">if( not bIsBuilt and pPlayer:GetTeam() == Game.GetActiveTeam() ) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0104}}<syntaxhighlight lang="lua">if( not plot:IsRevealed( Game.GetActiveTeam(), false ) ) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ResourceTooltipGenerator.lua}}
:<code>UI/InGame/ResourceTooltipGenerator.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0006}}<syntaxhighlight lang="lua">local iResourceID = plot:GetResourceType(Game.GetActiveTeam());</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TechAwardPopup.lua}}
:<code>UI/InGame/Popups/TechAwardPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0015}}<syntaxhighlight lang="lua">local activeTeamID = Game.GetActiveTeam();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0147}}<syntaxhighlight lang="lua">activeTeamID = Game.GetActiveTeam();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TurnsRemaining.lua (G&K)}}
:<code>DLC/Expansion/Scenarios/MedievalScenario/TurnsRemaining.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0283}}<syntaxhighlight lang="lua">if (Teams[player:GetTeam()]:IsHasMet(Game.GetActiveTeam())) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|UnitFlagManager.lua}}
:<code>UI/InGame/UnitFlagManager.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0849}}<syntaxhighlight lang="lua">if( Game.GetActiveTeam() == Players[ self.m_PlayerID ]:GetTeam() ) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1411}}<syntaxhighlight lang="lua">if( plot:IsVisible( Game.GetActiveTeam() ) ) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|VictoryProgress.lua}}
:<code>UI/InGame/Popups/VictoryProgress.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0289}}<syntaxhighlight lang="lua">local iTeam = Game.GetActiveTeam();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0408}}<syntaxhighlight lang="lua">local curTeam = Game.GetActiveTeam()</syntaxhighlight>
{{CodeLine5|0409}}<syntaxhighlight lang="lua">for i, v in pairs(Teams) do</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0457}}<syntaxhighlight lang="lua">if (Teams[leadAI:GetTeam()]:IsHasMet(Game.GetActiveTeam()) or Game:IsNetworkMultiPlayer()) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0837}}<syntaxhighlight lang="lua">if (pTeam:IsHasMet(Game.GetActiveTeam()) or Game:IsNetworkMultiPlayer()) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0986}}<syntaxhighlight lang="lua">local pTeam = Teams[Game.GetActiveTeam()];</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|VoteResultsPopup.lua}}
:<code>UI/InGame/Popups/VoteResultsPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0126}}<syntaxhighlight lang="lua">elseif (not pVoteCastTeam:IsHasMet(Game.GetActiveTeam())) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|VoteResultsPopup.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/Popups/VoteResultsPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0129}}<syntaxhighlight lang="lua">if (Teams[Game.GetActiveTeam()]:IsHasMet(iTeam)) then</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetActiveTeam]]
[[Category:Civ5 Diplomacy API|GetActiveTeam]]