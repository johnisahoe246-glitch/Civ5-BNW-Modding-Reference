{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Player}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>{{Type5|City}} Player:InitCity<b>(</b>'''int''' x, '''int''' y, '''bool''' bumpUnits = true<b>)</b></code>


'''Returned Value'''
:No description available.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|x:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|y:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|bumpUnits:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|TurnsRemaining.lua (G&K)}}
:<code>DLC/Expansion/Scenarios/MedievalScenario/TurnsRemaining.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1070}}<syntaxhighlight lang="lua">local capital = pPlayer:InitCity(startPlot:GetX(), startPlot:GetY());</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1125}}<syntaxhighlight lang="lua">local cityState = pPlayer:InitCity(startPlot:GetX(), startPlot:GetY());</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1239}}<syntaxhighlight lang="lua">local capital = pPlayer:InitCity(start_plot:GetX(), start_plot:GetY());</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|WorldView.lua}}
:<code>UI/InGame/WorldView/WorldView.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0229}}<syntaxhighlight lang="lua">player:InitCity(plot:GetX(), plot:GetY());</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0260}}<syntaxhighlight lang="lua">pActivePlayer:InitCity(plotX, plotY);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|InitCity]]
[[Category:Civ5 Cities API|InitCity]]