{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Game}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''void''' Game.SetVictoryValid<b>(</b>{{Type5|VictoryType}} arg0, '''bool''' arg1<b>)</b></code>


'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|arg0:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|arg1:
|valign="top"| ''No description available.''
|}


=Source code samples=
{{PseudoH4|TurnsRemaining.lua (G&K)}}
:<code>DLC/Expansion/Scenarios/MedievalScenario/TurnsRemaining.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1857}}<syntaxhighlight lang="lua">Game.SetVictoryValid(0,true);</syntaxhighlight>
{{CodeLine5|1858}}<syntaxhighlight lang="lua">Game.SetVictoryValid(1,false);</syntaxhighlight>
{{CodeLine5|1859}}<syntaxhighlight lang="lua">Game.SetVictoryValid(2,true);</syntaxhighlight>
{{CodeLine5|1860}}<syntaxhighlight lang="lua">Game.SetVictoryValid(3,false);</syntaxhighlight>
{{CodeLine5|1861}}<syntaxhighlight lang="lua">Game.SetVictoryValid(4,true);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TurnsRemaining.lua (G&K)}}
:<code>DLC/Expansion/Scenarios/SteampunkScenario/TurnsRemaining.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0123}}<syntaxhighlight lang="lua">Game.SetVictoryValid(GameInfo.Victories["VICTORY_TIME"].ID, true);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0865}}<syntaxhighlight lang="lua">Game.SetVictoryValid(GameInfo.Victories["VICTORY_TIME"].ID, false);</syntaxhighlight>
{{CodeLine5|0866}}<syntaxhighlight lang="lua">Game.SetVictoryValid(GameInfo.Victories["VICTORY_SPACE_RACE"].ID, false);</syntaxhighlight>
{{CodeLine5|0867}}<syntaxhighlight lang="lua">Game.SetVictoryValid(GameInfo.Victories["VICTORY_DOMINATION"].ID, false);</syntaxhighlight>
{{CodeLine5|0868}}<syntaxhighlight lang="lua">Game.SetVictoryValid(GameInfo.Victories["VICTORY_CULTURAL"].ID, false);</syntaxhighlight>
{{CodeLine5|0869}}<syntaxhighlight lang="lua">Game.SetVictoryValid(GameInfo.Victories["VICTORY_DIPLOMATIC"].ID, false);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|SetVictoryValid]]
[[Category:Civ5 Victory API|SetVictoryValid]]