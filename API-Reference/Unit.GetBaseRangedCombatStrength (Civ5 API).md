{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Unit}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''int''' Unit:GetBaseRangedCombatStrength<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|EnemyUnitPanel.lua}}
:<code>UI/InGame/WorldView/EnemyUnitPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0195}}<syntaxhighlight lang="lua">strength = pUnit:GetBaseRangedCombatStrength();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0210}}<syntaxhighlight lang="lua">iRangedStrength = pUnit:GetBaseRangedCombatStrength();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0580}}<syntaxhighlight lang="lua">if (pMyUnit:GetBaseRangedCombatStrength() > 0) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|MilitaryOverview.lua}}
:<code>UI/InGame/Popups/MilitaryOverview.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0257}}<syntaxhighlight lang="lua">sortEntry.ranged = unit:GetBaseRangedCombatStrength();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|UnitPanel.lua}}
:<code>UI/InGame/WorldView/UnitPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0617}}<syntaxhighlight lang="lua">strength = unit:GetBaseRangedCombatStrength();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0632}}<syntaxhighlight lang="lua">iRangedStrength = unit:GetBaseRangedCombatStrength();</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetBaseRangedCombatStrength]]
[[Category:Civ5 Combat API|GetBaseRangedCombatStrength]]