{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|City}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''int''' City:RangeCombatUnitDefense<b>(</b>{{Type5|Unit}} theirUnit<b>)</b></code>


'''Returned Value'''
:No description available.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|theirUnit:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|EnemyUnitPanel.lua}}
:<code>UI/InGame/WorldView/EnemyUnitPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1421}}<syntaxhighlight lang="lua">local theirUnitStrength = myCity:RangeCombatUnitDefense(theirUnit);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|RangeCombatUnitDefense]]
[[Category:Civ5 Units API|RangeCombatUnitDefense]]
[[Category:Civ5 Combat API|RangeCombatUnitDefense]]