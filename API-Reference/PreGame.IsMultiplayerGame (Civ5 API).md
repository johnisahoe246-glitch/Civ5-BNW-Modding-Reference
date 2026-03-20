{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|PreGame}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''int''' PreGame.IsMultiplayerGame<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|ActionInfoPanel.lua}}
:<code>UI/InGame/WorldView/ActionInfoPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0084}}<syntaxhighlight lang="lua">if Network.HasSentNetTurnComplete() and PreGame.IsMultiplayerGame() then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0154}}<syntaxhighlight lang="lua">if not player:IsTurnActive() or (PreGame.IsMultiplayerGame() and Network.HasSentNetTurnComplete()) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0224}}<syntaxhighlight lang="lua">if Network.HasSentNetTurnAllComplete() and PreGame.IsMultiplayerGame() then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0272}}<syntaxhighlight lang="lua">if not player:IsTurnActive() or (PreGame.IsMultiplayerGame() and Network.HasSentNetTurnComplete()) or Game.IsProcessingMessages() then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DebugMenu.lua}}
:<code>UI/InGame/DebugMenu.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0405}}<syntaxhighlight lang="lua">if(not isHide and PreGame.IsMultiplayerGame()) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|InGame.lua}}
:<code>UI/InGame/InGame.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0073}}<syntaxhighlight lang="lua">if ( wParam == Keys.VK_OEM_3 and UI:ShiftKeyDown() and UI:DebugFlag() and PreGame.IsMultiplayerGame()) then -- shift - ~</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0077}}<syntaxhighlight lang="lua">elseif ( wParam == Keys.VK_OEM_3 and UI:DebugFlag() and not PreGame.IsMultiplayerGame() and not PreGame.IsHotSeatGame()) then -- ~</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0082}}<syntaxhighlight lang="lua">elseif ( wParam == Keys.Z and UIManager:GetControl() and UI:DebugFlag() and not PreGame.IsMultiplayerGame() and not PreGame.IsHotSeatGame()) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|LoadScreen.lua}}
:<code>UI/FrontEnd/LoadScreen.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0092}}<syntaxhighlight lang="lua">if (not PreGame.IsMultiplayerGame() and not PreGame.IsHotSeatGame()) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0128}}<syntaxhighlight lang="lua">if (PreGame.IsMultiplayerGame() or PreGame.IsHotSeatGame()) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|OptionsMenu.lua}}
:<code>UI/Options/OptionsMenu.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0097}}<syntaxhighlight lang="lua">if (PreGame.IsMultiplayerGame()) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0305}}<syntaxhighlight lang="lua">if( bIsInGame and (PreGame.IsMultiplayerGame() or PreGame.IsHotSeatGame()) )then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0317}}<syntaxhighlight lang="lua">if( bIsInGame and PreGame.IsMultiplayerGame() and not Matchmaking.IsHost()) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|SelectMapSize.lua}}
:<code>UI/FrontEnd/GameSetup/SelectMapSize.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0061}}<syntaxhighlight lang="lua">if(not PreGame.IsMultiplayerGame()) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|UnitFlagManager.lua}}
:<code>UI/InGame/UnitFlagManager.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0193}}<syntaxhighlight lang="lua">if(PreGame.IsMultiplayerGame() and o.m_Player:IsHuman()) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|VictoryProgress.lua}}
:<code>UI/InGame/Popups/VictoryProgress.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0530}}<syntaxhighlight lang="lua">SetCivName(pPlayer, i, controlTable.Score, PreGame.IsMultiplayerGame(), 730);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|IsMultiplayerGame]]