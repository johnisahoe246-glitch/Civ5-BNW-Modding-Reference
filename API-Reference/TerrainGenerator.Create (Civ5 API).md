{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|TerrainGenerator}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''unknown''' TerrainGenerator.Create<b>(</b>'''table''' args<b>)</b></code>


'''Returned Value'''
:No description available.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|args:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|Arborea.lua (G&K)}}
:<code>DLC/Expansion/Maps/Arborea.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0730}}<syntaxhighlight lang="lua">local terraingen = TerrainGenerator.Create(args);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|Fractal.lua}}
:<code>Maps/Fractal.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0043}}<syntaxhighlight lang="lua">local terraingen = TerrainGenerator.Create();</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|Create]]
[[Category:Civ5 City Production API|Create]]