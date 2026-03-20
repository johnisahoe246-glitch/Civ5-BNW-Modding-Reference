{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Plot}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''int''' Plot:IsFreshWater<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|AssignStartingPlots.lua (G&K)}}
:<code>DLC/Expansion/Gameplay/Lua/AssignStartingPlots.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0825}}<syntaxhighlight lang="lua">if plot:IsFreshWater() then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|2650}}<syntaxhighlight lang="lua">elseif plot:IsFreshWater() or self.plotDataIsCoastal[plotIndex] == true then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|2974}}<syntaxhighlight lang="lua">elseif plot:IsFreshWater() then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|3524}}<syntaxhighlight lang="lua">if plot:IsFreshWater() then -- Place Wheat</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|3926}}<syntaxhighlight lang="lua">elseif searchPlot:IsFreshWater() then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|5237}}<syntaxhighlight lang="lua">if plot:IsFreshWater() == false then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|5241}}<syntaxhighlight lang="lua">if plot:IsRiver() or plot:IsLake() or plot:IsFreshWater() then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|9049}}<syntaxhighlight lang="lua">if res_plot:IsFreshWater() then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|9228}}<syntaxhighlight lang="lua">elseif terrainType == TerrainTypes.TERRAIN_DESERT and plot:IsFreshWater() then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|PlotHelpManager.lua}}
:<code>UI/InGame/PlotHelpManager.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0247}}<syntaxhighlight lang="lua">if (plot:IsFreshWater()) then</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|IsFreshWater]]
[[Category:Civ5 Terrain API|IsFreshWater]]