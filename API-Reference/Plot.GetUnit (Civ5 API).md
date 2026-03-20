{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Plot}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>{{Type5|Unit}} Plot:GetUnit<b>(</b>{{Type5|UnitID}} id<b>)</b></code>


'''Returned Value'''
:No description available.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|id:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|EnemyUnitPanel.lua}}
:<code>UI/InGame/WorldView/EnemyUnitPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1831}}<syntaxhighlight lang="lua">pUnit = pPlot:GetUnit(i);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1933}}<syntaxhighlight lang="lua">local theirUnit = pPlot:GetUnit(i);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|InGame.lua}}
:<code>UI/InGame/InGame.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0183}}<syntaxhighlight lang="lua">local pFoundUnit = plot:GetUnit(i);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|PlotMouseoverInclude.lua}}
:<code>UI/InGame/PlotMouseoverInclude.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0256}}<syntaxhighlight lang="lua">local unit = plot:GetUnit(i);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TurnsRemaining.lua - DLC_04 DLC}}
:<code>DLC/DLC_04/Scenarios/1066Scenario/TurnsRemaining.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0470}}<syntaxhighlight lang="lua">pPlot:GetUnit(0):Kill(true, -1);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0749}}<syntaxhighlight lang="lua">Map.GetPlot(42,39):GetUnit(0):SetDeployFromOperationTurn(1);</syntaxhighlight>
{{CodeLine5|0750}}<syntaxhighlight lang="lua">Map.GetPlot(43,39):GetUnit(0):SetDeployFromOperationTurn(1);</syntaxhighlight>
{{CodeLine5|0751}}<syntaxhighlight lang="lua">Map.GetPlot(42,38):GetUnit(0):SetDeployFromOperationTurn(1);</syntaxhighlight>
{{CodeLine5|0752}}<syntaxhighlight lang="lua">Map.GetPlot(43,38):GetUnit(0):SetDeployFromOperationTurn(1);</syntaxhighlight>
{{CodeLine5|0753}}<syntaxhighlight lang="lua">Map.GetPlot(44,38):GetUnit(0):SetDeployFromOperationTurn(1);</syntaxhighlight>
{{CodeLine5|0754}}<syntaxhighlight lang="lua">Map.GetPlot(42,37):GetUnit(0):SetDeployFromOperationTurn(1);</syntaxhighlight>
{{CodeLine5|0755}}<syntaxhighlight lang="lua">Map.GetPlot(43,37):GetUnit(0):SetDeployFromOperationTurn(1);</syntaxhighlight>
{{CodeLine5|0756}}<syntaxhighlight lang="lua">Map.GetPlot(44,37):GetUnit(0):SetDeployFromOperationTurn(1);</syntaxhighlight>
{{CodeLine5|0757}}<syntaxhighlight lang="lua">Map.GetPlot(45,37):GetUnit(0):SetDeployFromOperationTurn(1);</syntaxhighlight>
{{CodeLine5|0758}}<syntaxhighlight lang="lua">Map.GetPlot(43,36):GetUnit(0):SetDeployFromOperationTurn(1);</syntaxhighlight>
{{CodeLine5|0759}}<syntaxhighlight lang="lua">Map.GetPlot(44,36):GetUnit(0):SetDeployFromOperationTurn(1);</syntaxhighlight>
{{CodeLine5|0760}}<syntaxhighlight lang="lua">Map.GetPlot(45,36):GetUnit(0):SetDeployFromOperationTurn(1);</syntaxhighlight>
{{CodeLine5|0761}}<syntaxhighlight lang="lua">Map.GetPlot(43,35):GetUnit(0):SetDeployFromOperationTurn(1);</syntaxhighlight>
{{CodeLine5|0762}}<syntaxhighlight lang="lua">Map.GetPlot(44,35):GetUnit(0):SetDeployFromOperationTurn(1);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TurnsRemaining.lua (G&K)}}
:<code>DLC/Expansion/Scenarios/FallOfRomeScenario/TurnsRemaining.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1043}}<syntaxhighlight lang="lua">pPlot:GetUnit(0):Kill(false, -1);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TurnsRemaining.lua (G&K)}}
:<code>DLC/Expansion/Scenarios/MedievalScenario/TurnsRemaining.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1076}}<syntaxhighlight lang="lua">pUnit = startPlot:GetUnit(i);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1390}}<syntaxhighlight lang="lua">elseif (plot:GetUnit(0) ~= nil) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1402}}<syntaxhighlight lang="lua">elseif (adjPlot:GetUnit(0) ~= nil) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|UnitFlagManager.lua}}
:<code>UI/InGame/UnitFlagManager.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0595}}<syntaxhighlight lang="lua">local test = plot:GetUnit( i );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1027}}<syntaxhighlight lang="lua">local pPlotUnit = pPlot:GetUnit( i );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1261}}<syntaxhighlight lang="lua">local unit = plot:GetUnit( i );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1445}}<syntaxhighlight lang="lua">local pUnit = pPlot:GetUnit( i );</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetUnit]]
[[Category:Civ5 Units API|GetUnit]]