{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Plot}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''int''' Plot:DefenseModifier<b>(</b>{{Type5|TeamID}} defendTeam, '''bool''' ignoreBuilding, '''bool''' help<b>)</b></code>


'''Returned Value'''
:No description available.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|defendTeam:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|ignoreBuilding:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|help:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|EnemyUnitPanel.lua}}
:<code>UI/InGame/WorldView/EnemyUnitPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1136}}<syntaxhighlight lang="lua">iModifier = pToPlot:DefenseModifier(pTheirUnit:GetTeam(), false, false);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1493}}<syntaxhighlight lang="lua">iModifier = theirPlot:DefenseModifier(theirUnit:GetTeam(), false, false);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|DefenseModifier]]
[[Category:Civ5 Combat API|DefenseModifier]]