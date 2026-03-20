{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Player}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''int''' Player:IsEmpireVeryUnhappy<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|CityView.lua}}
:<code>UI/InGame/CityView/CityView.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1576}}<syntaxhighlight lang="lua">if (pPlayer:IsEmpireVeryUnhappy()) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|EnemyUnitPanel.lua}}
:<code>UI/InGame/WorldView/EnemyUnitPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0856}}<syntaxhighlight lang="lua">if (pMyPlayer:IsEmpireVeryUnhappy()) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1109}}<syntaxhighlight lang="lua">if (pTheirPlayer:IsEmpireVeryUnhappy()) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1466}}<syntaxhighlight lang="lua">if (theirPlayer:IsEmpireVeryUnhappy()) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ProductionPopup.lua}}
:<code>UI/InGame/Popups/ProductionPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0639}}<syntaxhighlight lang="lua">if (player:IsEmpireVeryUnhappy()) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TopPanel.lua}}
:<code>UI/InGame/TopPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0095}}<syntaxhighlight lang="lua">elseif (pPlayer:IsEmpireVeryUnhappy()) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|UnitPanel.lua}}
:<code>UI/InGame/WorldView/UnitPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1175}}<syntaxhighlight lang="lua">if (action.Type == "MISSION_FOUND" and pActivePlayer:IsEmpireVeryUnhappy()) then</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|IsEmpireVeryUnhappy]]
[[Category:Civ5 Happiness API|IsEmpireVeryUnhappy]]