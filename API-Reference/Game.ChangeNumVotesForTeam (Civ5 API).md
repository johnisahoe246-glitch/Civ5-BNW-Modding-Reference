{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Game}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''void''' Game.ChangeNumVotesForTeam<b>(</b>{{Type5|TeamID}} team, '''int''' kiVaticanExtraVotes<b>)</b></code>


'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|team:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|kiVaticanExtraVotes:
|valign="top"| ''No description available.''
|}


=Source code samples=
{{PseudoH4|TurnsRemaining.lua (G&K)}}
:<code>DLC/Expansion/Scenarios/MedievalScenario/TurnsRemaining.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0400}}<syntaxhighlight lang="lua">Game.ChangeNumVotesForTeam(iTeam, kiVaticanExtraVotes);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|ChangeNumVotesForTeam]]
[[Category:Civ5 Diplomacy API|ChangeNumVotesForTeam]]
[[Category:Civ5 United Nations API|ChangeNumVotesForTeam]]