{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Matchmaking}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''int''' Matchmaking.IsHost<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|DiploCorner.lua}}
:<code>UI/InGame/WorldView/DiploCorner.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0201}}<syntaxhighlight lang="lua">local bShow = Matchmaking.IsHost() and PreGame.IsInternetGame();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|GameMenu.lua}}
:<code>UI/InGame/Menus/GameMenu.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0141}}<syntaxhighlight lang="lua">if(not Matchmaking.IsHost()) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|JoiningRoom.lua}}
:<code>UI/FrontEnd/Multiplayer/JoiningRoom.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0027}}<syntaxhighlight lang="lua">if Matchmaking.IsHost() then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0102}}<syntaxhighlight lang="lua">if not Matchmaking.IsHost() then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|MPGameOptions.lua}}
:<code>UI/FrontEnd/Multiplayer/GameSetup/MPGameOptions.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0038}}<syntaxhighlight lang="lua">return (Matchmaking.IsHost() and PreGame.GetLoadFileName() == "") or PreGame.IsHotSeatGame() or Matchmaking.GetLocalID() == -1;</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0218}}<syntaxhighlight lang="lua">if(Matchmaking.GetLocalID() == -1 or Matchmaking.IsHost()) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|OptionsMenu.lua}}
:<code>UI/Options/OptionsMenu.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0098}}<syntaxhighlight lang="lua">if (Matchmaking.IsHost()) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0317}}<syntaxhighlight lang="lua">if( bIsInGame and PreGame.IsMultiplayerGame() and not Matchmaking.IsHost()) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|StagingRoom.lua}}
:<code>UI/FrontEnd/Multiplayer/StagingRoom.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0276}}<syntaxhighlight lang="lua">m_bIsHost = Matchmaking.IsHost();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0585}}<syntaxhighlight lang="lua">local isHost = Matchmaking.IsHost();</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|IsHost]]