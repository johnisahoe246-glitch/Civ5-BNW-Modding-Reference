{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Plot}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''int''' Plot:IsVisibleEnemyUnit<b>(</b>{{Type5|PlayerID}} player<b>)</b></code>


'''Returned Value'''
:No description available.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|player:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|CityView.lua}}
:<code>UI/InGame/CityView/CityView.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1793}}<syntaxhighlight lang="lua">elseif ( plot:IsVisibleEnemyUnit(pCity:GetOwner()) ) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TutorialChecks.lua}}
:<code>Tutorial/TutorialChecks.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1438}}<syntaxhighlight lang="lua">if (not pTargetPlot:IsWater() and pTargetPlot:IsVisibleEnemyUnit(player:GetID())) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|WorldView.lua}}
:<code>UI/InGame/WorldView/WorldView.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0618}}<syntaxhighlight lang="lua">if (plot:IsVisibleEnemyUnit(pHeadSelectedUnit:GetOwner()) or plot:IsEnemyCity(pHeadSelectedUnit)) then</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|IsVisibleEnemyUnit]]
[[Category:Civ5 Fog API|IsVisibleEnemyUnit]]
[[Category:Civ5 Units API|IsVisibleEnemyUnit]]
[[Category:Civ5 Diplomacy API|IsVisibleEnemyUnit]]