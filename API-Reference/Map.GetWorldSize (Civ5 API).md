{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Map}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''int''' Map.GetWorldSize<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|Amazon_XP.lua (G&K)}}
:<code>DLC/Expansion/Maps/Amazon_XP.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0066}}<syntaxhighlight lang="lua">local grain_amount = grainvalues[Map.GetWorldSize()];</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0358}}<syntaxhighlight lang="lua">local forest_grain = grainvalues[Map.GetWorldSize()];</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1278}}<syntaxhighlight lang="lua">local iNumToPlace = worldsizes[Map.GetWorldSize()];</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|AssignStartingPlots.lua (G&K)}}
:<code>DLC/Expansion/Gameplay/Lua/AssignStartingPlots.lua</code>
:{{CodeBegin5}}
{{CodeLine5|6017}}<syntaxhighlight lang="lua">local target_number = worldsizes[Map.GetWorldSize()];</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|7856}}<syntaxhighlight lang="lua">local CSluxCount = worldsizes[Map.GetWorldSize()];</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|7870}}<syntaxhighlight lang="lua">local maxToDisable = worldsizes[Map.GetWorldSize()];</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|8452}}<syntaxhighlight lang="lua">local target_list = worldsizes[Map.GetWorldSize()];</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|8493}}<syntaxhighlight lang="lua">local world_size_data = worldsizes[Map.GetWorldSize()];</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|FeatureGenerator.lua (G&K)}}
:<code>DLC/Expansion/Gameplay/Lua/FeatureGenerator.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0339}}<syntaxhighlight lang="lua">local atoll_target = worldsizes[Map.GetWorldSize()];</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|FractalWorld.lua}}
:<code>Gameplay/Lua/FractalWorld.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0077}}<syntaxhighlight lang="lua">local sizekey = Map.GetWorldSize();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|Hemispheres.lua (G&K)}}
:<code>DLC/Expansion/Maps/Hemispheres.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0109}}<syntaxhighlight lang="lua">local archGrain = worldsizes[Map.GetWorldSize()];</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|Highlands.lua}}
:<code>Maps/Highlands.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0140}}<syntaxhighlight lang="lua">local grain_list = worldsizes[Map.GetWorldSize()];</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0164}}<syntaxhighlight lang="lua">local baseNumPlates = platevalues[Map.GetWorldSize()] or 10;</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|Skirmish.lua}}
:<code>Maps/Skirmish.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0144}}<syntaxhighlight lang="lua">local grain = worldsizes[Map.GetWorldSize()];</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TerrainGenerator.lua}}
:<code>Gameplay/Lua/TerrainGenerator.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0067}}<syntaxhighlight lang="lua">local world_info = GameInfo.Worlds[Map.GetWorldSize()];</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetWorldSize]]
[[Category:Civ5 Game Settings API|GetWorldSize]]