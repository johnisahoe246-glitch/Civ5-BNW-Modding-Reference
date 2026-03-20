{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Area}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''int''' Area:GetNumRiverEdges<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|Amazon_XP.lua (G&K)}}
:<code>DLC/Expansion/Maps/Amazon_XP.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0823}}<syntaxhighlight lang="lua">return (plot:IsHills() or plot:IsMountain()) and (area:GetNumRiverEdges() <   ((area:GetNumTiles() / plotsPerRiverEdge) + 1));</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0829}}<syntaxhighlight lang="lua">return (area:GetNumRiverEdges() < (area:GetNumTiles() / plotsPerRiverEdge) + 1);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetNumRiverEdges]]
[[Category:Civ5 Rivers API|GetNumRiverEdges]]