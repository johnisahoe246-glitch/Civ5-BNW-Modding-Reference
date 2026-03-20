{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Unit}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''int''' Unit:GetRangeCombatDamage<b>(</b>{{Type5|Unit}} defender, {{Type5|City}} city, '''bool''' includeRand<b>)</b></code>


'''Returned Value'''
:No description available.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|defender:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|city:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|includeRand:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|EnemyUnitPanel.lua}}
:<code>UI/InGame/WorldView/EnemyUnitPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0323}}<syntaxhighlight lang="lua">iMyDamageInflicted = pMyUnit:GetRangeCombatDamage(nil, pCity, false);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0329}}<syntaxhighlight lang="lua">iTheirFireSupportCombatDamage = pFireSupportUnit:GetRangeCombatDamage(pMyUnit, nil, false);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0599}}<syntaxhighlight lang="lua">iMyDamageInflicted = pMyUnit:GetRangeCombatDamage(pTheirUnit, nil, false);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetRangeCombatDamage]]
[[Category:Civ5 Combat API|GetRangeCombatDamage]]