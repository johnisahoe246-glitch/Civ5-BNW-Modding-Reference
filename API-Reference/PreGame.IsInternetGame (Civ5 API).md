{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|PreGame}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''int''' PreGame.IsInternetGame<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|DiploCorner.lua}}
:<code>UI/InGame/WorldView/DiploCorner.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0201}}<syntaxhighlight lang="lua">local bShow = Matchmaking.IsHost() and PreGame.IsInternetGame();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|LoadMenu.lua}}
:<code>UI/FrontEnd/LoadMenu.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0065}}<syntaxhighlight lang="lua">if PreGame.IsInternetGame() then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|MPGameSetupScreen.lua}}
:<code>UI/FrontEnd/Multiplayer/GameSetup/MPGameSetupScreen.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0048}}<syntaxhighlight lang="lua">if (PreGame.IsInternetGame()) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0094}}<syntaxhighlight lang="lua">Controls.PrivateGameCheckbox:SetHide( not PreGame.IsInternetGame() );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|MPList.lua}}
:<code>UI/InGame/WorldView/MPList.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0191}}<syntaxhighlight lang="lua">if PreGame.IsInternetGame() then      -- Pings only valid with the Steam transport</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|StagingRoom.lua}}
:<code>UI/FrontEnd/Multiplayer/StagingRoom.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0589}}<syntaxhighlight lang="lua">if ( PreGame.IsInternetGame() and not isHost ) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0591}}<syntaxhighlight lang="lua">elseif ( not PreGame.IsInternetGame() and not isHost ) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0599}}<syntaxhighlight lang="lua">local bIsInternet = PreGame.IsInternetGame();</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|IsInternetGame]]