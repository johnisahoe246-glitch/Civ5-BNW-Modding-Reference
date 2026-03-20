{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|AssignStartingPlots}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''unknown''' AssignStartingPlots:GenerateLuxuryPlotListsInRegion<b>(</b>{{Type5|PlayerID}} region_number<b>)</b></code>


'''Returned Value'''
:No description available.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|region_number:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|AssignStartingPlots.lua (G&K)}}
:<code>DLC/Expansion/Gameplay/Lua/AssignStartingPlots.lua</code>
:{{CodeBegin5}}
{{CodeLine5|8706}}<syntaxhighlight lang="lua">luxury_plot_lists = self:GenerateLuxuryPlotListsInRegion(region_number)</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|8708}}<syntaxhighlight lang="lua">-- Calibrate number of luxuries per region to world size and number of civs</syntaxhighlight>
{{CodeLine5|8709}}<syntaxhighlight lang="lua">-- present. The amount of lux per region should be at its highest when the</syntaxhighlight>
{{CodeLine5|8710}}<syntaxhighlight lang="lua">-- number of civs in the game is closest to "default" for that map size.</syntaxhighlight>
{{CodeLine5|8711}}<syntaxhighlight lang="lua">local target_list = self:GetRegionLuxuryTargetNumbers()</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|Skirmish.lua}}
:<code>Maps/Skirmish.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1177}}<syntaxhighlight lang="lua">luxury_plot_lists = self:GenerateLuxuryPlotListsInRegion(region_number)</syntaxhighlight>
{{CodeLine5|1178}}<syntaxhighlight lang="lua">-- Place one large source of each resource type in each region.</syntaxhighlight>
{{CodeLine5|1179}}<syntaxhighlight lang="lua">local iNumThisLuxToPlace = 1;</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GenerateLuxuryPlotListsInRegion]]