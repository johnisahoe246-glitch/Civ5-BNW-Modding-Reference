{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Area}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''int''' Area:GetNumTiles<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|Amazon_XP.lua (G&K)}}
:<code>DLC/Expansion/Maps/Amazon_XP.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0823}}<syntaxhighlight lang="lua">return (plot:IsHills() or plot:IsMountain()) and (area:GetNumRiverEdges() <   ((area:GetNumTiles() / plotsPerRiverEdge) + 1));</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0829}}<syntaxhighlight lang="lua">return (area:GetNumRiverEdges() < (area:GetNumTiles() / plotsPerRiverEdge) + 1);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|Arborea.lua (G&K)}}
:<code>DLC/Expansion/Maps/Arborea.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0218}}<syntaxhighlight lang="lua">iNumBiggestAreaTiles = biggest_area:GetNumTiles();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|AssignStartingPlots.lua (G&K)}}
:<code>DLC/Expansion/Gameplay/Lua/AssignStartingPlots.lua</code>
:{{CodeBegin5}}
{{CodeLine5|5776}}<syntaxhighlight lang="lua">iNumBiggestOceanPlots = biggest_ocean:GetNumTiles()</syntaxhighlight>
{{CodeLine5|5777}}<syntaxhighlight lang="lua">end</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|Europe.lua (G&K)}}
:<code>DLC/Expansion/Maps/Europe.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0494}}<syntaxhighlight lang="lua">local testArea_size = testArea:GetNumTiles()</syntaxhighlight>
{{CodeLine5|0495}}<syntaxhighlight lang="lua">if testArea_size >= 10 then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1045}}<syntaxhighlight lang="lua">local iNumBiggestOceanPlots = biggest_ocean:GetNumTiles()</syntaxhighlight>
{{CodeLine5|1046}}<syntaxhighlight lang="lua">if iNumBiggestOceanPlots > (iW * iH) / 4 then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|FeatureGenerator.lua (G&K)}}
:<code>DLC/Expansion/Gameplay/Lua/FeatureGenerator.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0384}}<syntaxhighlight lang="lua">local iNumAreaPlots = adjArea:GetNumTiles()</syntaxhighlight>
{{CodeLine5|0385}}<syntaxhighlight lang="lua">if iNumAreaPlots > biggest_adj_area then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|Great_Plains_XP.lua (G&K)}}
:<code>DLC/Expansion/Maps/Great_Plains_XP.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1247}}<syntaxhighlight lang="lua">local iNumBiggestOceanPlots = biggest_ocean:GetNumTiles()</syntaxhighlight>
{{CodeLine5|1248}}<syntaxhighlight lang="lua">self.bWorldHasOceans = false;</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|MapGenerator.lua (G&K)}}
:<code>DLC/Expansion/Gameplay/Lua/MapGenerator.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0628}}<syntaxhighlight lang="lua">local numTiles = area:GetNumTiles();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0700}}<syntaxhighlight lang="lua">local scaler = (area:GetNumTiles() + (tilesPerGoody/2))/tilesPerGoody;</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetNumTiles]]