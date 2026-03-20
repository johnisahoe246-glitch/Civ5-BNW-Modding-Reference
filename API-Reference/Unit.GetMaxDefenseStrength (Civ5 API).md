{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Unit}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''int''' Unit:GetMaxDefenseStrength<b>(</b>{{Type5|Plot}} inPlot, {{Type5|Unit}} attacker, '''bool''' arg2 = nil<b>)</b></code>


'''Returned Value'''
:No description available.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|inPlot:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|attacker:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|arg2:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|EnemyUnitPanel.lua}}
:<code>UI/InGame/WorldView/EnemyUnitPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0603}}<syntaxhighlight lang="lua">iTheirStrength = pTheirUnit:GetMaxDefenseStrength(pToPlot, pMyUnit, true);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0609}}<syntaxhighlight lang="lua">iTheirStrength = pTheirUnit:GetMaxDefenseStrength(pToPlot, pMyUnit);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetMaxDefenseStrength]]
[[Category:Civ5 Combat API|GetMaxDefenseStrength]]