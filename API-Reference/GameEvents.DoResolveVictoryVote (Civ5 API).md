{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|GameEvents}}.<br/>
This is a static method, invoke it with a dot.
<br/>
*This method was added in Gods & Kings.
}}


=Usage=
<code>'''void''' GameEvents.DoResolveVictoryVote<b>(</b>'''bool''' preliminaryVote<b>)</b></code>


'''Event Type'''
:Unknown

'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|preliminaryVote:
|valign="top"| ''No description available.''
|}


=Source code samples=
{{PseudoH4|TurnsRemaining.lua (G&K)}}
:<code>DLC/Expansion/Scenarios/MedievalScenario/TurnsRemaining.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0391}}<syntaxhighlight lang="lua">GameEvents.DoResolveVictoryVote.Add(function(bPreliminaryVote)</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0394}}<syntaxhighlight lang="lua">-- Vatican City</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0396}}<syntaxhighlight lang="lua">local kiVaticanExtraVotes = 1;</syntaxhighlight>
{{CodeLine5|0397}}<syntaxhighlight lang="lua">local iTeam = GetVaticanExtraVoteRecipient();</syntaxhighlight>
{{CodeLine5|0398}}<syntaxhighlight lang="lua">if (iTeam ~= -1) then</syntaxhighlight>
{{CodeLine5|0399}}<syntaxhighlight lang="lua">SetPersistentProperty("VaticanExtraVoteTeam", iTeam); -- So VictoryProgress.lua can display the last team that got extra vote</syntaxhighlight>
{{CodeLine5|0400}}<syntaxhighlight lang="lua">Game.ChangeNumVotesForTeam(iTeam, kiVaticanExtraVotes);</syntaxhighlight>
{{CodeLine5|0401}}<syntaxhighlight lang="lua">end</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0403}}<syntaxhighlight lang="lua">return true;</syntaxhighlight>
{{CodeLine5|0404}}<syntaxhighlight lang="lua">end)</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0406}}<syntaxhighlight lang="lua">-- Get the team which receives the extra vote from Vatican City in a HRE election, or no team if there isn't one</syntaxhighlight>
{{CodeLine5|0407}}<syntaxhighlight lang="lua">function GetVaticanExtraVoteRecipient()</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|DoResolveVictoryVote]]
[[Category:Civ5 United Nations API|DoResolveVictoryVote]]
[[Category:Civ5 Victory API|DoResolveVictoryVote]]