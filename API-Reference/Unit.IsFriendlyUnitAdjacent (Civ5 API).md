{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Unit}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''bool''' Unit:IsFriendlyUnitAdjacent<b>(</b>'''bool''' combatUnit<b>)</b></code>


'''Returned Value'''
:No description available.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|combatUnit:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|EnemyUnitPanel.lua}}
:<code>UI/InGame/WorldView/EnemyUnitPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0875}}<syntaxhighlight lang="lua">if (pMyUnit:IsFriendlyUnitAdjacent(bCombatUnit)) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1128}}<syntaxhighlight lang="lua">if (pTheirUnit:IsFriendlyUnitAdjacent(bCombatUnit)) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1485}}<syntaxhighlight lang="lua">if (theirUnit:IsFriendlyUnitAdjacent(bCombatUnit)) then</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|IsFriendlyUnitAdjacent]]
[[Category:Civ5 Units API|IsFriendlyUnitAdjacent]]