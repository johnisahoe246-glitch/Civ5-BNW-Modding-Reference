{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Plot}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>{{Type5|AreaID}} Plot:GetArea<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|Amazon_XP.lua (G&K)}}
:<code>DLC/Expansion/Maps/Amazon_XP.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0987}}<syntaxhighlight lang="lua">local area = plot:GetArea()</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0989}}<syntaxhighlight lang="lua">-- Adding this check for Great Plains</syntaxhighlight>
{{CodeLine5|0990}}<syntaxhighlight lang="lua">if x < 1 or x >= iW - 1 or y < 1 or y >= iH - 1 then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|AssignStartingPlots.lua (G&K)}}
:<code>DLC/Expansion/Gameplay/Lua/AssignStartingPlots.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0888}}<syntaxhighlight lang="lua">local thisPlotsArea = plot:GetArea()</syntaxhighlight>
{{CodeLine5|0889}}<syntaxhighlight lang="lua">if thisPlotsArea ~= iAreaID then -- This plot is not a member of the landmass, set value to 0</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1554}}<syntaxhighlight lang="lua">local iArea = plot:GetArea();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1791}}<syntaxhighlight lang="lua">local area_of_plot = plot:GetArea();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|5225}}<syntaxhighlight lang="lua">local iAreaID = plot:GetArea();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|6328}}<syntaxhighlight lang="lua">local area = plot:GetArea()</syntaxhighlight>
{{CodeLine5|6329}}<syntaxhighlight lang="lua">if area ~= area_ID and area_ID ~= -1 then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|Boreal.lua (G&K)}}
:<code>DLC/Expansion/Maps/Boreal.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0718}}<syntaxhighlight lang="lua">local area = plot:GetArea()</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0720}}<syntaxhighlight lang="lua">-- Adding this check for Highlands</syntaxhighlight>
{{CodeLine5|0721}}<syntaxhighlight lang="lua">if x < 1 or x >= iW - 1 or y < 1 or y >= iH - 1 then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|Europe.lua (G&K)}}
:<code>DLC/Expansion/Maps/Europe.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0492}}<syntaxhighlight lang="lua">local testAreaID = testPlot:GetArea()</syntaxhighlight>
{{CodeLine5|0493}}<syntaxhighlight lang="lua">local testArea = Map.GetArea(testAreaID)</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|FeatureGenerator.lua (G&K)}}
:<code>DLC/Expansion/Gameplay/Lua/FeatureGenerator.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0382}}<syntaxhighlight lang="lua">local iArea = adjPlot:GetArea()</syntaxhighlight>
{{CodeLine5|0383}}<syntaxhighlight lang="lua">local adjArea = Map.GetArea(iArea)</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|Four_Corners.lua}}
:<code>Maps/Four_Corners.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0498}}<syntaxhighlight lang="lua">local area = plot:GetArea()</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0500}}<syntaxhighlight lang="lua">-- Adding this check for Four Corners</syntaxhighlight>
{{CodeLine5|0501}}<syntaxhighlight lang="lua">if x < 1 or x >= iW - 1 or y < 1 or y >= iH - 1 then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|InlandSea.lua}}
:<code>Maps/InlandSea.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0302}}<syntaxhighlight lang="lua">local area = plot:GetArea()</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0304}}<syntaxhighlight lang="lua">-- Adding this check for Inland Sea</syntaxhighlight>
{{CodeLine5|0305}}<syntaxhighlight lang="lua">if x < 1 or x >= iW - 1 or y < 1 or y >= iH - 1 then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|Lakes.lua}}
:<code>Maps/Lakes.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0194}}<syntaxhighlight lang="lua">local area = plot:GetArea()</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0196}}<syntaxhighlight lang="lua">-- Adding this check for Lakes</syntaxhighlight>
{{CodeLine5|0197}}<syntaxhighlight lang="lua">if y < 4 or y >= iH - 4 then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|MapGenerator.lua (G&K)}}
:<code>DLC/Expansion/Gameplay/Lua/MapGenerator.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0626}}<syntaxhighlight lang="lua">local areaID = plot:GetArea();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|MapmakerUtilities.lua}}
:<code>Gameplay/Lua/MapmakerUtilities.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0098}}<syntaxhighlight lang="lua">local area = plotFirst:GetArea();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0102}}<syntaxhighlight lang="lua">area = plotLast:GetArea();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0138}}<syntaxhighlight lang="lua">local area = plot:GetArea();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|North_vs_South.lua}}
:<code>Maps/North_vs_South.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0669}}<syntaxhighlight lang="lua">local area = plot:GetArea()</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0671}}<syntaxhighlight lang="lua">-- Adding this check for North vs South</syntaxhighlight>
{{CodeLine5|0672}}<syntaxhighlight lang="lua">if x < 1 or x >= iW - 1 or y < 1 or y >= iH - 1 then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|Ring.lua}}
:<code>Maps/Ring.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0642}}<syntaxhighlight lang="lua">local area = plot:GetArea()</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0644}}<syntaxhighlight lang="lua">-- Adding this check for Ring, to force all City States to the polar region in the center.</syntaxhighlight>
{{CodeLine5|0645}}<syntaxhighlight lang="lua">if (x > centWestX and x < centEastX and y > centSouthY and y < centNorthY) == false then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|Skirmish.lua}}
:<code>Maps/Skirmish.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1067}}<syntaxhighlight lang="lua">local area = plot:GetArea()</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1069}}<syntaxhighlight lang="lua">-- Adding this check for Skirmish.</syntaxhighlight>
{{CodeLine5|1070}}<syntaxhighlight lang="lua">if x < 1 or x >= iW - 1 or y < 1 or y >= iH - 1 then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|Terra.lua}}
:<code>Maps/Terra.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0650}}<syntaxhighlight lang="lua">local adjAreaID = adjPlot:GetArea();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0749}}<syntaxhighlight lang="lua">local iAreaID = adjPlot:GetArea();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|West_vs_East.lua}}
:<code>Maps/West_vs_East.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0569}}<syntaxhighlight lang="lua">local area = plot:GetArea()</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0571}}<syntaxhighlight lang="lua">-- Adding this check for West vs East.</syntaxhighlight>
{{CodeLine5|0572}}<syntaxhighlight lang="lua">if x < 1 or x >= iW - 1 or y < 1 or y >= iH - 1 then</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetArea]]
[[Category:Civ5 Terrain API|GetArea]]