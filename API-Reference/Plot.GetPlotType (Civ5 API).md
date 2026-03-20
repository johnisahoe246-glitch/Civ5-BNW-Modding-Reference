{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Plot}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>{{Type5|PlotType}} Plot:GetPlotType<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
''Too many occurences. Only 50 out of 169 are listed.''

{{PseudoH4|Amazon_XP.lua (G&K)}}
:<code>DLC/Expansion/Maps/Amazon_XP.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0342}}<syntaxhighlight lang="lua">if plot:GetPlotType() == PlotTypes.PLOT_MOUNTAIN then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0541}}<syntaxhighlight lang="lua">local sum = (numPlots - plot:GetPlotType()) * 20;</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0546}}<syntaxhighlight lang="lua">sum = sum + (numPlots - adjacentPlot:GetPlotType());</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0998}}<syntaxhighlight lang="lua">local plotType = plot:GetPlotType()</syntaxhighlight>
{{CodeLine5|0999}}<syntaxhighlight lang="lua">if plotType == PlotTypes.PLOT_OCEAN or plotType == PlotTypes.PLOT_MOUNTAIN then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1326}}<syntaxhighlight lang="lua">local plotType = res_plot:GetPlotType()</syntaxhighlight>
{{CodeLine5|1327}}<syntaxhighlight lang="lua">local terrainType = res_plot:GetTerrainType()</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|Arborea.lua (G&K)}}
:<code>DLC/Expansion/Maps/Arborea.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0608}}<syntaxhighlight lang="lua">if plot:GetPlotType() ~= PlotTypes.PLOT_OCEAN then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|AssignStartingPlots.lua}}
:<code>Gameplay/Lua/AssignStartingPlots.lua</code>
:{{CodeBegin5}}
{{CodeLine5|5010}}<syntaxhighlight lang="lua">plotType = adjPlot:GetPlotType();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|AssignStartingPlots.lua (G&K)}}
:<code>DLC/Expansion/Gameplay/Lua/AssignStartingPlots.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0786}}<syntaxhighlight lang="lua">local plotType = plot:GetPlotType();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1793}}<syntaxhighlight lang="lua">local plotType = plot:GetPlotType()</syntaxhighlight>
{{CodeLine5|1794}}<syntaxhighlight lang="lua">local terrainType = plot:GetTerrainType()</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|2632}}<syntaxhighlight lang="lua">local plotType = plot:GetPlotType()</syntaxhighlight>
{{CodeLine5|2633}}<syntaxhighlight lang="lua">if plotType == PlotTypes.PLOT_HILLS or plotType == PlotTypes.PLOT_LAND then -- Could host a city.</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|2960}}<syntaxhighlight lang="lua">local plotType = plot:GetPlotType()</syntaxhighlight>
{{CodeLine5|2961}}<syntaxhighlight lang="lua">if plotType ~= PlotTypes.PLOT_MOUNTAIN then -- Not a mountain plot.</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|3228}}<syntaxhighlight lang="lua">local plotType = plot:GetPlotType()</syntaxhighlight>
{{CodeLine5|3229}}<syntaxhighlight lang="lua">if plotType == PlotTypes.PLOT_HILLS or plotType == PlotTypes.PLOT_LAND then -- Land plot, process it.</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|3489}}<syntaxhighlight lang="lua">local plotType = plot:GetPlotType()</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|3491}}<syntaxhighlight lang="lua">if featureType == FeatureTypes.FEATURE_JUNGLE then -- Place Banana</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|3564}}<syntaxhighlight lang="lua">local plotType = plot:GetPlotType()</syntaxhighlight>
{{CodeLine5|3565}}<syntaxhighlight lang="lua">local featureType = plot:GetFeatureType();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|3783}}<syntaxhighlight lang="lua">local plotType = plot:GetPlotType()</syntaxhighlight>
{{CodeLine5|3784}}<syntaxhighlight lang="lua">if plotType == PlotTypes.PLOT_LAND then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|3877}}<syntaxhighlight lang="lua">local plotType = searchPlot:GetPlotType()</syntaxhighlight>
{{CodeLine5|3878}}<syntaxhighlight lang="lua">local terrainType = searchPlot:GetTerrainType()</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|5284}}<syntaxhighlight lang="lua">local plotType = plot:GetPlotType()</syntaxhighlight>
{{CodeLine5|5285}}<syntaxhighlight lang="lua">if plotType == PlotTypes.PLOT_LAND and self.CoreTileCanBeFlatland[wn] == true then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|5344}}<syntaxhighlight lang="lua">local plotType = adjPlot:GetPlotType();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|5949}}<syntaxhighlight lang="lua">if plot:GetPlotType() ~= PlotTypes.PLOT_LAND then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|9532}}<syntaxhighlight lang="lua">local plotType = plot:GetPlotType()</syntaxhighlight>
{{CodeLine5|9533}}<syntaxhighlight lang="lua">if plotType ~= PlotTypes.PLOT_LAND then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|Boreal.lua (G&K)}}
:<code>DLC/Expansion/Maps/Boreal.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0192}}<syntaxhighlight lang="lua">local plot_type = plot:GetPlotType()</syntaxhighlight>
{{CodeLine5|0193}}<syntaxhighlight lang="lua">if plot_type ~= PlotTypes.PLOT_OCEAN then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0232}}<syntaxhighlight lang="lua">local sum = ((numPlots - plot:GetPlotType()) * 20) + direction_influence_value;</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0729}}<syntaxhighlight lang="lua">local plotType = plot:GetPlotType()</syntaxhighlight>
{{CodeLine5|0730}}<syntaxhighlight lang="lua">if plotType == PlotTypes.PLOT_OCEAN or plotType == PlotTypes.PLOT_MOUNTAINS then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|Europe.lua (G&K)}}
:<code>DLC/Expansion/Maps/Europe.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1131}}<syntaxhighlight lang="lua">if adjPlot:GetPlotType() ~= PlotTypes.PLOT_LAND then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|FeatureGenerator.lua (G&K)}}
:<code>DLC/Expansion/Gameplay/Lua/FeatureGenerator.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0355}}<syntaxhighlight lang="lua">local plotType = plot:GetPlotType()</syntaxhighlight>
{{CodeLine5|0356}}<syntaxhighlight lang="lua">if plotType == PlotTypes.PLOT_OCEAN then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0369}}<syntaxhighlight lang="lua">local adjPlotType = adjPlot:GetPlotType()</syntaxhighlight>
{{CodeLine5|0370}}<syntaxhighlight lang="lua">if adjPlotType ~= PlotTypes.PLOT_OCEAN then -- Found land.</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|MapmakerUtilities.lua}}
:<code>Gameplay/Lua/MapmakerUtilities.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0308}}<syntaxhighlight lang="lua">local plotType = plot:GetPlotType()</syntaxhighlight>
{{CodeLine5|0309}}<syntaxhighlight lang="lua">if plotType ~= PlotTypes.PLOT_OCEAN then -- This plot is land, process it.</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0321}}<syntaxhighlight lang="lua">local type = testPlot:GetPlotType()</syntaxhighlight>
{{CodeLine5|0322}}<syntaxhighlight lang="lua">if type == PlotTypes.PLOT_OCEAN then -- Adjacent plot is water! Check if ocean or lake.</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|NaturalWondersCustomMethods.lua (G&K)}}
:<code>DLC/Expansion/Gameplay/Lua/NaturalWondersCustomMethods.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0213}}<syntaxhighlight lang="lua">if adjPlot:GetPlotType() == PlotTypes.PLOT_OCEAN then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0218}}<syntaxhighlight lang="lua">if adjPlot:GetPlotType() ~= PlotTypes.PLOT_MOUNTAIN then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|Rainforest.lua (G&K)}}
:<code>DLC/Expansion/Maps/Rainforest.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0735}}<syntaxhighlight lang="lua">local plot_type = plot:GetPlotType()</syntaxhighlight>
{{CodeLine5|0736}}<syntaxhighlight lang="lua">if plot_type == PlotTypes.PLOT_LAND or plot_type == PlotTypes.PLOT_HILLS then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|Skirmish.lua}}
:<code>Maps/Skirmish.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0253}}<syntaxhighlight lang="lua">local plotType = searchPlot:GetPlotType()</syntaxhighlight>
{{CodeLine5|0254}}<syntaxhighlight lang="lua">if plotType == PlotTypes.PLOT_MOUNTAIN then</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetPlotType]]
[[Category:Civ5 Terrain API|GetPlotType]]