{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Team}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''int''' Team:GetProjectedVotesFromMinorAllies<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|VictoryProgress.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/Popups/VictoryProgress.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0759}}<syntaxhighlight lang="lua">local iMinorVotes = pTeam:GetProjectedVotesFromMinorAllies();</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetProjectedVotesFromMinorAllies]]
[[Category:Civ5 United Nations API|GetProjectedVotesFromMinorAllies]]
[[Category:Civ5 City States API|GetProjectedVotesFromMinorAllies]]