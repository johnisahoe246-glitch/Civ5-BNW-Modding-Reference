{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Plot}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''int''' Plot:GetNumUnits<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|EnemyUnitPanel.lua}}
:<code>UI/InGame/WorldView/EnemyUnitPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1826}}<syntaxhighlight lang="lua">local iNumUnits = pPlot:GetNumUnits();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1927}}<syntaxhighlight lang="lua">local numUnitsOnPlot = pPlot:GetNumUnits();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|InGame.lua}}
:<code>UI/InGame/InGame.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0179}}<syntaxhighlight lang="lua">local unitCount = plot:GetNumUnits();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|PlotMouseoverInclude.lua}}
:<code>UI/InGame/PlotMouseoverInclude.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0253}}<syntaxhighlight lang="lua">local numUnits = plot:GetNumUnits();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TurnsRemaining.lua (G&K)}}
:<code>DLC/Expansion/Scenarios/MedievalScenario/TurnsRemaining.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1073}}<syntaxhighlight lang="lua">local iNumUnits = startPlot:GetNumUnits();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|UnitFlagManager.lua}}
:<code>UI/InGame/UnitFlagManager.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0589}}<syntaxhighlight lang="lua">if( plot:GetNumUnits() > 1 )</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0591}}<syntaxhighlight lang="lua">for i = 0, plot:GetNumUnits() - 1, 1</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1023}}<syntaxhighlight lang="lua">local numUnits = pPlot:GetNumUnits();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1443}}<syntaxhighlight lang="lua">local count = pPlot:GetNumUnits();</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetNumUnits]]
[[Category:Civ5 Units API|GetNumUnits]]