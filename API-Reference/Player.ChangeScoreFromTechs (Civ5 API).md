{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Player}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''void''' Player:ChangeScoreFromTechs<b>(</b>'''int''' score<b>)</b></code>


'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|score:
|valign="top"| ''No description available.''
|}


=Source code samples=
{{PseudoH4|TurnsRemaining.lua (G&K)}}
:<code>DLC/Expansion/Scenarios/FallOfRomeScenario/TurnsRemaining.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0305}}<syntaxhighlight lang="lua">pPlayer:ChangeScoreFromTechs(iScore);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|ChangeScoreFromTechs]]
[[Category:Civ5 Science API|ChangeScoreFromTechs]]
[[Category:Civ5 Score API|ChangeScoreFromTechs]]