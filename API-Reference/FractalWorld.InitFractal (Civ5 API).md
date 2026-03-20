{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|FractalWorld}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''void''' FractalWorld:InitFractal<b>(</b>'''table''' args<b>)</b></code>


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
{{CodeLine5|0197}}<syntaxhighlight lang="lua">self:InitFractal{continent_grain = grain_dice, rift_grain = rift_dice};</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|InitFractal]]