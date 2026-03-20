{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a global function. Use: <code>include("IconSupport.lua")</code>
}}


=Usage=
<code>'''void''' CivIconHookup<b>(</b>{{Type5|PlayerID}} player, '''int''' iconSize, {{Type5|Image}} iconControl, {{Type5|Image}} teamColorControl, '''int''' shadowIconControl, '''int''' alwaysUseComposite, '''int''' shadowed<b>)</b></code>


'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|player:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|iconSize:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|iconControl:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|teamColorControl:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|shadowIconControl:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|alwaysUseComposite:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|shadowed:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|AdvisorCounselPopup.lua}}
:<code>UI/InGame/Popups/AdvisorCounselPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0195}}<syntaxhighlight lang="lua">CivIconHookup( Game.GetActivePlayer(), 64, Controls.Icon, Controls.CivIconBG, Controls.CivIconShadow, false, true );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ChoosePantheonPopup.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/Popups/ChoosePantheonPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0082}}<syntaxhighlight lang="lua">CivIconHookup( pPlayer:GetID(), 64, Controls.CivIcon, Controls.CivIconBG, Controls.CivIconShadow, false, true );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CityStateDiploPopup.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/Popups/CityStateDiploPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0259}}<syntaxhighlight lang="lua">CivIconHookup(iAlly, 32, Controls.AllyIcon, Controls.AllyIconBG, Controls.AllyIconShadow, false, true);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0264}}<syntaxhighlight lang="lua">CivIconHookup(-1, 32, Controls.AllyIcon, Controls.AllyIconBG, Controls.AllyIconShadow, false, true);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|Demographics.lua}}
:<code>UI/InGame/Popups/Demographics.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0333}}<syntaxhighlight lang="lua">CivIconHookup( iPlayerID, 32, control, controlBG, controlShadow, false, true);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0336}}<syntaxhighlight lang="lua">CivIconHookup( -1, 32, control, controlBG, controlShadow, false, true);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0445}}<syntaxhighlight lang="lua">CivIconHookup( iPlayer, 64, Controls.Icon, Controls.CivIconBG, Controls.CivIconShadow, false, true);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DiploCurrentDeals.lua}}
:<code>UI/InGame/Popups/DiploCurrentDeals.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0090}}<syntaxhighlight lang="lua">CivIconHookup( iOtherPlayer, 32, controlTable.CivIcon, controlTable.CivIconBG, controlTable.CivIconShadow, false, true );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DiploGlobalRelationships.lua}}
:<code>UI/InGame/Popups/DiploGlobalRelationships.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0056}}<syntaxhighlight lang="lua">CivIconHookup(iOtherPlayer, 64, controlTable.CivSymbol, controlTable.CivIconBG, controlTable.CivIconShadow, false, true);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DiploList.lua}}
:<code>UI/InGame/DiploList.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0210}}<syntaxhighlight lang="lua">CivIconHookup( g_iPlayer, 32, Controls.MyCivIcon, Controls.CivIconBG, Controls.CivIconShadow, false, true );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0276}}<syntaxhighlight lang="lua">CivIconHookup( iPlayerLoop, 32, controlTable.CivSymbol, controlTable.CivIconBG, controlTable.CivIconShadow, false, true );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DiploVotePopup.lua}}
:<code>UI/InGame/Popups/DiploVotePopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0063}}<syntaxhighlight lang="lua">CivIconHookup( iPlayerLoop, 45, controlTable.CivIcon, controlTable.CivIconBG, controlTable.CivIconShadow, false, true );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DiscussionDialog.lua}}
:<code>UI/InGame/LeaderHead/DiscussionDialog.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0054}}<syntaxhighlight lang="lua">CivIconHookup( g_iAIPlayer, 64, Controls.ThemSymbolShadow, Controls.CivIconBG, Controls.CivIconShadow, false, true );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|EconomicOverview.lua}}
:<code>UI/InGame/Popups/EconomicOverview.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0060}}<syntaxhighlight lang="lua">CivIconHookup( Game.GetActivePlayer(), 64, Controls.CivIcon, Controls.CivIconBG, Controls.CivIconShadow, false, true );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|EndGameMenu.lua}}
:<code>UI/InGame/Popups/EndGameMenu.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0285}}<syntaxhighlight lang="lua">CivIconHookup( Game.GetActivePlayer(), 80, Controls.CivIcon, Controls.CivIconBG, Controls.CivIconShadow, false, true );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|EspionageOverview.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/Popups/EspionageOverview.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0393}}<syntaxhighlight lang="lua">CivIconHookup(city:GetOwner(), 32, Controls.AgentLocationIcon, Controls.AgentLocationIconBG, Controls.AgentLocationIconShadow, false, true);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0584}}<syntaxhighlight lang="lua">CivIconHookup(city:GetOwner(), 32, agentEntry.AgentLocationIcon, agentEntry.AgentLocationIconBG, agentEntry.AgentLocationIconShadow, false, true);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0975}}<syntaxhighlight lang="lua">CivIconHookup( Game.GetActivePlayer(), 32, entry.CivIcon, entry.CivIconBG, entry.CivIconShadow, false, true);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1139}}<syntaxhighlight lang="lua">CivIconHookup( cityInfo.PlayerID, 32, entry.CivIcon, entry.CivIconBG, entry.CivIconShadow, false, true);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|GameMenu.lua}}
:<code>UI/InGame/Menus/GameMenu.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0201}}<syntaxhighlight lang="lua">CivIconHookup( iPlayer, 64, Controls.CivIcon, Controls.CivIconBG, Controls.CivIconShadow, false, true );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|LeaderHeadRoot.lua}}
:<code>UI/InGame/LeaderHead/LeaderHeadRoot.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0037}}<syntaxhighlight lang="lua">CivIconHookup( iPlayer, 64, Controls.ThemSymbolShadow, Controls.CivIconBG, Controls.CivIconShadow, false, true );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|MilitaryOverview.lua}}
:<code>UI/InGame/Popups/MilitaryOverview.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0369}}<syntaxhighlight lang="lua">CivIconHookup( 0, 64, Controls.Icon, Controls.CivIconBG, Controls.CivIconShadow, false, true );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|MPList.lua}}
:<code>UI/InGame/WorldView/MPList.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0144}}<syntaxhighlight lang="lua">CivIconHookup( pPlayer:GetID(), 32, controlTable.Icon, controlTable.CivIconBG, controlTable.CivIconShadow, false, true );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|NewTurn.lua}}
:<code>UI/InGame/NewTurn.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0040}}<syntaxhighlight lang="lua">CivIconHookup(  Game.GetActivePlayer(), 64, Controls.CivIcon, Controls.CivIconBG, Controls.CivIconShadow, false, true);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|NotificationPanel.lua}}
:<code>UI/InGame/WorldView/NotificationPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0200}}<syntaxhighlight lang="lua">CivIconHookup( iExtraGameData, 45, instance.CivIcon, instance.CivIconBG, instance.CivIconShadow, false, true );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0203}}<syntaxhighlight lang="lua">CivIconHookup( 22, 45, instance.CivIcon, instance.CivIconBG, instance.CivIconShadow, false, true );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0256}}<syntaxhighlight lang="lua">CivIconHookup( index, 80, instance.WarImage, instance.CivIconBG, instance.CivIconShadow, false, true );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0259}}<syntaxhighlight lang="lua">CivIconHookup( index, 45, instance.War1Image, instance.Civ1IconBG, instance.Civ1IconShadow, false, true );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0261}}<syntaxhighlight lang="lua">CivIconHookup( index, 45, instance.War2Image, instance.Civ2IconBG, instance.Civ2IconShadow, false, true );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0264}}<syntaxhighlight lang="lua">CivIconHookup( index, 80, instance.PeaceImage, instance.CivIconBG, instance.CivIconShadow, false, true );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0267}}<syntaxhighlight lang="lua">CivIconHookup( index, 45, instance.Peace1Image, instance.Civ1IconBG, instance.Civ1IconShadow, false, true );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0272}}<syntaxhighlight lang="lua">CivIconHookup( index, 45, instance.Peace2Image, instance.Civ2IconBG, instance.Civ2IconShadow, false, true );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ProductionPopup.lua}}
:<code>UI/InGame/Popups/ProductionPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0753}}<syntaxhighlight lang="lua">CivIconHookup( Game.GetActivePlayer(), 32, Controls.CivIcon, Controls.CivIconBG, Controls.CivIconShadow, false, true );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TradeLogic.lua}}
:<code>UI/InGame/WorldView/TradeLogic.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0926}}<syntaxhighlight lang="lua">CivIconHookup( g_iUs, 64, Controls.UsSymbolShadow, Controls.UsCivIconBG, Controls.UsCivIconShadow, false, true );</syntaxhighlight>
{{CodeLine5|0927}}<syntaxhighlight lang="lua">CivIconHookup( g_iThem, 64, Controls.ThemSymbolShadow, Controls.ThemCivIconBG, Controls.ThemCivIconShadow, false, true );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|2783}}<syntaxhighlight lang="lua">CivIconHookup( iLoopPlayer, 32, controlTable.CivSymbol, controlTable.CivIconBG, controlTable.CivIconShadow, false, true );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|VictoryProgress.lua}}
:<code>UI/InGame/Popups/VictoryProgress.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0900}}<syntaxhighlight lang="lua">CivIconHookup( iPlayer, iconSize, controlTable, controlBG, controlShadow, false, true );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0913}}<syntaxhighlight lang="lua">CivIconHookup(-1, iconSize, controlTable, controlBG, controlShadow, false, true );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|VictoryProgress.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/Popups/VictoryProgress.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0787}}<syntaxhighlight lang="lua">CivIconHookup(iLastVoteLeader, 32, controlTable.LastVoteCivIcon, controlTable.LastVoteCivIconBG, controlTable.LastVoteCivIconShadow, false, true);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|VictoryStatus.lua (G&K)}}
:<code>DLC/Expansion/Scenarios/SteampunkScenario/VictoryStatus.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0236}}<syntaxhighlight lang="lua">CivIconHookup(iActivePlayer, 64, Controls.CivIcon, Controls.CivIconBG, Controls.CivIconShadow, false, true);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|VoteResultsPopup.lua}}
:<code>UI/InGame/Popups/VoteResultsPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0047}}<syntaxhighlight lang="lua">CivIconHookup( pPlayer:GetID(), 32, controlTable.Icon, controlTable.IconBG, controlTable.IconShadow, false, true );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0054}}<syntaxhighlight lang="lua">CivIconHookup( -1, 32, controlTable.Icon, controlTable.IconBG, controlTable.IconShadow, false, true );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0082}}<syntaxhighlight lang="lua">CivIconHookup( pPlayer:GetID(), 32, controlTable.Icon, controlTable.IconBG, controlTable.IconShadow, false, true);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0123}}<syntaxhighlight lang="lua">CivIconHookup( pVoteCastTeam:GetLeaderID(), 32, controlTable.BallotIcon, controlTable.BallotIconBG, controlTable.BallotIconShadow, false, true );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0128}}<syntaxhighlight lang="lua">CivIconHookup( -1, 32, controlTable.BallotIcon, controlTable.BallotIconBG, controlTable.BallotIconShadow, false, true );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|WhosWinningPopup.lua}}
:<code>UI/InGame/Popups/WhosWinningPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0274}}<syntaxhighlight lang="lua">CivIconHookup( iPlayerID, 32, controlTable.Icon, controlTable.CivIconBG, controlTable.CivIconShadow, false, true);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0279}}<syntaxhighlight lang="lua">CivIconHookup( -1, 32, controlTable.Icon, controlTable.CivIconBG, controlTable.CivIconShadow, false, true);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|CivIconHookup]]