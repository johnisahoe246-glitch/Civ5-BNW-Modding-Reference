{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Plot}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''void''' Plot:SetRevealed<b>(</b>{{Type5|TeamID}} team, '''bool''' newValue, '''bool''' terrainOnly, {{Type5|TeamID}} fromTeam<b>)</b></code>


'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|team:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|newValue:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|terrainOnly:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|fromTeam:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|InGame.lua}}
:<code>UI/InGame/InGame.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0094}}<syntaxhighlight lang="lua">pPlot:SetRevealed(team, false);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0097}}<syntaxhighlight lang="lua">pPlot:SetRevealed(team, bIsDebug);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TurnsRemaining.lua (G&K)}}
:<code>DLC/Expansion/Scenarios/MedievalScenario/TurnsRemaining.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1038}}<syntaxhighlight lang="lua">pPlot:SetRevealed(iTeam, true);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1044}}<syntaxhighlight lang="lua">adjPlot:SetRevealed(iTeam, true);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|SetRevealed]]
[[Category:Civ5 Fog API|SetRevealed]]