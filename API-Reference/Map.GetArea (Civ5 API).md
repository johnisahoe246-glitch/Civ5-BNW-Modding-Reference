{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Map}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>{{Type5|Area}} Map.GetArea<b>(</b>{{Type5|AreaID}} areaID<b>)</b></code>


'''Returned Value'''
:No description available.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|areaID:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|AssignStartingPlots.lua (G&K)}}
:<code>DLC/Expansion/Gameplay/Lua/AssignStartingPlots.lua</code>
:{{CodeBegin5}}
{{CodeLine5|8275}}<syntaxhighlight lang="lua">region_area_object = Map.GetArea(iAreaID);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|Europe.lua (G&K)}}
:<code>DLC/Expansion/Maps/Europe.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0493}}<syntaxhighlight lang="lua">local testArea = Map.GetArea(testAreaID)</syntaxhighlight>
{{CodeLine5|0494}}<syntaxhighlight lang="lua">local testArea_size = testArea:GetNumTiles()</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|FeatureGenerator.lua (G&K)}}
:<code>DLC/Expansion/Gameplay/Lua/FeatureGenerator.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0383}}<syntaxhighlight lang="lua">local adjArea = Map.GetArea(iArea)</syntaxhighlight>
{{CodeLine5|0384}}<syntaxhighlight lang="lua">local iNumAreaPlots = adjArea:GetNumTiles()</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|MapGenerator.lua (G&K)}}
:<code>DLC/Expansion/Gameplay/Lua/MapGenerator.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0627}}<syntaxhighlight lang="lua">local area = Map.GetArea(areaID);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetArea]]
[[Category:Civ5 Terrain API|GetArea]]