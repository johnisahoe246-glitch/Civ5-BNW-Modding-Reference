{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a global function. Use: <code>include("MapGenerator.lua")</code>
}}


=Usage=
<code>'''void''' SetPlotTypes<b>(</b>table('''int''' => {{Type5|PlotType}}) plotTypes<b>)</b></code>


'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|plotTypes:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|Amazon_XP.lua (G&K)}}
:<code>DLC/Expansion/Maps/Amazon_XP.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0240}}<syntaxhighlight lang="lua">SetPlotTypes(plotTypes);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|Arborea.lua (G&K)}}
:<code>DLC/Expansion/Maps/Arborea.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0214}}<syntaxhighlight lang="lua">SetPlotTypes(self.plotTypes);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|Europe.lua (G&K)}}
:<code>DLC/Expansion/Maps/Europe.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0405}}<syntaxhighlight lang="lua">SetPlotTypes(plotsEur);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|Four_Corners.lua}}
:<code>Maps/Four_Corners.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0174}}<syntaxhighlight lang="lua">SetPlotTypes(plot_list);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|Hemispheres.lua (G&K)}}
:<code>DLC/Expansion/Maps/Hemispheres.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0883}}<syntaxhighlight lang="lua">SetPlotTypes(plotsHemi);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|InlandSea.lua}}
:<code>Maps/InlandSea.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0129}}<syntaxhighlight lang="lua">SetPlotTypes(plotsIS);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|Lakes.lua}}
:<code>Maps/Lakes.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0132}}<syntaxhighlight lang="lua">SetPlotTypes(plotsLakes);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|Large_Islands.lua (G&K)}}
:<code>DLC/Expansion/Maps/Large_Islands.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1036}}<syntaxhighlight lang="lua">SetPlotTypes(plotsLI);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|Ring.lua}}
:<code>Maps/Ring.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0431}}<syntaxhighlight lang="lua">SetPlotTypes(plotsRing);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|Skirmish.lua}}
:<code>Maps/Skirmish.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0228}}<syntaxhighlight lang="lua">SetPlotTypes(plotsSkirmish);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|Terra.lua}}
:<code>Maps/Terra.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0565}}<syntaxhighlight lang="lua">SetPlotTypes(plotsTerra);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|SetPlotTypes]]