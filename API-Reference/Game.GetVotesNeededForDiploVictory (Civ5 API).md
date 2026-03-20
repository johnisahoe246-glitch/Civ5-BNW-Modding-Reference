{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Game}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''int''' Game.GetVotesNeededForDiploVictory<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|VictoryProgress.lua}}
:<code>UI/InGame/Popups/VictoryProgress.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0421}}<syntaxhighlight lang="lua">Controls.VotesNeeded:SetText(Game.GetVotesNeededForDiploVictory());</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0743}}<syntaxhighlight lang="lua">Controls.NeededVotes:SetText(Locale.ConvertTextKey("TXT_KEY_VP_DIPLO_VOTES_NEEDED").." "..Game.GetVotesNeededForDiploVictory());</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|VoteResultsPopup.lua}}
:<code>UI/InGame/Popups/VoteResultsPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0194}}<syntaxhighlight lang="lua">local iVotesToWin = Game.GetVotesNeededForDiploVictory();</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetVotesNeededForDiploVictory]]
[[Category:Civ5 Diplomacy API|GetVotesNeededForDiploVictory]]
[[Category:Civ5 United Nations API|GetVotesNeededForDiploVictory]]
[[Category:Civ5 Victory API|GetVotesNeededForDiploVictory]]