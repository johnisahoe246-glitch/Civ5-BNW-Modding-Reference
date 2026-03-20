{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Team}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''int''' Team:IsAtWar<b>(</b>{{Type5|TeamID}} index<b>)</b></code>


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
{{CodeLine5|0469}}<syntaxhighlight lang="lua">local bWar = Teams[iActiveTeam]:IsAtWar(team);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CityStateDiploPopup.lua}}
:<code>UI/InGame/Popups/CityStateDiploPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0076}}<syntaxhighlight lang="lua">local bWar = pActiveTeam:IsAtWar(iTeam);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CityStateStatusHelper.lua (G&K)}}
:<code>DLC/Expansion/UI/CityStateStatusHelper.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0060}}<syntaxhighlight lang="lua">local bWar = pMajorTeam:IsAtWar(iMinorTeam);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CivsAlive.lua - DLC_01 DLC}}
:<code>DLC/DLC_01/Scenarios/Mongol Scenario/CivsAlive.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0141}}<syntaxhighlight lang="lua">if (pHumanTeam:IsAtWar(eDestroyedTeam)) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DiploCorner.lua}}
:<code>UI/InGame/WorldView/DiploCorner.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0277}}<syntaxhighlight lang="lua">if( (pUsTeam:IsAtWar( iOtherTeam ) and (g_bAlwaysWar or g_bNoChangeWar) ) or</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DiploGlobalRelationships.lua}}
:<code>UI/InGame/Popups/DiploGlobalRelationships.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0119}}<syntaxhighlight lang="lua">if (g_pUsTeam:IsAtWar(iOtherTeam)) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0156}}<syntaxhighlight lang="lua">if (pOtherTeam:IsAtWar(iThirdTeam) and iThirdPlayer ~= g_iUs) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DiploList.lua}}
:<code>UI/InGame/DiploList.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0156}}<syntaxhighlight lang="lua">if( (g_pTeam:IsAtWar( iOtherTeam ) and (g_bAlwaysWar or g_bNoChangeWar) ) or</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0301}}<syntaxhighlight lang="lua">if( g_pTeam:IsAtWar( iOtherTeam ) ) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0347}}<syntaxhighlight lang="lua">if( not( g_pTeam:IsAtWar( pOtherPlayer:GetTeam() ) and (g_bAlwaysWar or g_bNoChangeWar) ) ) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0355}}<syntaxhighlight lang="lua">not g_pTeam:IsAtWar( pOtherPlayer:GetTeam()) and g_pTeam:CanDeclareWar(pOtherPlayer:GetTeam()) and</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0441}}<syntaxhighlight lang="lua">if (g_pTeam:IsAtWar(iOtherTeam)) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0469}}<syntaxhighlight lang="lua">local bWar = Teams[Game.GetActiveTeam()]:IsAtWar(pOtherPlayer:GetTeam());</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0490}}<syntaxhighlight lang="lua">if( iQuest == -1 or g_pTeam:IsAtWar(iOtherTeam) ) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DiploList.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/DiploList.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0497}}<syntaxhighlight lang="lua">or g_pTeam:IsAtWar(iOtherTeam)) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DiploRelationships.lua}}
:<code>UI/InGame/Popups/DiploRelationships.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0066}}<syntaxhighlight lang="lua">if (pTeam:IsAtWar(iOtherTeam)) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0376}}<syntaxhighlight lang="lua">local bWar = Teams[Game.GetActiveTeam()]:IsAtWar(pPlayer:GetTeam());</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DiscussionDialog.lua}}
:<code>UI/InGame/LeaderHead/DiscussionDialog.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0066}}<syntaxhighlight lang="lua">if (pActiveTeam:IsAtWar(g_iAITeam)) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|EnemyUnitPanel.lua}}
:<code>UI/InGame/WorldView/EnemyUnitPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1809}}<syntaxhighlight lang="lua">if (pTeam:IsAtWar(pCity:GetTeam()) or (UIManager:GetAlt() and pCity:GetOwner() ~= iTeam)) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1845}}<syntaxhighlight lang="lua">if (pTeam:IsAtWar(pUnit:GetTeam()) or (UIManager:GetAlt() and pUnit:GetOwner() ~= iTeam)) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1941}}<syntaxhighlight lang="lua">if (myTeam:IsAtWar(theirUnit:GetTeam()) or (UIManager:GetAlt() and theirUnit:GetOwner() ~= myTeamID)) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|InfoTooltipInclude.lua}}
:<code>UI/InGame/InfoTooltipInclude.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0758}}<syntaxhighlight lang="lua">if (pActiveTeam:IsAtWar(iOtherTeam)) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|LeaderHeadRoot.lua}}
:<code>UI/InGame/LeaderHead/LeaderHeadRoot.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0160}}<syntaxhighlight lang="lua">local bAtWar = pActiveTeam:IsAtWar(g_iAITeam);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0267}}<syntaxhighlight lang="lua">local bAtWar = Teams[Game.GetActiveTeam()]:IsAtWar(g_iAITeam);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|MPList.lua}}
:<code>UI/InGame/WorldView/MPList.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0168}}<syntaxhighlight lang="lua">if( g_pLocalTeam:IsAtWar( pPlayer:GetTeam() ) ) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|PlotMouseoverInclude.lua}}
:<code>UI/InGame/PlotMouseoverInclude.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0286}}<syntaxhighlight lang="lua">elseif pTeam:IsAtWar(unitTeam) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0362}}<syntaxhighlight lang="lua">elseif pTeam:IsAtWar(plotTeam) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TradeLogic.lua}}
:<code>UI/InGame/WorldView/TradeLogic.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0261}}<syntaxhighlight lang="lua">print( "war: " .. tostring( g_pUsTeam:IsAtWar( g_iThemTeam ) ) );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0265}}<syntaxhighlight lang="lua">if( (g_pUsTeam:IsAtWar( g_iThemTeam ) and (g_bAlwaysWar or g_bNoChangeWar) ) or</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0292}}<syntaxhighlight lang="lua">if( g_pUsTeam:IsAtWar( g_iThemTeam ) ) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0616}}<syntaxhighlight lang="lua">if (g_iUsTeam >= 0 and g_iThemTeam >= 0 and Teams[g_iUsTeam]:IsAtWar(g_iThemTeam)) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|2574}}<syntaxhighlight lang="lua">if (not Teams[iLoopTeam]:IsAtWar(iFromTeam)) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|2587}}<syntaxhighlight lang="lua">elseif (pMinorTeam:IsAtWar(iFromTeam) and iAlly ~= -1 and Teams[Players[iAlly]:GetTeam()]:IsAtWar(iFromTeam)) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|2608}}<syntaxhighlight lang="lua">if (Teams[iLoopTeam]:IsAtWar(iFromTeam)) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TradeLogic.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/WorldView/TradeLogic.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1374}}<syntaxhighlight lang="lua">if ( g_pUsTeam:IsAtWar( g_iThemTeam ) ) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|2982}}<syntaxhighlight lang="lua">if (g_pUsTeam:IsAtWar(g_iThemTeam )) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TutorialChecks.lua}}
:<code>Tutorial/TutorialChecks.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1125}}<syntaxhighlight lang="lua">if (pOtherPlayer:IsMinorCiv() and pOtherPlayer:IsAlive() and not pTeam:IsAtWar(iOtherTeam)) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|2464}}<syntaxhighlight lang="lua">if (iPlotOwner >= 0 and Players[iPlotOwner]:IsMinorCiv() and not pTeam:IsAtWar(iPlotTeam)) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|2812}}<syntaxhighlight lang="lua">if (pTeam:IsHasMet(iOtherTeam) and not pTeam:IsAtWar(iOtherTeam)) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|VictoryProgress.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/Popups/VictoryProgress.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0798}}<syntaxhighlight lang="lua">if (Teams[iActiveTeam]:IsAtWar(iTeam)) then</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|IsAtWar]]
[[Category:Civ5 Diplomacy API|IsAtWar]]