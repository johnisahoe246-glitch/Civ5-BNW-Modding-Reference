{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Unit}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''int''' Unit:IsHigherTechThan<b>(</b>{{Type5|UnitType}} arg0<b>)</b></code>


'''Returned Value'''
:No description available.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|arg0:
|valign="top"| ''No description available.''
|}


=Source code samples=
{{PseudoH4|EnemyUnitPanel.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/WorldView/EnemyUnitPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0907}}<syntaxhighlight lang="lua">if (iModifier ~= 0 and pTheirUnit:IsHigherTechThan(pMyUnit:GetUnitType())) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1456}}<syntaxhighlight lang="lua">if (iModifier ~= 0 and pMyUnit:IsHigherTechThan(pTheirUnit:GetUnitType())) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1798}}<syntaxhighlight lang="lua">if (iModifier ~= 0 and pMyUnit:IsHigherTechThan(theirUnit:GetUnitType())) then</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|IsHigherTechThan]]
[[Category:Civ5 Science API|IsHigherTechThan]]
[[Category:Civ5 Diplomacy API|IsHigherTechThan]]