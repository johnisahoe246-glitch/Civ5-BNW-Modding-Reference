{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Modding}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>{{Type5|Slider}} Modding.OpenSaveData<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|ReligionOverview.lua (G&K)}}
:<code>DLC/Expansion/Scenarios/MedievalScenario/ReligionOverview.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0157}}<syntaxhighlight lang="lua">local savedData = Modding.OpenSaveData();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TurnsRemaining.lua (G&K)}}
:<code>DLC/Expansion/Scenarios/MedievalScenario/TurnsRemaining.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0013}}<syntaxhighlight lang="lua">g_SaveData = Modding.OpenSaveData();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|VictoryProgress.lua (G&K)}}
:<code>DLC/Expansion/Scenarios/MedievalScenario/VictoryProgress.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0007}}<syntaxhighlight lang="lua">local g_savedData = Modding.OpenSaveData();</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|OpenSaveData]]