{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Player}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''int''' Player:GetTraitGreatGeneralExtraBonus<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|EnemyUnitPanel.lua}}
:<code>UI/InGame/WorldView/EnemyUnitPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0773}}<syntaxhighlight lang="lua">iModifier = iModifier + pMyPlayer:GetTraitGreatGeneralExtraBonus();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1159}}<syntaxhighlight lang="lua">iModifier = iModifier + pTheirPlayer:GetTraitGreatGeneralExtraBonus();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1514}}<syntaxhighlight lang="lua">iModifier = iModifier + theirPlayer:GetTraitGreatGeneralExtraBonus();</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetTraitGreatGeneralExtraBonus]]
[[Category:Civ5 Great People API|GetTraitGreatGeneralExtraBonus]]