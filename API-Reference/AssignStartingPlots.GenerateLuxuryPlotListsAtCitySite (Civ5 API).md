{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|AssignStartingPlots}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''unknown''' AssignStartingPlots:GenerateLuxuryPlotListsAtCitySite<b>(</b>'''int''' x, '''int''' y, '''int''' radius, '''bool''' removeFeatureIce<b>)</b></code>


'''Returned Value'''
:No description available.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|x:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|y:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|radius:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|removeFeatureIce:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|AssignStartingPlots.lua (G&K)}}
:<code>DLC/Expansion/Gameplay/Lua/AssignStartingPlots.lua</code>
:{{CodeBegin5}}
{{CodeLine5|3831}}<syntaxhighlight lang="lua">self:GenerateLuxuryPlotListsAtCitySite(x, y, 1, true)</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|3833}}<syntaxhighlight lang="lua">-- Set up Conditions checks.</syntaxhighlight>
{{CodeLine5|3834}}<syntaxhighlight lang="lua">local alongOcean = false;</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|6631}}<syntaxhighlight lang="lua">self:GenerateLuxuryPlotListsAtCitySite(x, y, 1, true) -- Removes Feature Ice from coasts adjacent to the city state's new location</syntaxhighlight>
{{CodeLine5|6632}}<syntaxhighlight lang="lua">self:PlaceResourceImpact(x, y, 5, 4) -- City State layer</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|6686}}<syntaxhighlight lang="lua">self:GenerateLuxuryPlotListsAtCitySite(cs_x, cs_y, 1, true) -- Removes Feature Ice from coasts adjacent to the city state's new location</syntaxhighlight>
{{CodeLine5|6687}}<syntaxhighlight lang="lua">self:PlaceResourceImpact(cs_x, cs_y, 5, 4) -- City State layer</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|8527}}<syntaxhighlight lang="lua">luxury_plot_lists = self:GenerateLuxuryPlotListsAtCitySite(x, y, 2, false)</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|8529}}<syntaxhighlight lang="lua">-- First pass, checking only first two rings with a 50% ratio.</syntaxhighlight>
{{CodeLine5|8530}}<syntaxhighlight lang="lua">shuf_list = GetShuffledCopyOfTable(luxury_plot_lists[primary])</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|8547}}<syntaxhighlight lang="lua">luxury_plot_lists = self:GenerateLuxuryPlotListsAtCitySite(x, y, 3, false)</syntaxhighlight>
{{CodeLine5|8548}}<syntaxhighlight lang="lua">shuf_list = GetShuffledCopyOfTable(luxury_plot_lists[primary])</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|8677}}<syntaxhighlight lang="lua">luxury_plot_lists = self:GenerateLuxuryPlotListsAtCitySite(x, y, 2, false)</syntaxhighlight>
{{CodeLine5|8678}}<syntaxhighlight lang="lua">shuf_list = GetShuffledCopyOfTable(luxury_plot_lists[primary])</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|Europe_Scenario.lua (G&K)}}
:<code>DLC/Expansion/Scenarios/MedievalScenario/Europe_Scenario.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1729}}<syntaxhighlight lang="lua">self:GenerateLuxuryPlotListsAtCitySite(x, y, 1, true) -- Removes Feature Ice from coasts adjacent to the city state's new location</syntaxhighlight>
{{CodeLine5|1730}}<syntaxhighlight lang="lua">self:PlaceResourceImpact(x, y, 5, 3) -- City State layer *** Custom for Europe Scenario, down from 4 ***</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GenerateLuxuryPlotListsAtCitySite]]
[[Category:Civ5 Cities API|GenerateLuxuryPlotListsAtCitySite]]