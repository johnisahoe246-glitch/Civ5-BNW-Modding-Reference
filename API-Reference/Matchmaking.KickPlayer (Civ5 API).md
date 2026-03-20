{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Matchmaking}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''void''' Matchmaking.KickPlayer<b>(</b>{{Type5|PlayerID}} player<b>)</b></code>


'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|player:
|valign="top"| ''No description available.''
|}


=Source code samples=
{{PseudoH4|StagingRoom.lua}}
:<code>UI/FrontEnd/Multiplayer/StagingRoom.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0174}}<syntaxhighlight lang="lua">Matchmaking.KickPlayer( playerID );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1328}}<syntaxhighlight lang="lua">Matchmaking.KickPlayer( iPlayerID );</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|KickPlayer]]
[[Category:Civ5 Players API|KickPlayer]]