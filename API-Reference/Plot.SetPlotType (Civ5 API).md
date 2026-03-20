{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Plot}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''void''' Plot:SetPlotType<b>(</b>{{Type5|PlotType}} terrain, '''bool''' recalculateAreas = nil, '''bool''' rebuildGraphics) = nil<b>)</b></code>


'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|terrain:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|recalculateAreas:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|rebuildGraphics):
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|Amazon_XP.lua (G&K)}}
:<code>DLC/Expansion/Maps/Amazon_XP.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0344}}<syntaxhighlight lang="lua">plot:SetPlotType(PlotTypes.PLOT_HILLS, false, true); -- These flags are for recalc of areas and rebuild of graphics. Instead of recalc over and over, do recalc at end of loop.</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|Arborea.lua (G&K)}}
:<code>DLC/Expansion/Maps/Arborea.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0611}}<syntaxhighlight lang="lua">plot:SetPlotType(PlotTypes.PLOT_HILLS, false, false);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|AssignStartingPlots.lua (G&K)}}
:<code>DLC/Expansion/Gameplay/Lua/AssignStartingPlots.lua</code>
:{{CodeBegin5}}
{{CodeLine5|2856}}<syntaxhighlight lang="lua">forcePlot:SetPlotType(PlotTypes.PLOT_LAND, false, true);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|3577}}<syntaxhighlight lang="lua">plot:SetPlotType(PlotTypes.PLOT_HILLS, false, true);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|5946}}<syntaxhighlight lang="lua">plot:SetPlotType(PlotTypes.PLOT_MOUNTAIN, false, false);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|5950}}<syntaxhighlight lang="lua">plot:SetPlotType(PlotTypes.PLOT_LAND, false, false);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|9534}}<syntaxhighlight lang="lua">plot:SetPlotType(PlotTypes.PLOT_LAND, false, true)</syntaxhighlight>
{{CodeLine5|9535}}<syntaxhighlight lang="lua">end</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|Europe.lua (G&K)}}
:<code>DLC/Expansion/Maps/Europe.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1132}}<syntaxhighlight lang="lua">adjPlot:SetPlotType(PlotTypes.PLOT_LAND, false, false);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|MapGenerator.lua (G&K)}}
:<code>DLC/Expansion/Gameplay/Lua/MapGenerator.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0173}}<syntaxhighlight lang="lua">plot:SetPlotType(plotTypes[i + 1], false, false);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0567}}<syntaxhighlight lang="lua">plot:SetPlotType(PlotTypes.PLOT_OCEAN);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|NaturalWondersCustomMethods.lua (G&K)}}
:<code>DLC/Expansion/Gameplay/Lua/NaturalWondersCustomMethods.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0144}}<syntaxhighlight lang="lua">plot:SetPlotType(PlotTypes.PLOT_OCEAN, false, false);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0156}}<syntaxhighlight lang="lua">SEPlot:SetPlotType(PlotTypes.PLOT_OCEAN, false, false);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0219}}<syntaxhighlight lang="lua">adjPlot:SetPlotType(PlotTypes.PLOT_MOUNTAIN, false, false);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|Skirmish.lua}}
:<code>Maps/Skirmish.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0255}}<syntaxhighlight lang="lua">plot:SetPlotType(PlotTypes.PLOT_HILLS, false, false)</syntaxhighlight>
{{CodeLine5|0256}}<syntaxhighlight lang="lua">break</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|SetPlotType]]
[[Category:Civ5 Terrain API|SetPlotType]]