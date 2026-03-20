{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Unit}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''int''' Unit:GetBaseCombatStrength<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|EnemyUnitPanel.lua}}
:<code>UI/InGame/WorldView/EnemyUnitPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0197}}<syntaxhighlight lang="lua">strength = pUnit:GetBaseCombatStrength();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1840}}<syntaxhighlight lang="lua">if (pUnit:GetBaseCombatStrength() > 0 or pHeadUnit:IsRanged()) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|MilitaryOverview.lua}}
:<code>UI/InGame/Popups/MilitaryOverview.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0250}}<syntaxhighlight lang="lua">sortEntry.strength = unit:GetBaseCombatStrength();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|PlotMouseoverInclude.lua}}
:<code>UI/InGame/PlotMouseoverInclude.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0266}}<syntaxhighlight lang="lua">strength = unit:GetBaseCombatStrength();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0299}}<syntaxhighlight lang="lua">strUnitText = strUnitText .. ", [ICON_STRENGTH]" .. unit:GetBaseCombatStrength();</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetBaseCombatStrength]]
[[Category:Civ5 Combat API|GetBaseCombatStrength]]