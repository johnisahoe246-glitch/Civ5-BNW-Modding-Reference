{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Plot}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''int''' Plot:IsVisible<b>(</b>{{Type5|TeamID}} team, '''bool''' debug<b>)</b></code>


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

{{PseudoH4|Bombardment.lua}}
:<code>UI/InGame/Bombardment.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0065}}<syntaxhighlight lang="lua">if pTargetPlot:IsVisible(thisTeam, false) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|EnemyUnitPanel.lua}}
:<code>UI/InGame/WorldView/EnemyUnitPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1824}}<syntaxhighlight lang="lua">if (pPlot:IsVisible(iTeam, false)) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1925}}<syntaxhighlight lang="lua">if (pPlot:IsVisible(myTeamID, false)) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|EnemyUnitPanel.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/WorldView/EnemyUnitPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|2072}}<syntaxhighlight lang="lua">if (pPlot:IsVisible(iTeam, false) and not pHeadUnit:IsCityAttackOnly()) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|InGame.lua}}
:<code>UI/InGame/InGame.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0236}}<syntaxhighlight lang="lua">if (plot:IsVisible(player:GetTeam(), false) and (plot:IsVisibleEnemyDefender(pUnit) or plot:IsEnemyCity(pUnit))) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|PlotHelpManager.lua}}
:<code>UI/InGame/PlotHelpManager.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0129}}<syntaxhighlight lang="lua">if (plot:IsVisible(iActiveTeam, bIsDebug)) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|UnitFlagManager.lua}}
:<code>UI/InGame/UnitFlagManager.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1411}}<syntaxhighlight lang="lua">if( plot:IsVisible( Game.GetActiveTeam() ) ) then</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|IsVisible]]
[[Category:Civ5 Fog API|IsVisible]]