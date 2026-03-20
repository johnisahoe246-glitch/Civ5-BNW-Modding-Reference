{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Game}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>{{Type5|PlayerID}} Game.GetFounder<b>(</b>{{Type5|ReligionType}} arg0, '''int''' arg1<b>)</b></code>


'''Returned Value'''
:No description available.
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
{{CodeLine5|1176}}<syntaxhighlight lang="lua">if (Game.GetFounder(GameInfoTypes["RELIGION_ORTHODOXY"], -1) == iPlayerLoop) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1186}}<syntaxhighlight lang="lua">if (Game.GetFounder(GameInfoTypes["RELIGION_ISLAM"], -1) == iPlayerLoop) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1201}}<syntaxhighlight lang="lua">if (Game.GetFounder(GameInfoTypes["RELIGION_CHRISTIANITY"], -1) == iPlayerLoop) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1216}}<syntaxhighlight lang="lua">if (Game.GetFounder(GameInfoTypes["RELIGION_PROTESTANTISM"], -1) == iPlayerLoop) then</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetFounder]]
[[Category:Civ5 Religion API|GetFounder]]