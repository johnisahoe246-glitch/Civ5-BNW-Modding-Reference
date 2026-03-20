{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Player}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''int''' Player:GetCombatBonusVsHigherTech<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
{{PseudoH4|EnemyUnitPanel.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/WorldView/EnemyUnitPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0905}}<syntaxhighlight lang="lua">iModifier = pMyPlayer:GetCombatBonusVsHigherTech();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1454}}<syntaxhighlight lang="lua">iModifier = pTheirPlayer:GetCombatBonusVsHigherTech();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1796}}<syntaxhighlight lang="lua">iModifier = theirPlayer:GetCombatBonusVsHigherTech();</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetCombatBonusVsHigherTech]]
[[Category:Civ5 Science API|GetCombatBonusVsHigherTech]]
[[Category:Civ5 Combat API|GetCombatBonusVsHigherTech]]
[[Category:Civ5 Diplomacy API|GetCombatBonusVsHigherTech]]