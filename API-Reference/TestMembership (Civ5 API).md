{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a global function. Use: <code>include("MapmakerUtilities.lua")</code>
}}


=Usage=
<code>'''int''' TestMembership<b>(</b>table('''int''' => {{Type5|PlayerID}}) table, {{Type5|PlayerID}} value<b>)</b></code>


'''Returned Value'''
:No description available.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|table:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|value:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|Amazon_XP.lua (G&K)}}
:<code>DLC/Expansion/Maps/Amazon_XP.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1037}}<syntaxhighlight lang="lua">local test = TestMembership(self.resourceIDs_assigned_to_regions, res_ID)</syntaxhighlight>
{{CodeLine5|1038}}<syntaxhighlight lang="lua">if self.iNumTypesAssignedToRegions < self.iNumMaxAllowedForRegions or test == true then -- Not a new type that would exceed number of allowed types, so continue.</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1071}}<syntaxhighlight lang="lua">local test = TestMembership(self.resourceIDs_assigned_to_regions, res_ID)</syntaxhighlight>
{{CodeLine5|1072}}<syntaxhighlight lang="lua">if self.iNumTypesAssignedToRegions < self.iNumMaxAllowedForRegions or test == true then -- Won't exceed allowed types.</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1160}}<syntaxhighlight lang="lua">local already_assigned = TestMembership(self.resourceIDs_assigned_to_regions, resource_ID)</syntaxhighlight>
{{CodeLine5|1161}}<syntaxhighlight lang="lua">if not already_assigned then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1174}}<syntaxhighlight lang="lua">local test = TestMembership(self.resourceIDs_assigned_to_regions, res_ID)</syntaxhighlight>
{{CodeLine5|1175}}<syntaxhighlight lang="lua">if test == false then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1227}}<syntaxhighlight lang="lua">local test1 = TestMembership(self.resourceIDs_assigned_to_regions, res_ID)</syntaxhighlight>
{{CodeLine5|1228}}<syntaxhighlight lang="lua">local test2 = TestMembership(self.resourceIDs_assigned_to_cs, res_ID)</syntaxhighlight>
{{CodeLine5|1229}}<syntaxhighlight lang="lua">if test1 == false and test2 == false then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|AssignStartingPlots.lua (G&K)}}
:<code>DLC/Expansion/Gameplay/Lua/AssignStartingPlots.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1558}}<syntaxhighlight lang="lua">if TestMembership(land_area_IDs, iArea) == false then -- This plot is the first detected in its AreaID.</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1617}}<syntaxhighlight lang="lua">if TestMembership(fertility_value_list, interim_table[tableConstructionLoop]) == true then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1690}}<syntaxhighlight lang="lua">if TestMembership(inhabitedAreaIDs, bestRemainingArea) == false then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|6153}}<syntaxhighlight lang="lua">if TestMembership(areas_inhabited_by_civs, region_areaID) == false then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|6197}}<syntaxhighlight lang="lua">if TestMembership(areas_inhabited_by_civs, areaID) == true then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|6210}}<syntaxhighlight lang="lua">if TestMembership(areas_uninhabited, areaID) == true then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|MapmakerUtilities.lua}}
:<code>Gameplay/Lua/MapmakerUtilities.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0073}}<syntaxhighlight lang="lua">local bCheckTeamList = TestMembership(teams_with_major_civs, teamID)</syntaxhighlight>
{{CodeLine5|0074}}<syntaxhighlight lang="lua">if bCheckTeamList == false then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0490}}<syntaxhighlight lang="lua">local bTest = TestMembership(priorityRegionIDs, region_type);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0509}}<syntaxhighlight lang="lua">local bTest = TestMembership(avoidRegionIDs, region_type);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|TestMembership]]