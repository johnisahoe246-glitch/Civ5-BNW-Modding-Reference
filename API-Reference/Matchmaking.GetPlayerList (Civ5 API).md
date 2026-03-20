{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Matchmaking}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>table({{Type5|PlayerID}} => '''table''') Matchmaking.GetPlayerList<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|DiploList.lua}}
:<code>UI/InGame/DiploList.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0008}}<syntaxhighlight lang="lua">local m_PlayerTable = Matchmaking.GetPlayerList();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|StagingRoom.lua}}
:<code>UI/FrontEnd/Multiplayer/StagingRoom.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0031}}<syntaxhighlight lang="lua">local playerList = Matchmaking.GetPlayerList();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0280}}<syntaxhighlight lang="lua">local playerTable = Matchmaking.GetPlayerList();</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetPlayerList]]
[[Category:Civ5 Players API|GetPlayerList]]