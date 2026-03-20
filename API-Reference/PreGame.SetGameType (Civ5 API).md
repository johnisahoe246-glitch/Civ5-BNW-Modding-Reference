{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|PreGame}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''void''' PreGame.SetGameType<b>(</b>{{Type5|GameType}} gameType<b>)</b></code>


'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|gameType:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|MultiplayerSelect.lua}}
:<code>UI/FrontEnd/Multiplayer/MultiplayerSelect.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0012}}<syntaxhighlight lang="lua">PreGame.SetGameType(GameTypes.GAME_NETWORK_MULTIPLAYER);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0041}}<syntaxhighlight lang="lua">PreGame.SetGameType(GameTypes.GAME_HOTSEAT_MULTIPLAYER);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0066}}<syntaxhighlight lang="lua">PreGame.SetGameType( GameTypes.GAME_SINGLE_PLAYER );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|SinglePlayer.lua}}
:<code>UI/FrontEnd/SinglePlayer.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0020}}<syntaxhighlight lang="lua">PreGame.SetGameType(GameTypes.GAME_SINGLE_PLAYER);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|StagingRoom.lua}}
:<code>UI/FrontEnd/Multiplayer/StagingRoom.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0605}}<syntaxhighlight lang="lua">PreGame.SetGameType(eGameType);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|SetGameType]]
[[Category:Civ5 Game Settings API|SetGameType]]