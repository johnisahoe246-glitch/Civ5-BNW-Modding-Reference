{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Map}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>{{Type5|Area}} Map.FindBiggestArea<b>(</b>'''bool''' ocean<b>)</b></code>


'''Returned Value'''
:No description available.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|ocean:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|Arborea.lua (G&K)}}
:<code>DLC/Expansion/Maps/Arborea.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0217}}<syntaxhighlight lang="lua">biggest_area = Map.FindBiggestArea(false);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|AssignStartingPlots.lua (G&K)}}
:<code>DLC/Expansion/Gameplay/Lua/AssignStartingPlots.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1475}}<syntaxhighlight lang="lua">local biggest_area = Map.FindBiggestArea(false);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|5771}}<syntaxhighlight lang="lua">local biggest_landmass = Map.FindBiggestArea(false)</syntaxhighlight>
{{CodeLine5|5772}}<syntaxhighlight lang="lua">self.iBiggestLandmassID = biggest_landmass:GetID()</syntaxhighlight>
{{CodeLine5|5773}}<syntaxhighlight lang="lua">local biggest_ocean = Map.FindBiggestArea(true)</syntaxhighlight>
{{CodeLine5|5774}}<syntaxhighlight lang="lua">local iNumBiggestOceanPlots = 0;</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|Europe.lua (G&K)}}
:<code>DLC/Expansion/Maps/Europe.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1044}}<syntaxhighlight lang="lua">local biggest_ocean = Map.FindBiggestArea(true)</syntaxhighlight>
{{CodeLine5|1045}}<syntaxhighlight lang="lua">local iNumBiggestOceanPlots = biggest_ocean:GetNumTiles()</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|FindBiggestArea]]
[[Category:Civ5 Terrain API|FindBiggestArea]]