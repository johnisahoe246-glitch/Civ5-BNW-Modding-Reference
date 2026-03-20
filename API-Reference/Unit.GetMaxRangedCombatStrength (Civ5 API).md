{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Unit}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''int''' Unit:GetMaxRangedCombatStrength<b>(</b>{{Type5|Unit}} other, '''int''' attacking, '''bool''' arg2, '''bool''' arg3<b>)</b></code>


'''Returned Value'''
:No description available.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|other:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|attacking:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|arg2:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|arg3:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|EnemyUnitPanel.lua}}
:<code>UI/InGame/WorldView/EnemyUnitPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0302}}<syntaxhighlight lang="lua">iMyStrength = pMyUnit:GetMaxRangedCombatStrength(nil, pCity, true, true);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0581}}<syntaxhighlight lang="lua">iMyStrength = pMyUnit:GetMaxRangedCombatStrength(pTheirUnit, nil, true, true);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0600}}<syntaxhighlight lang="lua">iTheirStrength = pTheirUnit:GetMaxRangedCombatStrength(pMyUnit, nil, false, true);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetMaxRangedCombatStrength]]
[[Category:Civ5 Combat API|GetMaxRangedCombatStrength]]