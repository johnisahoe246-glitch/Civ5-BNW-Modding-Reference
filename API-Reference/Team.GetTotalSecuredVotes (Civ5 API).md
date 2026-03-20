{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Team}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''int''' Team:GetTotalSecuredVotes<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|VictoryProgress.lua}}
:<code>UI/InGame/Popups/VictoryProgress.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0419}}<syntaxhighlight lang="lua">Controls.VotesHave:SetText(Teams[curTeam]:GetTotalSecuredVotes());</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0667}}<syntaxhighlight lang="lua">table.sort(sortedPlayerList, function(a, b) return Teams[Players[b]:GetTeam()]:GetTotalSecuredVotes() <</syntaxhighlight>
{{CodeLine5|0668}}<syntaxhighlight lang="lua">Teams[Players[a]:GetTeam()]:GetTotalSecuredVotes() end );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0735}}<syntaxhighlight lang="lua">controlTable.TotalVotes:SetText(Teams[pTeam]:GetTotalSecuredVotes());</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetTotalSecuredVotes]]
[[Category:Civ5 United Nations API|GetTotalSecuredVotes]]
[[Category:Civ5 Score API|GetTotalSecuredVotes]]