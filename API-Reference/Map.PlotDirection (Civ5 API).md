{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Map}}.<br/>
This is a static method, invoke it with a dot.<br/>
Gets a plot adjacent to the map coordinates given.
}}


=Usage=
<code>{{Type5|Plot}} Map.PlotDirection<b>(</b>'''int''' x, '''int''' y, '''int''' direction<b>)</b></code>


'''Returned Value'''
:An adjacent {{Type5|Plot}} based on the coordinates and direction given.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|x:
|valign="top"| ''The x coordinate of the plot of which to get the adjacent plot.''
|-
|valign="top" style="padding-right:6px;"|y:
|valign="top"| ''The y coordinate of the plot of which to get the adjacent plot.''
|-
|valign="top" style="padding-right:6px;"|direction:
|valign="top"| ''An integer specifying the direction of the adjacent plot relative to the coordinates given. Enumerated in {{Type5|DirectionType}}.''
|}


=Source code samples=
''Too many occurences. Only 50 out of 283 are listed.''

{{PseudoH4|Amazon_XP.lua (G&K)}}
:<code>DLC/Expansion/Maps/Amazon_XP.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0457}}<syntaxhighlight lang="lua">local adjacentPlot = Map.PlotDirection(riverPlot:GetX(), riverPlot:GetY(), DirectionTypes.DIRECTION_EAST);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0463}}<syntaxhighlight lang="lua">riverPlot = Map.PlotDirection(riverPlot:GetX(), riverPlot:GetY(), DirectionTypes.DIRECTION_NORTHEAST);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0466}}<syntaxhighlight lang="lua">local adjacentPlot = Map.PlotDirection(riverPlot:GetX(), riverPlot:GetY(), DirectionTypes.DIRECTION_SOUTHEAST);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0474}}<syntaxhighlight lang="lua">riverPlot = Map.PlotDirection(startPlot:GetX(), startPlot:GetY(), DirectionTypes.DIRECTION_EAST);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0478}}<syntaxhighlight lang="lua">local adjacentPlot = Map.PlotDirection(riverPlot:GetX(), riverPlot:GetY(), DirectionTypes.DIRECTION_SOUTHWEST);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0486}}<syntaxhighlight lang="lua">riverPlot = Map.PlotDirection(startPlot:GetX(), startPlot:GetY(), DirectionTypes.DIRECTION_SOUTHWEST);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0544}}<syntaxhighlight lang="lua">local adjacentPlot = Map.PlotDirection(plot:GetX(), plot:GetY(), direction);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0655}}<syntaxhighlight lang="lua">riverPlot = Map.PlotDirection(riverPlot:GetX(), riverPlot:GetY(), DirectionTypes.DIRECTION_WEST);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0674}}<syntaxhighlight lang="lua">return Map.PlotDirection(riverPlotX, riverPlotY, DirectionTypes.DIRECTION_NORTHWEST);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0678}}<syntaxhighlight lang="lua">return Map.PlotDirection(riverPlotX, riverPlotY, DirectionTypes.DIRECTION_NORTHEAST);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0682}}<syntaxhighlight lang="lua">return Map.PlotDirection(riverPlotX, riverPlotY, DirectionTypes.DIRECTION_EAST);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0686}}<syntaxhighlight lang="lua">return Map.PlotDirection(riverPlotX, riverPlotY, DirectionTypes.DIRECTION_SOUTHWEST);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0690}}<syntaxhighlight lang="lua">return Map.PlotDirection(riverPlotX, riverPlotY, DirectionTypes.DIRECTION_WEST);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|AssignStartingPlots.lua}}
:<code>Gameplay/Lua/AssignStartingPlots.lua</code>
:{{CodeBegin5}}
{{CodeLine5|5000}}<syntaxhighlight lang="lua">local adjPlot = Map.PlotDirection(x, y, direction)</syntaxhighlight>
{{CodeLine5|5001}}<syntaxhighlight lang="lua">if adjPlot:IsLake() then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|AssignStartingPlots.lua (G&K)}}
:<code>DLC/Expansion/Gameplay/Lua/AssignStartingPlots.lua</code>
:{{CodeBegin5}}
{{CodeLine5|5194}}<syntaxhighlight lang="lua">local adjPlot = Map.PlotDirection(x, y, direction)</syntaxhighlight>
{{CodeLine5|5195}}<syntaxhighlight lang="lua">if adjPlot == nil then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|5343}}<syntaxhighlight lang="lua">local adjPlot = Map.PlotDirection(x, y, direction)</syntaxhighlight>
{{CodeLine5|5344}}<syntaxhighlight lang="lua">local plotType = adjPlot:GetPlotType();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|5421}}<syntaxhighlight lang="lua">local adjPlot = Map.PlotDirection(x, y, direction)</syntaxhighlight>
{{CodeLine5|5422}}<syntaxhighlight lang="lua">local terrainType = adjPlot:GetTerrainType();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|5516}}<syntaxhighlight lang="lua">local adjPlot = Map.PlotDirection(x, y, direction)</syntaxhighlight>
{{CodeLine5|5517}}<syntaxhighlight lang="lua">local featureType = adjPlot:GetFeatureType();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|5964}}<syntaxhighlight lang="lua">local adjPlot = Map.PlotDirection(x, y, direction)</syntaxhighlight>
{{CodeLine5|5965}}<syntaxhighlight lang="lua">if adjPlot:GetTerrainType() ~= TerrainTypes.TERRAIN_COAST then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|FeatureGenerator.lua (G&K)}}
:<code>DLC/Expansion/Gameplay/Lua/FeatureGenerator.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0367}}<syntaxhighlight lang="lua">local adjPlot = Map.PlotDirection(x, y, direction)</syntaxhighlight>
{{CodeLine5|0368}}<syntaxhighlight lang="lua">if adjPlot ~= nil then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|FractalWorld.lua}}
:<code>Gameplay/Lua/FractalWorld.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0329}}<syntaxhighlight lang="lua">local nextPlot = Map.PlotDirection(currentX, currentY, currentDirection);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|Great_Plains.lua}}
:<code>Maps/Great_Plains.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1051}}<syntaxhighlight lang="lua">local adjPlot = Map.PlotDirection(x, y, direction)</syntaxhighlight>
{{CodeLine5|1052}}<syntaxhighlight lang="lua">plotType = adjPlot:GetPlotType();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|InGame.lua}}
:<code>UI/InGame/InGame.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0485}}<syntaxhighlight lang="lua">local adjacentPlot = Map.PlotDirection(unitX, unitY, thisDirection);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|MapmakerUtilities.lua}}
:<code>Gameplay/Lua/MapmakerUtilities.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0319}}<syntaxhighlight lang="lua">local testPlot = Map.PlotDirection(x, y, current_direction);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0372}}<syntaxhighlight lang="lua">local NEPlot = Map.PlotDirection(x, y, DirectionTypes.DIRECTION_NORTHEAST);</syntaxhighlight>
{{CodeLine5|0373}}<syntaxhighlight lang="lua">local EPlot = Map.PlotDirection(x, y, DirectionTypes.DIRECTION_EAST);</syntaxhighlight>
{{CodeLine5|0374}}<syntaxhighlight lang="lua">local SEPlot = Map.PlotDirection(x, y, DirectionTypes.DIRECTION_SOUTHEAST);</syntaxhighlight>
{{CodeLine5|0375}}<syntaxhighlight lang="lua">local SWPlot = Map.PlotDirection(x, y, DirectionTypes.DIRECTION_SOUTHWEST);</syntaxhighlight>
{{CodeLine5|0376}}<syntaxhighlight lang="lua">local WPlot = Map.PlotDirection(x, y, DirectionTypes.DIRECTION_WEST);</syntaxhighlight>
{{CodeLine5|0377}}<syntaxhighlight lang="lua">local NWPlot = Map.PlotDirection(x, y, DirectionTypes.DIRECTION_NORTHWEST);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|NaturalWondersCustomMethods.lua (G&K)}}
:<code>DLC/Expansion/Gameplay/Lua/NaturalWondersCustomMethods.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0038}}<syntaxhighlight lang="lua">local SEPlot = Map.PlotDirection(x, y, DirectionTypes.DIRECTION_SOUTHEAST)</syntaxhighlight>
{{CodeLine5|0039}}<syntaxhighlight lang="lua">local southeastX = SEPlot:GetX();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0042}}<syntaxhighlight lang="lua">local adjPlot = Map.PlotDirection(southeastX, southeastY, direction)</syntaxhighlight>
{{CodeLine5|0043}}<syntaxhighlight lang="lua">if adjPlot == nil then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0066}}<syntaxhighlight lang="lua">local adjPlot = Map.PlotDirection(x, y, direction)</syntaxhighlight>
{{CodeLine5|0067}}<syntaxhighlight lang="lua">if adjPlot:IsWater() == false then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0154}}<syntaxhighlight lang="lua">local SEPlot = Map.PlotDirection(x, y, DirectionTypes.DIRECTION_SOUTHEAST)</syntaxhighlight>
{{CodeLine5|0155}}<syntaxhighlight lang="lua">if not SEPlot:IsWater() then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0167}}<syntaxhighlight lang="lua">local adjPlot = Map.PlotDirection(southeastX, southeastY, direction)</syntaxhighlight>
{{CodeLine5|0168}}<syntaxhighlight lang="lua">if adjPlot:GetTerrainType() ~= TerrainTypes.TERRAIN_COAST then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0212}}<syntaxhighlight lang="lua">local adjPlot = Map.PlotDirection(x, y, direction)</syntaxhighlight>
{{CodeLine5|0213}}<syntaxhighlight lang="lua">if adjPlot:GetPlotType() == PlotTypes.PLOT_OCEAN then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TurnsRemaining.lua - DLC_02 DLC}}
:<code>DLC/DLC_02/Scenarios/NewWorldScenario/TurnsRemaining.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0401}}<syntaxhighlight lang="lua">local adjacentPlot = Map.PlotDirection(pPlot:GetX(), pPlot:GetY(), direction);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TurnsRemaining.lua (G&K)}}
:<code>DLC/Expansion/Scenarios/MedievalScenario/TurnsRemaining.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1042}}<syntaxhighlight lang="lua">local adjPlot = Map.PlotDirection(pPlot:GetX(), pPlot:GetY(), direction);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1398}}<syntaxhighlight lang="lua">local adjPlot = Map.PlotDirection(iX, iY, direction);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|WorldBuilderRandomItems.lua}}
:<code>Gameplay/Lua/WorldBuilderRandomItems.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0060}}<syntaxhighlight lang="lua">local otherPlot = Map.PlotDirection(plotX, plotY, direction);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|PlotDirection]]