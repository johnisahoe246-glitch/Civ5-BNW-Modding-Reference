{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Team}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''int''' Team:GetTotalProjectedVotes<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|VictoryProgress.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/Popups/VictoryProgress.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0419}}<syntaxhighlight lang="lua">Controls.VotesHave:SetText(Teams[curTeam]:GetTotalProjectedVotes());</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0669}}<syntaxhighlight lang="lua">table.sort(sortedPlayerList, function(a, b) return Teams[Players[b]:GetTeam()]:GetTotalProjectedVotes() <</syntaxhighlight>
{{CodeLine5|0670}}<syntaxhighlight lang="lua">Teams[Players[a]:GetTeam()]:GetTotalProjectedVotes() end );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0829}}<syntaxhighlight lang="lua">local iProjectedVotes = pTeam:GetTotalProjectedVotes();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|VictoryProgress.lua (G&K)}}
:<code>DLC/Expansion/Scenarios/MedievalScenario/VictoryProgress.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1158}}<syntaxhighlight lang="lua">iVotes = iVotes + pTeam:GetTotalProjectedVotes();</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetTotalProjectedVotes]]
[[Category:Civ5 United Nations API|GetTotalProjectedVotes]]
[[Category:Civ5 Score API|GetTotalProjectedVotes]]