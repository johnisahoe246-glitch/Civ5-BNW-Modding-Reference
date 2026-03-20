{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|AssignStartingPlots}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''int''', '''bool''' AssignStartingPlots:EvaluateCandidatePlot<b>(</b>'''int''' plotIndex, '''int''' region_type<b>)</b></code>


'''Returned Values'''
:No description available.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|plotIndex:
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
{{CodeLine5|2763}}<syntaxhighlight lang="lua">local score, meets_minimums = self:EvaluateCandidatePlot(plotIndex, region_type)</syntaxhighlight>
{{CodeLine5|2764}}<syntaxhighlight lang="lua">-- Test current plot against best known plot.</syntaxhighlight>
{{CodeLine5|2765}}<syntaxhighlight lang="lua">if meets_minimums == true then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|2816}}<syntaxhighlight lang="lua">local score, meets_minimums = self:EvaluateCandidatePlot(closestPlot, region_type)</syntaxhighlight>
{{CodeLine5|2817}}<syntaxhighlight lang="lua">-- Assign this plot as the start for this region.</syntaxhighlight>
{{CodeLine5|2818}}<syntaxhighlight lang="lua">self.startingPlots[region_number] = {x, y, score};</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|EvaluateCandidatePlot]]