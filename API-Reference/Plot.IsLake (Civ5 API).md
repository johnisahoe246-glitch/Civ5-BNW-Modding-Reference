{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Plot}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''int''' Plot:IsLake<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|AssignStartingPlots.lua}}
:<code>Gameplay/Lua/AssignStartingPlots.lua</code>
:{{CodeBegin5}}
{{CodeLine5|4931}}<syntaxhighlight lang="lua">if plot:IsRiver() or plot:IsLake() then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|5001}}<syntaxhighlight lang="lua">if adjPlot:IsLake() then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|AssignStartingPlots.lua (G&K)}}
:<code>DLC/Expansion/Gameplay/Lua/AssignStartingPlots.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1803}}<syntaxhighlight lang="lua">if plot:IsLake() then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|2209}}<syntaxhighlight lang="lua">elseif plot:IsLake() then -- Lakes are Food, Good.</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|3540}}<syntaxhighlight lang="lua">if plot:IsLake() == false then -- Place Fish</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|3885}}<syntaxhighlight lang="lua">if searchPlot:IsLake() then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|5241}}<syntaxhighlight lang="lua">if plot:IsRiver() or plot:IsLake() or plot:IsFreshWater() then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|7150}}<syntaxhighlight lang="lua">elseif plot:IsLake() then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|8052}}<syntaxhighlight lang="lua">if plot:IsLake() == false then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|9246}}<syntaxhighlight lang="lua">if not plot:IsLake() then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|MapmakerUtilities.lua}}
:<code>Gameplay/Lua/MapmakerUtilities.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0323}}<syntaxhighlight lang="lua">if testPlot:IsLake() == false then -- Adjacent plot is salt water!</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|NaturalWondersCustomMethods.lua (G&K)}}
:<code>DLC/Expansion/Gameplay/Lua/NaturalWondersCustomMethods.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0046}}<syntaxhighlight lang="lua">if adjPlot:IsWater() == false or adjPlot:IsLake() == true then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0105}}<syntaxhighlight lang="lua">if terrainType == TerrainTypes.TERRAIN_COAST and plot:IsLake() == false then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|PlotMouseoverInclude.lua}}
:<code>UI/InGame/PlotMouseoverInclude.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0105}}<syntaxhighlight lang="lua">if (plot:IsLake()) then</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|IsLake]]
[[Category:Civ5 Terrain API|IsLake]]