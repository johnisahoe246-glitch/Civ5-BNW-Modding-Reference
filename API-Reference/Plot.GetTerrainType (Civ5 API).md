{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Plot}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>{{Type5|TerrainType}} Plot:GetTerrainType<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
''Too many occurences. Only 50 out of 166 are listed.''

{{PseudoH4|Amazon_XP.lua (G&K)}}
:<code>DLC/Expansion/Maps/Amazon_XP.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0263}}<syntaxhighlight lang="lua">terrainTypes[i] = plot:GetTerrainType();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0281}}<syntaxhighlight lang="lua">terrainTypes[i - 1] = plot:GetTerrainType();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1002}}<syntaxhighlight lang="lua">local terrainType = plot:GetTerrainType()</syntaxhighlight>
{{CodeLine5|1003}}<syntaxhighlight lang="lua">if terrainType == TerrainTypes.TERRAIN_SNOW then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1327}}<syntaxhighlight lang="lua">local terrainType = res_plot:GetTerrainType()</syntaxhighlight>
{{CodeLine5|1328}}<syntaxhighlight lang="lua">local featureType = res_plot:GetFeatureType()</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|AssignStartingPlots.lua}}
:<code>Gameplay/Lua/AssignStartingPlots.lua</code>
:{{CodeBegin5}}
{{CodeLine5|4985}}<syntaxhighlight lang="lua">local terrainType = plot:GetTerrainType()</syntaxhighlight>
{{CodeLine5|4986}}<syntaxhighlight lang="lua">local iNumMountains, iNumHills, iNumDeserts, iNumTundra = 0, 0, 0, 0;</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|5004}}<syntaxhighlight lang="lua">terrainType = adjPlot:GetTerrainType()</syntaxhighlight>
{{CodeLine5|5005}}<syntaxhighlight lang="lua">if terrainType == TerrainTypes.TERRAIN_TUNDRA then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|5041}}<syntaxhighlight lang="lua">local terrainType = plot:GetTerrainType()</syntaxhighlight>
{{CodeLine5|5042}}<syntaxhighlight lang="lua">if not (terrainType == TerrainTypes.TERRAIN_DESERT or terrainType == TerrainTypes.TERRAIN_TUNDRA) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|5058}}<syntaxhighlight lang="lua">terrainType = adjPlot:GetTerrainType()</syntaxhighlight>
{{CodeLine5|5059}}<syntaxhighlight lang="lua">if terrainType == TerrainTypes.TERRAIN_GRASS then -- Grass is unacceptable.</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|5133}}<syntaxhighlight lang="lua">local terrainType = plot:GetTerrainType()</syntaxhighlight>
{{CodeLine5|5134}}<syntaxhighlight lang="lua">if terrainType == TerrainTypes.TERRAIN_DESERT or terrainType == TerrainTypes.TERRAIN_TUNDRA then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|5144}}<syntaxhighlight lang="lua">terrainType = adjPlot:GetTerrainType()</syntaxhighlight>
{{CodeLine5|5145}}<syntaxhighlight lang="lua">if terrainType == TerrainTypes.TERRAIN_DESERT or terrainType == TerrainTypes.TERRAIN_TUNDRA then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|5179}}<syntaxhighlight lang="lua">local terrainType = plot:GetTerrainType()</syntaxhighlight>
{{CodeLine5|5180}}<syntaxhighlight lang="lua">if terrainType == TerrainTypes.TERRAIN_GRASS then -- Rejecting grass.</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|5196}}<syntaxhighlight lang="lua">terrainType = adjPlot:GetTerrainType()</syntaxhighlight>
{{CodeLine5|5197}}<syntaxhighlight lang="lua">if terrainType == TerrainTypes.TERRAIN_GRASS then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|AssignStartingPlots.lua (G&K)}}
:<code>DLC/Expansion/Gameplay/Lua/AssignStartingPlots.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0787}}<syntaxhighlight lang="lua">local terrainType = plot:GetTerrainType();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1794}}<syntaxhighlight lang="lua">local terrainType = plot:GetTerrainType()</syntaxhighlight>
{{CodeLine5|1795}}<syntaxhighlight lang="lua">local featureType = plot:GetFeatureType()</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|3787}}<syntaxhighlight lang="lua">local terrainType = plot:GetTerrainType()</syntaxhighlight>
{{CodeLine5|3788}}<syntaxhighlight lang="lua">if terrainType == TerrainTypes.TERRAIN_GRASS then -- Place Stone</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|3878}}<syntaxhighlight lang="lua">local terrainType = searchPlot:GetTerrainType()</syntaxhighlight>
{{CodeLine5|3879}}<syntaxhighlight lang="lua">local featureType = searchPlot:GetFeatureType()</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|5298}}<syntaxhighlight lang="lua">local terrainType = plot:GetTerrainType()</syntaxhighlight>
{{CodeLine5|5299}}<syntaxhighlight lang="lua">if terrainType == TerrainTypes.TERRAIN_GRASS and self.CoreTileCanBeGrass[wn] == true then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|5422}}<syntaxhighlight lang="lua">local terrainType = adjPlot:GetTerrainType();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|5954}}<syntaxhighlight lang="lua">if plot:GetTerrainType() ~= TerrainTypes.TERRAIN_GRASS then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|5958}}<syntaxhighlight lang="lua">if plot:GetTerrainType() ~= TerrainTypes.TERRAIN_PLAINS then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|5965}}<syntaxhighlight lang="lua">if adjPlot:GetTerrainType() ~= TerrainTypes.TERRAIN_COAST then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|6164}}<syntaxhighlight lang="lua">local terrainType = plot:GetTerrainType()</syntaxhighlight>
{{CodeLine5|6165}}<syntaxhighlight lang="lua">if (plotType == PlotTypes.PLOT_LAND or plotType == PlotTypes.PLOT_HILLS) and terrainType ~= TerrainTypes.TERRAIN_SNOW then -- Habitable land plot, process it.</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|9209}}<syntaxhighlight lang="lua">local terrainType = plot:GetTerrainType()</syntaxhighlight>
{{CodeLine5|9210}}<syntaxhighlight lang="lua">local plotIndex = realY * iW + realX + 1;</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|Boreal.lua (G&K)}}
:<code>DLC/Expansion/Maps/Boreal.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0569}}<syntaxhighlight lang="lua">local terrain_type = plot:GetTerrainType()</syntaxhighlight>
{{CodeLine5|0570}}<syntaxhighlight lang="lua">if terrain_type == TerrainTypes.TERRAIN_OCEAN then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|EnemyUnitPanel.lua}}
:<code>UI/InGame/WorldView/EnemyUnitPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1032}}<syntaxhighlight lang="lua">iModifier = pMyUnit:TerrainAttackModifier(pToPlot:GetTerrainType());</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1035}}<syntaxhighlight lang="lua">local terrainTypeBonus = Locale.ConvertTextKey( GameInfo.Terrains[pToPlot:GetTerrainType()].Description );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1333}}<syntaxhighlight lang="lua">iModifier = pTheirUnit:TerrainDefenseModifier(pToPlot:GetTerrainType());</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1336}}<syntaxhighlight lang="lua">local typeBonus = Locale.ConvertTextKey(GameInfo.Terrains[pToPlot:GetTerrainType()].Description);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1605}}<syntaxhighlight lang="lua">iModifier = theirUnit:TerrainDefenseModifier(theirPlot:GetTerrainType());</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1608}}<syntaxhighlight lang="lua">local typeBonus = Locale.ConvertTextKey(GameInfo.Terrains[theirPlot:GetTerrainType()].Description);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|Europe.lua (G&K)}}
:<code>DLC/Expansion/Maps/Europe.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0464}}<syntaxhighlight lang="lua">terrainVal = plot:GetTerrainType();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0998}}<syntaxhighlight lang="lua">local terrainType = plot:GetTerrainType()</syntaxhighlight>
{{CodeLine5|0999}}<syntaxhighlight lang="lua">local iNumMountains, iNumHills, iNumDesert = 0, 0, 0;</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1012}}<syntaxhighlight lang="lua">terrainType = adjPlot:GetTerrainType()</syntaxhighlight>
{{CodeLine5|1013}}<syntaxhighlight lang="lua">if terrainType == TerrainTypes.TERRAIN_DESERT then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1167}}<syntaxhighlight lang="lua">if plot:GetTerrainType() ~= TerrainTypes.TERRAIN_DESERT then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|FeatureGenerator.lua (G&K)}}
:<code>DLC/Expansion/Gameplay/Lua/FeatureGenerator.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0360}}<syntaxhighlight lang="lua">local terrainType = plot:GetTerrainType()</syntaxhighlight>
{{CodeLine5|0361}}<syntaxhighlight lang="lua">if terrainType == TerrainTypes.TERRAIN_COAST then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0373}}<syntaxhighlight lang="lua">local adjTerrainType = adjPlot:GetTerrainType()</syntaxhighlight>
{{CodeLine5|0374}}<syntaxhighlight lang="lua">if adjTerrainType == TerrainTypes.TERRAIN_TUNDRA or adjTerrainType == TerrainTypes.TERRAIN_SNOW then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|Great_Plains_XP.lua (G&K)}}
:<code>DLC/Expansion/Maps/Great_Plains_XP.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1200}}<syntaxhighlight lang="lua">local terrainType = plot:GetTerrainType()</syntaxhighlight>
{{CodeLine5|1201}}<syntaxhighlight lang="lua">if terrainType == TerrainTypes.TERRAIN_GRASS or terrainType == TerrainTypes.TERRAIN_TUNDRA then -- Rejecting grass or tundra.</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1217}}<syntaxhighlight lang="lua">terrainType = adjPlot:GetTerrainType()</syntaxhighlight>
{{CodeLine5|1218}}<syntaxhighlight lang="lua">if terrainType == TerrainTypes.TERRAIN_GRASS or terrainType == TerrainTypes.TERRAIN_TUNDRA then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|Ice_Age.lua}}
:<code>Maps/Ice_Age.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0493}}<syntaxhighlight lang="lua">local terrainType = plot:GetTerrainType()</syntaxhighlight>
{{CodeLine5|0494}}<syntaxhighlight lang="lua">if terrainType == TerrainTypes.TERRAIN_TUNDRA then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|MapGenerator.lua (G&K)}}
:<code>DLC/Expansion/Gameplay/Lua/MapGenerator.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0204}}<syntaxhighlight lang="lua">if(plot:GetTerrainType() == deepWater) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|NaturalWondersCustomMethods.lua (G&K)}}
:<code>DLC/Expansion/Gameplay/Lua/NaturalWondersCustomMethods.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0053}}<syntaxhighlight lang="lua">local terrainType = adjPlot:GetTerrainType()</syntaxhighlight>
{{CodeLine5|0054}}<syntaxhighlight lang="lua">if terrainType == TerrainTypes.TERRAIN_COAST then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0103}}<syntaxhighlight lang="lua">local terrainType = adjPlot:GetTerrainType()</syntaxhighlight>
{{CodeLine5|0104}}<syntaxhighlight lang="lua">local featureType = adjPlot:GetFeatureType()</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0146}}<syntaxhighlight lang="lua">if plot:GetTerrainType() ~= TerrainTypes.TERRAIN_COAST then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0158}}<syntaxhighlight lang="lua">if SEPlot:GetTerrainType() ~= TerrainTypes.TERRAIN_COAST then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|PlotMouseoverInclude.lua}}
:<code>UI/InGame/PlotMouseoverInclude.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0108}}<syntaxhighlight lang="lua">convertedKey = Locale.ConvertTextKey(GameInfo.Terrains[plot:GetTerrainType()].Description);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|Rainforest.lua (G&K)}}
:<code>DLC/Expansion/Maps/Rainforest.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0733}}<syntaxhighlight lang="lua">local terrain_type = plot:GetTerrainType()</syntaxhighlight>
{{CodeLine5|0734}}<syntaxhighlight lang="lua">if terrain_type == TerrainTypes.TERRAIN_GRASS then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ReplayViewer.lua}}
:<code>UI/InGame/Popups/ReplayViewer.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1339}}<syntaxhighlight lang="lua">TerrainType = plot:GetTerrainType(),</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TerrainGenerator.lua}}
:<code>Gameplay/Lua/TerrainGenerator.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0165}}<syntaxhighlight lang="lua">local val = plot:GetTerrainType();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0193}}<syntaxhighlight lang="lua">return plot:GetTerrainType();</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetTerrainType]]
[[Category:Civ5 Terrain API|GetTerrainType]]