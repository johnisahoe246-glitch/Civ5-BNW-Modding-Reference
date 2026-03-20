{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Unit}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''int''' Unit:FeatureDefenseModifier<b>(</b>{{Type5|FeatureType}} feature<b>)</b></code>


'''Returned Value'''
:No description available.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|feature:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|EnemyUnitPanel.lua}}
:<code>UI/InGame/WorldView/EnemyUnitPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1323}}<syntaxhighlight lang="lua">iModifier = pTheirUnit:FeatureDefenseModifier(pToPlot:GetFeatureType());</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1595}}<syntaxhighlight lang="lua">iModifier = theirUnit:FeatureDefenseModifier(theirPlot:GetFeatureType());</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|FeatureDefenseModifier]]
[[Category:Civ5 Features & Natural wonders API|FeatureDefenseModifier]]
[[Category:Civ5 Combat API|FeatureDefenseModifier]]