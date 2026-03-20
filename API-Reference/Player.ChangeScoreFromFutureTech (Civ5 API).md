{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Player}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''void''' Player:ChangeScoreFromFutureTech<b>(</b>'''int''' vPReceived<b>)</b></code>


'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|vPReceived:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|TurnsRemaining.lua - DLC_02 DLC}}
:<code>DLC/DLC_02/Scenarios/NewWorldScenario/TurnsRemaining.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0217}}<syntaxhighlight lang="lua">player:ChangeScoreFromFutureTech(iVPReceived);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TurnsRemaining.lua (G&K)}}
:<code>DLC/Expansion/Scenarios/FallOfRomeScenario/TurnsRemaining.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0406}}<syntaxhighlight lang="lua">newPlayer:ChangeScoreFromFutureTech(pCity:GetPopulation() * 2 * 100);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TurnsRemaining.lua (G&K)}}
:<code>DLC/Expansion/Scenarios/MedievalScenario/TurnsRemaining.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1177}}<syntaxhighlight lang="lua">pPlayer:ChangeScoreFromFutureTech(10);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|VoteResultsPopup.lua (G&K)}}
:<code>DLC/Expansion/Scenarios/MedievalScenario/VoteResultsPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0297}}<syntaxhighlight lang="lua">Players[iBestVotePlayer]:ChangeScoreFromFutureTech(250);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|ChangeScoreFromFutureTech]]
[[Category:Civ5 Science API|ChangeScoreFromFutureTech]]
[[Category:Civ5 Score API|ChangeScoreFromFutureTech]]