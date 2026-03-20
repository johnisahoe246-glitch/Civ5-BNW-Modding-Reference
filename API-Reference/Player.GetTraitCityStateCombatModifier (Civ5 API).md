{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Player}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''int''' Player:GetTraitCityStateCombatModifier<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|EnemyUnitPanel.lua}}
:<code>UI/InGame/WorldView/EnemyUnitPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1072}}<syntaxhighlight lang="lua">iModifier = pMyPlayer:GetTraitCityStateCombatModifier();</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetTraitCityStateCombatModifier]]
[[Category:Civ5 Cities API|GetTraitCityStateCombatModifier]]
[[Category:Civ5 Combat API|GetTraitCityStateCombatModifier]]