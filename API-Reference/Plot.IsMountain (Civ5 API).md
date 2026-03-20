{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Plot}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''int''' Plot:IsMountain<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|Amazon_XP.lua (G&K)}}
:<code>DLC/Expansion/Maps/Amazon_XP.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0435}}<syntaxhighlight lang="lua">if plot:GetFeatureType() == FeatureTypes.NO_FEATURE and not plot:IsMountain() then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0813}}<syntaxhighlight lang="lua">return plot:IsHills() or plot:IsMountain();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0823}}<syntaxhighlight lang="lua">return (plot:IsHills() or plot:IsMountain()) and (area:GetNumRiverEdges() <   ((area:GetNumTiles() / plotsPerRiverEdge) + 1));</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|AssignStartingPlots.lua (G&K)}}
:<code>DLC/Expansion/Gameplay/Lua/AssignStartingPlots.lua</code>
:{{CodeBegin5}}
{{CodeLine5|5945}}<syntaxhighlight lang="lua">if not plot:IsMountain() then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|Great_Plains.lua}}
:<code>Maps/Great_Plains.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1508}}<syntaxhighlight lang="lua">if plot:IsWater() or plot:IsMountain() or plot:GetFeatureType() == FeatureTypes.FEATURE_OASIS then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|PlotMouseoverInclude.lua}}
:<code>UI/InGame/PlotMouseoverInclude.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0080}}<syntaxhighlight lang="lua">if (plot:IsMountain()) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TutorialChecks.lua}}
:<code>Tutorial/TutorialChecks.lua</code>
:{{CodeBegin5}}
{{CodeLine5|2051}}<syntaxhighlight lang="lua">elseif (pPlot:IsMountain()) then</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|IsMountain]]
[[Category:Civ5 Terrain API|IsMountain]]