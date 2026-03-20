{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Game}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>{{Type5|CombatPredictionType}} Game.GetCombatPrediction<b>(</b>{{Type5|Unit}} myUnit, {{Type5|Unit}} theirUnit<b>)</b></code>


'''Returned Value'''
:No description available.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|myUnit:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|theirUnit:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|EnemyUnitPanel.lua}}
:<code>UI/InGame/WorldView/EnemyUnitPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0681}}<syntaxhighlight lang="lua">local eCombatPrediction = Game.GetCombatPrediction(pMyUnit, pTheirUnit);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetCombatPrediction]]
[[Category:Civ5 Combat API|GetCombatPrediction]]