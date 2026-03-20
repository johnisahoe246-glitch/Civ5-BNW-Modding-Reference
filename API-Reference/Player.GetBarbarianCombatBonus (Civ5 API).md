{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Player}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''int''' Player:GetBarbarianCombatBonus<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|EnemyUnitPanel.lua}}
:<code>UI/InGame/WorldView/EnemyUnitPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1055}}<syntaxhighlight lang="lua">iModifier = iModifier + Players[pMyUnit:GetOwner()]:GetBarbarianCombatBonus();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1628}}<syntaxhighlight lang="lua">iModifier = iModifier + myPlayer:GetBarbarianCombatBonus();</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetBarbarianCombatBonus]]
[[Category:Civ5 Combat API|GetBarbarianCombatBonus]]
[[Category:Civ5 Barbarians API|GetBarbarianCombatBonus]]