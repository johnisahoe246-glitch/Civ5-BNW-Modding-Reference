{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|PreGame}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''int''' PreGame.IsHotSeatGame<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|InGame.lua}}
:<code>UI/InGame/InGame.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0077}}<syntaxhighlight lang="lua">elseif ( wParam == Keys.VK_OEM_3 and UI:DebugFlag() and not PreGame.IsMultiplayerGame() and not PreGame.IsHotSeatGame()) then -- ~</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0082}}<syntaxhighlight lang="lua">elseif ( wParam == Keys.Z and UIManager:GetControl() and UI:DebugFlag() and not PreGame.IsMultiplayerGame() and not PreGame.IsHotSeatGame()) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|LoadMenu.lua}}
:<code>UI/FrontEnd/LoadMenu.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0068}}<syntaxhighlight lang="lua">if (PreGame.IsHotSeatGame()) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0721}}<syntaxhighlight lang="lua">if PreGame.IsHotSeatGame() then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|LoadScreen.lua}}
:<code>UI/FrontEnd/LoadScreen.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0092}}<syntaxhighlight lang="lua">if (not PreGame.IsMultiplayerGame() and not PreGame.IsHotSeatGame()) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0128}}<syntaxhighlight lang="lua">if (PreGame.IsMultiplayerGame() or PreGame.IsHotSeatGame()) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|MiniMapPanel.lua}}
:<code>UI/InGame/WorldView/MiniMapPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0318}}<syntaxhighlight lang="lua">OptionsManager.CommitGameOptions( PreGame.IsHotSeatGame() );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0369}}<syntaxhighlight lang="lua">OptionsManager.CommitGameOptions(PreGame.IsHotSeatGame());</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|MPGameOptions.lua}}
:<code>UI/FrontEnd/Multiplayer/GameSetup/MPGameOptions.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0017}}<syntaxhighlight lang="lua">if ( PreGame.IsHotSeatGame() ) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0038}}<syntaxhighlight lang="lua">return (Matchmaking.IsHost() and PreGame.GetLoadFileName() == "") or PreGame.IsHotSeatGame() or Matchmaking.GetLocalID() == -1;</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0045}}<syntaxhighlight lang="lua">return (PreGame.GetLoadFileName() == "" and Matchmaking.GetLocalID() == -1) or PreGame.IsHotSeatGame();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0440}}<syntaxhighlight lang="lua">if (not PreGame.IsHotSeatGame()) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|MPGameSetupScreen.lua}}
:<code>UI/FrontEnd/Multiplayer/GameSetup/MPGameSetupScreen.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0018}}<syntaxhighlight lang="lua">if (not PreGame.IsHotSeatGame() ) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0095}}<syntaxhighlight lang="lua">Controls.GameNameBox:SetHide( PreGame.IsHotSeatGame() );</syntaxhighlight>
{{CodeLine5|0096}}<syntaxhighlight lang="lua">Controls.GameNameDivider:SetHide( PreGame.IsHotSeatGame() );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|OptionsMenu.lua}}
:<code>UI/Options/OptionsMenu.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0305}}<syntaxhighlight lang="lua">if( bIsInGame and (PreGame.IsMultiplayerGame() or PreGame.IsHotSeatGame()) )then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|SetCivNames.lua}}
:<code>UI/FrontEnd/GameSetup/SetCivNames.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0255}}<syntaxhighlight lang="lua">local bIsHotSeat = PreGame.IsHotSeatGame();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|StagingRoom.lua}}
:<code>UI/FrontEnd/Multiplayer/StagingRoom.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0436}}<syntaxhighlight lang="lua">if( PreGame.IsHotSeatGame() ) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0587}}<syntaxhighlight lang="lua">if ( not PreGame.IsHotSeatGame() ) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0733}}<syntaxhighlight lang="lua">if( ContextPtr:IsHidden() == false and not PreGame.IsHotSeatGame()) then</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|IsHotSeatGame]]