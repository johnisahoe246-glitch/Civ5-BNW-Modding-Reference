{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Unit}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''int''' Unit:IsStackedGreatGeneral<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|EnemyUnitPanel.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/WorldView/EnemyUnitPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0819}}<syntaxhighlight lang="lua">if (pMyUnit:GetGreatGeneralCombatModifier() ~= 0 and pMyUnit:IsStackedGreatGeneral()) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1276}}<syntaxhighlight lang="lua">if (pTheirUnit:GetGreatGeneralCombatModifier() ~= 0 and pTheirUnit:IsStackedGreatGeneral()) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1701}}<syntaxhighlight lang="lua">if (theirUnit:GetGreatGeneralCombatModifier() ~= 0 and theirUnit:IsStackedGreatGeneral()) then</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|IsStackedGreatGeneral]]
[[Category:Civ5 Great People API|IsStackedGreatGeneral]]