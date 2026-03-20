{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Map}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''int''' Map.GetFractalFlags<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|FeatureGenerator.lua (G&K)}}
:<code>DLC/Expansion/Gameplay/Lua/FeatureGenerator.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0111}}<syntaxhighlight lang="lua">fractalFlags = Map.GetFractalFlags(),</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|FractalWorld.lua}}
:<code>Gameplay/Lua/FractalWorld.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0026}}<syntaxhighlight lang="lua">iFlags = Map.GetFractalFlags(),</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|MultilayeredFractal.lua (G&K)}}
:<code>DLC/Expansion/Gameplay/Lua/MultilayeredFractal.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0131}}<syntaxhighlight lang="lua">local iTerrainFlags = Map.GetFractalFlags(); -- Matches wrap to that of the map.</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TerrainGenerator.lua}}
:<code>Gameplay/Lua/TerrainGenerator.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0079}}<syntaxhighlight lang="lua">fractalFlags   = Map.GetFractalFlags(),</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetFractalFlags]]