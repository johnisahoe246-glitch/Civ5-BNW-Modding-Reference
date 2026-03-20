{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Team}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''int''' Team:IsHasMet<b>(</b>{{Type5|TeamID}} index<b>)</b></code>


'''Returned Value'''
:No description available.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|index:
|valign="top"| ''No description available.''
|}


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
{{CodeLine5|0265}}<syntaxhighlight lang="lua">if (Teams[Players[iAlly]:GetTeam()]:IsHasMet(Game.GetActiveTeam())) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|Demographics.lua}}
:<code>UI/InGame/Popups/Demographics.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0335}}<syntaxhighlight lang="lua">elseif (not pTeam:IsHasMet(Game.GetActiveTeam())) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DiploGlobalRelationships.lua}}
:<code>UI/InGame/Popups/DiploGlobalRelationships.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0041}}<syntaxhighlight lang="lua">if (g_pUsTeam:IsHasMet(iOtherTeam)) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0153}}<syntaxhighlight lang="lua">if (g_pUsTeam:IsHasMet(iThirdTeam) or iThirdPlayer == g_iUs) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DiploList.lua}}
:<code>UI/InGame/DiploList.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0254}}<syntaxhighlight lang="lua">if (g_pTeam:IsHasMet(iOtherTeam)) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0424}}<syntaxhighlight lang="lua">g_pTeam:IsHasMet( iOtherTeam ) ) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DiploRelationships.lua}}
:<code>UI/InGame/Popups/DiploRelationships.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0056}}<syntaxhighlight lang="lua">if (pTeam:IsHasMet(iOtherTeam)) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DiploVotePopup.lua}}
:<code>UI/InGame/Popups/DiploVotePopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0058}}<syntaxhighlight lang="lua">if (pTeam:IsHasMet(iTeamLoop)) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DiscussionDialog.lua}}
:<code>UI/InGame/LeaderHead/DiscussionDialog.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0431}}<syntaxhighlight lang="lua">if (pTeam:IsHasMet(iThirdPartyTeam)) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0865}}<syntaxhighlight lang="lua">if (not pActiveTeam:IsHasMet(iThirdPartyTeam)) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0870}}<syntaxhighlight lang="lua">if (not Teams[g_iAITeam]:IsHasMet(iThirdPartyTeam)) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|MPList.lua}}
:<code>UI/InGame/WorldView/MPList.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0104}}<syntaxhighlight lang="lua">local bMet = g_pLocalTeam:IsHasMet( iTeam );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|PlotMouseoverInclude.lua}}
:<code>UI/InGame/PlotMouseoverInclude.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0012}}<syntaxhighlight lang="lua">if( pOtherPlayer:IsMinorCiv() and iActiveTeam ~= iOtherTeam and pOtherPlayer:IsAlive() and pTeam:IsHasMet( iOtherTeam ) ) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ReligionOverview.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/Popups/ReligionOverview.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0506}}<syntaxhighlight lang="lua">if(not activeTeam:IsHasMet(pPlayer:GetTeam())) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TradeLogic.lua}}
:<code>UI/InGame/WorldView/TradeLogic.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0471}}<syntaxhighlight lang="lua">g_pUsTeam:IsHasMet( iLoopTeam ) and g_pThemTeam:IsHasMet( iLoopTeam ) and</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TutorialChecks.lua}}
:<code>Tutorial/TutorialChecks.lua</code>
:{{CodeBegin5}}
{{CodeLine5|2812}}<syntaxhighlight lang="lua">if (pTeam:IsHasMet(iOtherTeam) and not pTeam:IsAtWar(iOtherTeam)) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|VictoryProgress.lua}}
:<code>UI/InGame/Popups/VictoryProgress.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0457}}<syntaxhighlight lang="lua">if (Teams[leadAI:GetTeam()]:IsHasMet(Game.GetActiveTeam()) or Game:IsNetworkMultiPlayer()) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0837}}<syntaxhighlight lang="lua">if (pTeam:IsHasMet(Game.GetActiveTeam()) or Game:IsNetworkMultiPlayer()) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|VictoryProgress.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/Popups/VictoryProgress.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0713}}<syntaxhighlight lang="lua">if (Teams[iActiveTeam] ~= nil and Teams[iActiveTeam]:IsHasMet(iTeamLoop)) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0746}}<syntaxhighlight lang="lua">local bShowToolTips = (Teams[iActiveTeam]:IsHasMet(iTeam) and pTeam:IsAlive());</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|VictoryProgress.lua (G&K)}}
:<code>DLC/Expansion/Scenarios/SteampunkScenario/VictoryProgress.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0742}}<syntaxhighlight lang="lua">local bShowToolTips = Teams[iActiveTeam]:IsHasMet(iTeam);</syntaxhighlight>
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
[[Category:Civ5 Methods and Functions|IsHasMet]]
[[Category:Civ5 Diplomacy API|IsHasMet]]