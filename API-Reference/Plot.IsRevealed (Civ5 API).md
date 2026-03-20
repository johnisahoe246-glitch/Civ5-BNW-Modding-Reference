{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Plot}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''int''' Plot:IsRevealed<b>(</b>{{Type5|TeamID}} team, '''bool''' debug<b>)</b></code>


'''Returned Value'''
:No description available.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|team:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|debug:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|EnemyUnitPanel.lua}}
:<code>UI/InGame/WorldView/EnemyUnitPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1802}}<syntaxhighlight lang="lua">if (pPlot:IsRevealed(iTeam, false)) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|InGame.lua}}
:<code>UI/InGame/InGame.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0461}}<syntaxhighlight lang="lua">if evalPlot:IsRevealed(unitTeam, false) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|PathHelpManager.lua}}
:<code>UI/InGame/WorldView/PathHelpManager.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0039}}<syntaxhighlight lang="lua">if( plot:IsRevealed( Game.GetActiveTeam(), false ) ) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|PlotHelpManager.lua}}
:<code>UI/InGame/PlotHelpManager.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0124}}<syntaxhighlight lang="lua">if (plot and plot:IsRevealed(iActiveTeam, bIsDebug)) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ResourceIconManager.lua}}
:<code>UI/InGame/ResourceIconManager.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0084}}<syntaxhighlight lang="lua">if( plot:IsRevealed( pPlayer:GetTeam(), false ) ) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0104}}<syntaxhighlight lang="lua">if( not plot:IsRevealed( Game.GetActiveTeam(), false ) ) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TurnsRemaining.lua - DLC_02 DLC}}
:<code>DLC/DLC_02/Scenarios/NewWorldScenario/TurnsRemaining.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0554}}<syntaxhighlight lang="lua">if (pPlot:IsRevealed(pTeam:GetID())) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TutorialChecks.lua}}
:<code>Tutorial/TutorialChecks.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1076}}<syntaxhighlight lang="lua">if (pCapitalCityPlot:IsRevealed(player:GetTeam())) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1084}}<syntaxhighlight lang="lua">if (pUnitPlot:IsRevealed(player:GetTeam())) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|2526}}<syntaxhighlight lang="lua">if (pPlot:IsRevealed(pPlayer:GetTeam())) then</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|IsRevealed]]
[[Category:Civ5 Fog API|IsRevealed]]