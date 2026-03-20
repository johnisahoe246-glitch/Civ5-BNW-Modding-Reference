{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Map}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''int''', '''int''' Map.GetGridSize<b>(</b><b>)</b></code>


'''Returned Values'''
:No description available.


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|Amazon_XP.lua (G&K)}}
:<code>DLC/Expansion/Maps/Amazon_XP.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0052}}<syntaxhighlight lang="lua">local iW, iH = Map.GetGridSize();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0452}}<syntaxhighlight lang="lua">local iW, iH = Map.GetGridSize()</syntaxhighlight>
{{CodeLine5|0453}}<syntaxhighlight lang="lua">local riverPlot;</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0558}}<syntaxhighlight lang="lua">local iW, iH = Map.GetGridSize()</syntaxhighlight>
{{CodeLine5|0559}}<syntaxhighlight lang="lua">thisFlowDirection = thisFlowDirection or FlowDirectionTypes.NO_FLOWDIRECTION;</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0797}}<syntaxhighlight lang="lua">local iW, iH = Map.GetGridSize()</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0799}}<syntaxhighlight lang="lua">-- Place the Amazon!</syntaxhighlight>
{{CodeLine5|0800}}<syntaxhighlight lang="lua">print("Charting the Amazon River (Lua Amazon) ...")</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1434}}<syntaxhighlight lang="lua">local iW, iH = Map.GetGridSize()</syntaxhighlight>
{{CodeLine5|1435}}<syntaxhighlight lang="lua">local uran_amt, horse_amt, oil_amt, iron_amt, coal_amt, alum_amt = self:GetMajorStrategicResourceQuantityValues()</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|AssignStartingPlots.lua (G&K)}}
:<code>DLC/Expansion/Gameplay/Lua/AssignStartingPlots.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0863}}<syntaxhighlight lang="lua">local iW, iH = Map.GetGridSize()</syntaxhighlight>
{{CodeLine5|0864}}<syntaxhighlight lang="lua">local xEnd, yEnd; --[[ These coordinates will be used in case of wrapping landmass,</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0908}}<syntaxhighlight lang="lua">local iW, iH = Map.GetGridSize()</syntaxhighlight>
{{CodeLine5|0909}}<syntaxhighlight lang="lua">local adjusted_table = {};</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1290}}<syntaxhighlight lang="lua">local iW, iH = Map.GetGridSize()</syntaxhighlight>
{{CodeLine5|1291}}<syntaxhighlight lang="lua">local iWestX = rectangle_data_table[1];</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|6100}}<syntaxhighlight lang="lua">local iW, iH = Map.GetGridSize()</syntaxhighlight>
{{CodeLine5|6101}}<syntaxhighlight lang="lua">local ratio = self.iNumCityStates / self.iNumCivs;</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|6447}}<syntaxhighlight lang="lua">local iW, iH = Map.GetGridSize()</syntaxhighlight>
{{CodeLine5|6448}}<syntaxhighlight lang="lua">local iNumCoastal = table.maxn(coastal_plot_list);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|9525}}<syntaxhighlight lang="lua">local iW, iH = Map.GetGridSize()</syntaxhighlight>
{{CodeLine5|9526}}<syntaxhighlight lang="lua">for y = 0, iH - 1 do</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|Boreal.lua (G&K)}}
:<code>DLC/Expansion/Maps/Boreal.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0225}}<syntaxhighlight lang="lua">local iW, iH = Map.GetGridSize()</syntaxhighlight>
{{CodeLine5|0226}}<syntaxhighlight lang="lua">local x = plot:GetX()</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0475}}<syntaxhighlight lang="lua">local iW, iH = Map.GetGridSize()</syntaxhighlight>
{{CodeLine5|0476}}<syntaxhighlight lang="lua">print("Inland Sea - Adding Rivers");</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0565}}<syntaxhighlight lang="lua">local iW, iH = Map.GetGridSize()</syntaxhighlight>
{{CodeLine5|0566}}<syntaxhighlight lang="lua">if iY == iH - 1 then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|FeatureGenerator.lua (G&K)}}
:<code>DLC/Expansion/Gameplay/Lua/FeatureGenerator.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0311}}<syntaxhighlight lang="lua">local iW, iH = Map.GetGridSize()</syntaxhighlight>
{{CodeLine5|0312}}<syntaxhighlight lang="lua">local biggest_ocean = Map.FindBiggestArea(true)</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|FractalWorld.lua}}
:<code>Gameplay/Lua/FractalWorld.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0015}}<syntaxhighlight lang="lua">local gridWidth, gridHeight = Map.GetGridSize();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|GenericWorldAnchor.lua}}
:<code>UI/InGame/GenericWorldAnchor.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0007}}<syntaxhighlight lang="lua">local m_gridWidth, _ = Map.GetGridSize();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|Great_Plains.lua}}
:<code>Maps/Great_Plains.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0789}}<syntaxhighlight lang="lua">local iW, iH = Map.GetGridSize()</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0791}}<syntaxhighlight lang="lua">-- Place the Mississippi!</syntaxhighlight>
{{CodeLine5|0792}}<syntaxhighlight lang="lua">print("Charting the Mississippi (Lua Great Plains) ...")</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ReplayViewer.lua}}
:<code>UI/InGame/Popups/ReplayViewer.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1249}}<syntaxhighlight lang="lua">local mapWidth, mapHeight = Map.GetGridSize();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ResourceIconManager.lua}}
:<code>UI/InGame/ResourceIconManager.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0019}}<syntaxhighlight lang="lua">local g_gridWidth, _ = Map.GetGridSize();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|Ring.lua}}
:<code>Maps/Ring.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0168}}<syntaxhighlight lang="lua">local iW, iH = Map.GetGridSize()</syntaxhighlight>
{{CodeLine5|0169}}<syntaxhighlight lang="lua">local iWH = iW * iH;</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0618}}<syntaxhighlight lang="lua">local iW, iH = Map.GetGridSize()</syntaxhighlight>
{{CodeLine5|0619}}<syntaxhighlight lang="lua">self.iNumCityStatesPerRegion = 0;</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|Skirmish.lua}}
:<code>Maps/Skirmish.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0623}}<syntaxhighlight lang="lua">local iW, iH = Map.GetGridSize()</syntaxhighlight>
{{CodeLine5|0624}}<syntaxhighlight lang="lua">print("Skirmish - Adding Rivers");</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|Tilted_Axis.lua (G&K)}}
:<code>DLC/Expansion/Maps/Tilted_Axis.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0799}}<syntaxhighlight lang="lua">local iW, iH = Map.GetGridSize()</syntaxhighlight>
{{CodeLine5|0800}}<syntaxhighlight lang="lua">if iY >= iH / 2 then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0919}}<syntaxhighlight lang="lua">local iW, iH = Map.GetGridSize()</syntaxhighlight>
{{CodeLine5|0920}}<syntaxhighlight lang="lua">local args = {</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|West_vs_East.lua}}
:<code>Maps/West_vs_East.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0194}}<syntaxhighlight lang="lua">local iW, iH = Map.GetGridSize()</syntaxhighlight>
{{CodeLine5|0195}}<syntaxhighlight lang="lua">print("West vs East - Adding Rivers");</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetGridSize]]