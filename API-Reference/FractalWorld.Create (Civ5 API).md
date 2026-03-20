{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|FractalWorld}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''unknown''' FractalWorld.Create<b>(</b>'''float''' fracXExp = nil, '''float''' fracYExp = nil<b>)</b></code>


'''Returned Value'''
:No description available.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|fracXExp:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|fracYExp:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|Arborea.lua (G&K)}}
:<code>DLC/Expansion/Maps/Arborea.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0653}}<syntaxhighlight lang="lua">local fractal_world = FractalWorld.Create();</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|Create]]
[[Category:Civ5 City Production API|Create]]