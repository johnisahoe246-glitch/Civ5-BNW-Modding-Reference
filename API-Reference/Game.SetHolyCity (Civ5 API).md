{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Game}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''void''' Game.SetHolyCity<b>(</b>{{Type5|ReligionType}} arg0, {{Type5|City}} newHolyCity<b>)</b></code>


'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|arg0:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|newHolyCity:
|valign="top"| ''No description available.''
|}


=Source code samples=
{{PseudoH4|TurnsRemaining.lua (G&K)}}
:<code>DLC/Expansion/Scenarios/MedievalScenario/TurnsRemaining.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0212}}<syntaxhighlight lang="lua">Game.SetHolyCity (GameInfoTypes["RELIGION_ORTHODOXY"], pNewHolyCity);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|SetHolyCity]]
[[Category:Civ5 Cities API|SetHolyCity]]
[[Category:Civ5 Religion API|SetHolyCity]]