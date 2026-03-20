{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Area}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>{{Type5|AreaID}} Area:GetID<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|Arborea.lua (G&K)}}
:<code>DLC/Expansion/Maps/Arborea.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0222}}<syntaxhighlight lang="lua">iBiggestID = biggest_area:GetID();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|AssignStartingPlots.lua (G&K)}}
:<code>DLC/Expansion/Gameplay/Lua/AssignStartingPlots.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1476}}<syntaxhighlight lang="lua">local iAreaID = biggest_area:GetID();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|5772}}<syntaxhighlight lang="lua">self.iBiggestLandmassID = biggest_landmass:GetID()</syntaxhighlight>
{{CodeLine5|5773}}<syntaxhighlight lang="lua">local biggest_ocean = Map.FindBiggestArea(true)</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|WorldBuilderRandomItems.lua}}
:<code>Gameplay/Lua/WorldBuilderRandomItems.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0087}}<syntaxhighlight lang="lua">if (otherArea:GetID() == area:GetID()) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0141}}<syntaxhighlight lang="lua">if(triedAreas[area:GetID()] == nil) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0159}}<syntaxhighlight lang="lua">triedAreas[bestArea:GetID()] = true;</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0168}}<syntaxhighlight lang="lua">if (bestArea:GetID() == plot:Area():GetID() ) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0182}}<syntaxhighlight lang="lua">if (otherPlot ~= nil and (otherPlot:Area():GetID() == bestArea:GetID() )) then</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetID]]