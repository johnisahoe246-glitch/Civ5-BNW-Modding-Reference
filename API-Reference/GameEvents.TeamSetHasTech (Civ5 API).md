{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|GameEvents}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''void''' GameEvents.TeamSetHasTech<b>(</b>{{Type5|TeamID}} team, {{Type5|TechType}} tech, '''bool''' adopted<b>)</b></code>


'''Event Type'''
:Unknown

'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|team:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|tech:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|adopted:
|valign="top"| ''No description available.''
|}


=Source code samples=
{{PseudoH4|TurnsRemaining.lua (G&K)}}
:<code>DLC/Expansion/Scenarios/MedievalScenario/TurnsRemaining.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0699}}<syntaxhighlight lang="lua">GameEvents.TeamSetHasTech.Add(function(iTeam, iTech, bAdopted)</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0701}}<syntaxhighlight lang="lua">local iTurn = Game.GetGameTurn();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0703}}<syntaxhighlight lang="lua">-- Humanism adopted?</syntaxhighlight>
{{CodeLine5|0704}}<syntaxhighlight lang="lua">if (iTech == GameInfoTypes["TECH_ACOUSTICS"] and GetPersistentProperty("ReformationStart") == -1) then</syntaxhighlight>
{{CodeLine5|0705}}<syntaxhighlight lang="lua">SetPersistentProperty("ReformationStart", iTurn + 3);</syntaxhighlight>
{{CodeLine5|0706}}<syntaxhighlight lang="lua">SetPersistentProperty("SecondReformer", iTurn + 6);</syntaxhighlight>
{{CodeLine5|0707}}<syntaxhighlight lang="lua">SetPersistentProperty("ThirdReformer", iTurn + 9);</syntaxhighlight>
{{CodeLine5|0708}}<syntaxhighlight lang="lua">end</syntaxhighlight>
{{CodeLine5|0709}}<syntaxhighlight lang="lua">end);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|TeamSetHasTech]]
[[Category:Civ5 Science API|TeamSetHasTech]]
[[Category:Civ5 Diplomacy API|TeamSetHasTech]]