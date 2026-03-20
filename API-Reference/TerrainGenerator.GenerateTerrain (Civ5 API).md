{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|TerrainGenerator}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>table('''int''' => {{Type5|TerrainType}}) TerrainGenerator:GenerateTerrain<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
{{PseudoH4|Ice_Age.lua}}
:<code>Maps/Ice_Age.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0317}}<syntaxhighlight lang="lua">local terrainTypes = terraingen:GenerateTerrain()</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0319}}<syntaxhighlight lang="lua">SetTerrainTypes(terrainTypes);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GenerateTerrain]]
[[Category:Civ5 Terrain API|GenerateTerrain]]