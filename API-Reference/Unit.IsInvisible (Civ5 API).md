{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Unit}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''bool''' Unit:IsInvisible<b>(</b>{{Type5|TeamID}} team, '''bool''' debug, '''bool''' checkCargo = false<b>)</b></code>


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
|-
|valign="top" style="padding-right:6px;"|checkCargo:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|EnemyUnitPanel.lua}}
:<code>UI/InGame/WorldView/EnemyUnitPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1832}}<syntaxhighlight lang="lua">if (pUnit ~= nil and not pUnit:IsInvisible(iTeam, false)) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1936}}<syntaxhighlight lang="lua">if (theirUnit ~= nil and not theirUnit:IsInvisible(myTeamID, false)) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|PlotMouseoverInclude.lua}}
:<code>UI/InGame/PlotMouseoverInclude.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0257}}<syntaxhighlight lang="lua">if (unit ~= nil and not unit:IsInvisible(iActiveTeam, bIsDebug)) then</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|IsInvisible]]
[[Category:Civ5 Fog API|IsInvisible]]