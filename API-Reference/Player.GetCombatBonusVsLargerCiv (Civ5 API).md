{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Player}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''int''' Player:GetCombatBonusVsLargerCiv<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
{{PseudoH4|EnemyUnitPanel.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/WorldView/EnemyUnitPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0915}}<syntaxhighlight lang="lua">iModifier = pMyPlayer:GetCombatBonusVsLargerCiv();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1464}}<syntaxhighlight lang="lua">iModifier = pTheirPlayer:GetCombatBonusVsLargerCiv();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1806}}<syntaxhighlight lang="lua">iModifier = theirPlayer:GetCombatBonusVsLargerCiv();</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetCombatBonusVsLargerCiv]]
[[Category:Civ5 Combat API|GetCombatBonusVsLargerCiv]]