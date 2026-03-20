{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Plot}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''int''' Plot:IsHills<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|Amazon_XP.lua (G&K)}}
:<code>DLC/Expansion/Maps/Amazon_XP.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0813}}<syntaxhighlight lang="lua">return plot:IsHills() or plot:IsMountain();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0823}}<syntaxhighlight lang="lua">return (plot:IsHills() or plot:IsMountain()) and (area:GetNumRiverEdges() <   ((area:GetNumTiles() / plotsPerRiverEdge) + 1));</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|EnemyUnitPanel.lua}}
:<code>UI/InGame/WorldView/EnemyUnitPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0958}}<syntaxhighlight lang="lua">if (pToPlot:IsHills()) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1560}}<syntaxhighlight lang="lua">if (theirPlot:IsHills()) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|Great_Plains.lua}}
:<code>Maps/Great_Plains.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0536}}<syntaxhighlight lang="lua">if (long < 0.16 and lat > 0.23) and (plot:IsFlatlands() or plot:IsHills()) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|PlotMouseoverInclude.lua}}
:<code>UI/InGame/PlotMouseoverInclude.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0116}}<syntaxhighlight lang="lua">if (plot:IsHills()) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|Ring.lua}}
:<code>Maps/Ring.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0530}}<syntaxhighlight lang="lua">if plot:IsFlatlands() or plot:IsHills() then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TutorialChecks.lua}}
:<code>Tutorial/TutorialChecks.lua</code>
:{{CodeBegin5}}
{{CodeLine5|2049}}<syntaxhighlight lang="lua">if (pPlot:IsHills()) then</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|IsHills]]
[[Category:Civ5 Terrain API|IsHills]]