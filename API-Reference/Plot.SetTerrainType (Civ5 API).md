{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Plot}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''void''' Plot:SetTerrainType<b>(</b>{{Type5|TerrainType}} terrain, '''bool''' recalculateAreas, '''bool''' rebuildGraphics)<b>)</b></code>


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
{{CodeLine5|0399}}<syntaxhighlight lang="lua">plot:SetTerrainType(TerrainTypes.TERRAIN_GRASS, false, false)</syntaxhighlight>
{{CodeLine5|0400}}<syntaxhighlight lang="lua">end</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0404}}<syntaxhighlight lang="lua">plot:SetTerrainType(TerrainTypes.TERRAIN_GRASS, false, false)</syntaxhighlight>
{{CodeLine5|0405}}<syntaxhighlight lang="lua">elseif plot:IsFlatlands() then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0412}}<syntaxhighlight lang="lua">plot:SetTerrainType(TerrainTypes.TERRAIN_GRASS, false, false)</syntaxhighlight>
{{CodeLine5|0413}}<syntaxhighlight lang="lua">if plot:IsFlatlands() then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0420}}<syntaxhighlight lang="lua">plot:SetTerrainType(TerrainTypes.TERRAIN_GRASS, false, false)</syntaxhighlight>
{{CodeLine5|0421}}<syntaxhighlight lang="lua">else</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0424}}<syntaxhighlight lang="lua">plot:SetTerrainType(TerrainTypes.TERRAIN_GRASS, false, false)</syntaxhighlight>
{{CodeLine5|0425}}<syntaxhighlight lang="lua">plot:SetFeatureType(featureMarsh, -1);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|AssignStartingPlots.lua}}
:<code>Gameplay/Lua/AssignStartingPlots.lua</code>
:{{CodeBegin5}}
{{CodeLine5|5598}}<syntaxhighlight lang="lua">plot:SetTerrainType(TerrainTypes.TERRAIN_GRASS, false, false)</syntaxhighlight>
{{CodeLine5|5599}}<syntaxhighlight lang="lua">for loop, direction in ipairs(self.direction_types) do</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|5831}}<syntaxhighlight lang="lua">plot:SetTerrainType(TerrainTypes.TERRAIN_PLAINS, false, false)</syntaxhighlight>
{{CodeLine5|5832}}<syntaxhighlight lang="lua">plot:SetFeatureType(wonder_list[8])</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|5844}}<syntaxhighlight lang="lua">plot:SetTerrainType(TerrainTypes.TERRAIN_PLAINS, false, false)</syntaxhighlight>
{{CodeLine5|5845}}<syntaxhighlight lang="lua">plot:SetFeatureType(wonder_list[10])</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|AssignStartingPlots.lua (G&K)}}
:<code>DLC/Expansion/Gameplay/Lua/AssignStartingPlots.lua</code>
:{{CodeBegin5}}
{{CodeLine5|2857}}<syntaxhighlight lang="lua">forcePlot:SetTerrainType(TerrainTypes.TERRAIN_GRASS, false, true);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|4296}}<syntaxhighlight lang="lua">plot:SetTerrainType(TerrainTypes.TERRAIN_GRASS, false, false)</syntaxhighlight>
{{CodeLine5|4297}}<syntaxhighlight lang="lua">self:PlaceResourceImpact(conv_x, conv_y, 1, 0) -- Disallow strategic resources at this plot, to keep it a farm plot.</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|5955}}<syntaxhighlight lang="lua">plot:SetTerrainType(TerrainTypes.TERRAIN_GRASS, false, false);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|5959}}<syntaxhighlight lang="lua">plot:SetTerrainType(TerrainTypes.TERRAIN_PLAINS, false, false);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|5966}}<syntaxhighlight lang="lua">adjPlot:SetTerrainType(TerrainTypes.TERRAIN_COAST, false, false)</syntaxhighlight>
{{CodeLine5|5967}}<syntaxhighlight lang="lua">end</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|9537}}<syntaxhighlight lang="lua">plot:SetTerrainType(TerrainTypes.TERRAIN_GRASS, false, true)</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|9539}}<syntaxhighlight lang="lua">--print("-"); print("Fixed a Sugar/Jungle at plot", x, y);</syntaxhighlight>
{{CodeLine5|9540}}<syntaxhighlight lang="lua">end</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|Boreal.lua (G&K)}}
:<code>DLC/Expansion/Maps/Boreal.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0197}}<syntaxhighlight lang="lua">plot:SetTerrainType(TerrainTypes.TERRAIN_SNOW, false, false);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0199}}<syntaxhighlight lang="lua">plot:SetTerrainType(TerrainTypes.TERRAIN_TUNDRA, false, false);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|Europe.lua (G&K)}}
:<code>DLC/Expansion/Maps/Europe.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1168}}<syntaxhighlight lang="lua">plot:SetTerrainType(TerrainTypes.TERRAIN_DESERT, false, false)</syntaxhighlight>
{{CodeLine5|1169}}<syntaxhighlight lang="lua">end</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|FeatureGenerator.lua (G&K)}}
:<code>DLC/Expansion/Gameplay/Lua/FeatureGenerator.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0295}}<syntaxhighlight lang="lua">plot:SetTerrainType(self.terrainPlains, false, true)  -- These flags are for recalc of areas and rebuild of graphics. No need to recalc from any of these changes.</syntaxhighlight>
{{CodeLine5|0296}}<syntaxhighlight lang="lua">elseif (plot:IsRiver()) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0299}}<syntaxhighlight lang="lua">plot:SetTerrainType(self.terrainPlains, false, true)</syntaxhighlight>
{{CodeLine5|0300}}<syntaxhighlight lang="lua">elseif (terrainType == self.terrainIce) then</syntaxhighlight>
{{CodeLine5|0301}}<syntaxhighlight lang="lua">plot:SetTerrainType(self.terrainTundra, false, true)</syntaxhighlight>
{{CodeLine5|0302}}<syntaxhighlight lang="lua">end</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|MapGenerator.lua (G&K)}}
:<code>DLC/Expansion/Gameplay/Lua/MapGenerator.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0189}}<syntaxhighlight lang="lua">plot:SetTerrainType(shallowWater, false, false);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0191}}<syntaxhighlight lang="lua">plot:SetTerrainType(deepWater, false, false);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0222}}<syntaxhighlight lang="lua">plot:SetTerrainType(terrainTypes[i], false, false);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|NaturalWondersCustomMethods.lua (G&K)}}
:<code>DLC/Expansion/Gameplay/Lua/NaturalWondersCustomMethods.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0147}}<syntaxhighlight lang="lua">plot:SetTerrainType(TerrainTypes.TERRAIN_COAST, false, false)</syntaxhighlight>
{{CodeLine5|0148}}<syntaxhighlight lang="lua">end</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0159}}<syntaxhighlight lang="lua">SEPlot:SetTerrainType(TerrainTypes.TERRAIN_COAST, false, false)</syntaxhighlight>
{{CodeLine5|0160}}<syntaxhighlight lang="lua">end</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0203}}<syntaxhighlight lang="lua">plot:SetTerrainType(TerrainTypes.TERRAIN_GRASS, false, false)</syntaxhighlight>
{{CodeLine5|0204}}<syntaxhighlight lang="lua">local direction_types = {</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|Ring.lua}}
:<code>Maps/Ring.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0545}}<syntaxhighlight lang="lua">plot:SetTerrainType(self.terrainPlains, false, true)  -- These flags are for recalc of areas and rebuild of graphics. No need to recalc from any of these changes.</syntaxhighlight>
{{CodeLine5|0546}}<syntaxhighlight lang="lua">end</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|SetTerrainType]]
[[Category:Civ5 Terrain API|SetTerrainType]]