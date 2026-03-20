{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|AssignStartingPlots}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''unknown''' AssignStartingPlots.Create<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|Amazon_XP.lua (G&K)}}
:<code>DLC/Expansion/Maps/Amazon_XP.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1547}}<syntaxhighlight lang="lua">local start_plot_database = AssignStartingPlots.Create()</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1549}}<syntaxhighlight lang="lua">print("Dividing the map in to Regions.");</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|Archipelago.lua}}
:<code>Maps/Archipelago.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0105}}<syntaxhighlight lang="lua">local start_plot_database = AssignStartingPlots.Create()</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0107}}<syntaxhighlight lang="lua">print("Dividing the map in to Regions (Lua Archipelago)");</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|Boreal.lua (G&K)}}
:<code>DLC/Expansion/Maps/Boreal.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0782}}<syntaxhighlight lang="lua">local start_plot_database = AssignStartingPlots.Create()</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0784}}<syntaxhighlight lang="lua">print("Dividing the map in to Regions (Lua Boreal)");</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|Great_Plains.lua}}
:<code>Maps/Great_Plains.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1580}}<syntaxhighlight lang="lua">local start_plot_database = AssignStartingPlots.Create()</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1582}}<syntaxhighlight lang="lua">print("Dividing the map in to Regions (Lua Inland Sea)");</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|Highlands.lua}}
:<code>Maps/Highlands.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0601}}<syntaxhighlight lang="lua">local start_plot_database = AssignStartingPlots.Create()</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0603}}<syntaxhighlight lang="lua">print("Dividing the map in to Regions (Lua Highlands)");</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|Large_Islands.lua (G&K)}}
:<code>DLC/Expansion/Maps/Large_Islands.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1116}}<syntaxhighlight lang="lua">local start_plot_database = AssignStartingPlots.Create()</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1118}}<syntaxhighlight lang="lua">print("Dividing the map in to Regions (Lua Large Islands)");</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|Ring.lua}}
:<code>Maps/Ring.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0672}}<syntaxhighlight lang="lua">local start_plot_database = AssignStartingPlots.Create()</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0674}}<syntaxhighlight lang="lua">print("Dividing the map in to Regions (Lua Ring)"); -- Custom for Ring</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|Create]]
[[Category:Civ5 City Production API|Create]]