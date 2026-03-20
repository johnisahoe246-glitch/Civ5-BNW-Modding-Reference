{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|AssignStartingPlots}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''unknown''' AssignStartingPlots:IterateThroughCandidatePlotList<b>(</b>table('''int''' => '''int''') plot_list, '''int''' region_type<b>)</b></code>


'''Returned Value'''
:No description available.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|plot_list:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|region_type:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|AssignStartingPlots.lua (G&K)}}
:<code>DLC/Expansion/Gameplay/Lua/AssignStartingPlots.lua</code>
:{{CodeBegin5}}
{{CodeLine5|2729}}<syntaxhighlight lang="lua">local election_returns = self:IterateThroughCandidatePlotList(plot_list, region_type)</syntaxhighlight>
{{CodeLine5|2730}}<syntaxhighlight lang="lua">-- If any candidates are eligible, choose one.</syntaxhighlight>
{{CodeLine5|2731}}<syntaxhighlight lang="lua">local found_eligible = election_returns[1];</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|3049}}<syntaxhighlight lang="lua">local election_returns = self:IterateThroughCandidatePlotList(plot_list, region_type)</syntaxhighlight>
{{CodeLine5|3050}}<syntaxhighlight lang="lua">-- If any riverside candidates are eligible, choose one.</syntaxhighlight>
{{CodeLine5|3051}}<syntaxhighlight lang="lua">local found_eligible = election_returns[1];</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|3309}}<syntaxhighlight lang="lua">local election_returns = self:IterateThroughCandidatePlotList(plot_list, region_type)</syntaxhighlight>
{{CodeLine5|3310}}<syntaxhighlight lang="lua">-- If any plots in this area are eligible, choose one.</syntaxhighlight>
{{CodeLine5|3311}}<syntaxhighlight lang="lua">local found_eligible = election_returns[1];</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|IterateThroughCandidatePlotList]]