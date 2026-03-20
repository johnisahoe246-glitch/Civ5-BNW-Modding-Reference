{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Player}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''int''' Player:GetTraitGoldenAgeCombatModifier<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|EnemyUnitPanel.lua}}
:<code>UI/InGame/WorldView/EnemyUnitPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1065}}<syntaxhighlight lang="lua">iModifier = pMyPlayer:GetTraitGoldenAgeCombatModifier();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1386}}<syntaxhighlight lang="lua">iModifier = pTheirPlayer:GetTraitGoldenAgeCombatModifier();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1647}}<syntaxhighlight lang="lua">iModifier = theirPlayer:GetTraitGoldenAgeCombatModifier();</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetTraitGoldenAgeCombatModifier]]
[[Category:Civ5 Golden Age API|GetTraitGoldenAgeCombatModifier]]
[[Category:Civ5 Combat API|GetTraitGoldenAgeCombatModifier]]