{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Unit}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''int''' Unit:GetNumEnemyUnitsAdjacent<b>(</b>{{Type5|Unit}} otherUnit<b>)</b></code>


'''Returned Value'''
:No description available.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|otherUnit:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|EnemyUnitPanel.lua}}
:<code>UI/InGame/WorldView/EnemyUnitPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0806}}<syntaxhighlight lang="lua">local iNumAdjacentFriends = pTheirUnit:GetNumEnemyUnitsAdjacent(pMyUnit);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1183}}<syntaxhighlight lang="lua">iNumAdjacentFriends = pMyUnit:GetNumEnemyUnitsAdjacent(pTheirUnit);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TutorialChecks.lua}}
:<code>Tutorial/TutorialChecks.lua</code>
:{{CodeBegin5}}
{{CodeLine5|3048}}<syntaxhighlight lang="lua">if (v:GetNumEnemyUnitsAdjacent(v) > 0 or v:IsEnemyCityAdjacent()) then</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetNumEnemyUnitsAdjacent]]
[[Category:Civ5 Units API|GetNumEnemyUnitsAdjacent]]
[[Category:Civ5 Diplomacy API|GetNumEnemyUnitsAdjacent]]