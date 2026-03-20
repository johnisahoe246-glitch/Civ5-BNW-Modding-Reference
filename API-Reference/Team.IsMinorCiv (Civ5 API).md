{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Team}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''int''' Team:IsMinorCiv<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|DeclareWarMovePopup.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/PopupsGeneric/DeclareWarMovePopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0015}}<syntaxhighlight lang="lua">if (plot:GetTeam() == eRivalTeam and (not Teams[eRivalTeam]:IsMinorCiv() or plot:IsCity())) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0034}}<syntaxhighlight lang="lua">if (not Teams[eRivalTeam]:IsMinorCiv()) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0073}}<syntaxhighlight lang="lua">if (not Teams[eRivalTeam]:IsMinorCiv() and not Teams[eRivalTeam]:IsHuman()) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DeclareWarRangeStrikePopup.lua}}
:<code>UI/InGame/PopupsGeneric/DeclareWarRangeStrikePopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0011}}<syntaxhighlight lang="lua">if (not rivalTeam:IsMinorCiv()) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0049}}<syntaxhighlight lang="lua">if (not rivalTeam:IsMinorCiv() and not rivalTeam:IsHuman()) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|VictoryProgress.lua}}
:<code>UI/InGame/Popups/VictoryProgress.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0719}}<syntaxhighlight lang="lua">elseif(v:IsMinorCiv()) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|VoteResultsPopup.lua}}
:<code>UI/InGame/Popups/VoteResultsPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0034}}<syntaxhighlight lang="lua">if (not pTeam:IsMinorCiv()) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0052}}<syntaxhighlight lang="lua">if(not pTeam:IsMinorCiv()) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0070}}<syntaxhighlight lang="lua">if(not g_bIsTeamGame or pTeam:IsMinorCiv()) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0110}}<syntaxhighlight lang="lua">if (pTeam:IsMinorCiv() and iTeam == iVoteCast) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0223}}<syntaxhighlight lang="lua">if (pLoopTeam:IsMinorCiv()) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|VoteResultsPopup.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/Popups/VoteResultsPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0130}}<syntaxhighlight lang="lua">if (pTeam:IsMinorCiv()) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0194}}<syntaxhighlight lang="lua">if (iVotes == 0 and pTeam:IsMinorCiv()) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0276}}<syntaxhighlight lang="lua">if (Teams[a[1]]:IsMinorCiv()) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0279}}<syntaxhighlight lang="lua">if (Teams[b[1]]:IsMinorCiv()) then</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|IsMinorCiv]]
[[Category:Civ5 City States API|IsMinorCiv]]