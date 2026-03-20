{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|AssignStartingPlots}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''int''' AssignStartingPlots:PlaceSpecificNumberOfResources<b>(</b>{{Type5|ResourceType}} resource_, {{Type5|ResourceType}} quantity, '''int''' amount, '''float''' ratio, '''int''' impact_table_number, '''int''' min_radius, '''int''' max_radius, table('''int''' => {{Type5|PlayerID}}) plot_list<b>)</b></code>


'''Returned Value'''
:No description available.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|resource_:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|quantity:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|amount:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|ratio:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|impact_table_number:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|min_radius:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|max_radius:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|plot_list:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|Amazon_XP.lua (G&K)}}
:<code>DLC/Expansion/Maps/Amazon_XP.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1281}}<syntaxhighlight lang="lua">self:PlaceSpecificNumberOfResources(self.oil_ID, sea_oil_amt, iNumToPlace, 0.2, 1, 4, 7, self.coast_list)</syntaxhighlight>
{{CodeLine5|1282}}<syntaxhighlight lang="lua">end</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|AssignStartingPlots.lua (G&K)}}
:<code>DLC/Expansion/Gameplay/Lua/AssignStartingPlots.lua</code>
:{{CodeBegin5}}
{{CodeLine5|3737}}<syntaxhighlight lang="lua">iNumLeftToPlace = self:PlaceSpecificNumberOfResources(self.iron_ID, iron_amt, 1, 1, -1, 0, 0, shuf_list);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|3744}}<syntaxhighlight lang="lua">iNumLeftToPlace = self:PlaceSpecificNumberOfResources(self.horse_ID, horse_amt, 1, 1, -1, 0, 0, shuf_list);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|3751}}<syntaxhighlight lang="lua">iNumLeftToPlace = self:PlaceSpecificNumberOfResources(self.oil_ID, oil_amt, 1, 1, -1, 0, 0, shuf_list);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|8531}}<syntaxhighlight lang="lua">local iNumLeftToPlace = self:PlaceSpecificNumberOfResources(this_region_luxury, 1, iNumToPlace, 0.5, -1, 0, 0, shuf_list);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|8534}}<syntaxhighlight lang="lua">iNumLeftToPlace = self:PlaceSpecificNumberOfResources(this_region_luxury, 1, iNumLeftToPlace, 0.5, -1, 0, 0, shuf_list);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|8549}}<syntaxhighlight lang="lua">iNumLeftToPlace = self:PlaceSpecificNumberOfResources(this_region_luxury, 1, iNumLeftToPlace, 1, -1, 0, 0, shuf_list);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|8578}}<syntaxhighlight lang="lua">randoms_to_place = self:PlaceSpecificNumberOfResources(random_res, 1, 1, 1, -1, 0, 0, shuf_list);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|8679}}<syntaxhighlight lang="lua">local iNumLeftToPlace = self:PlaceSpecificNumberOfResources(use_this_ID, 1, 1, 1, -1, 0, 0, shuf_list);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|8682}}<syntaxhighlight lang="lua">iNumLeftToPlace = self:PlaceSpecificNumberOfResources(use_this_ID, 1, 1, 1, -1, 0, 0, shuf_list);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|8726}}<syntaxhighlight lang="lua">iNumLeftToPlace = self:PlaceSpecificNumberOfResources(res_ID, 1, iNumThisLuxToPlace, 0.3, 2, 0, 3, shuf_list);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|8729}}<syntaxhighlight lang="lua">iNumLeftToPlace = self:PlaceSpecificNumberOfResources(res_ID, 1, iNumLeftToPlace, 0.3, 2, 0, 3, shuf_list);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|8733}}<syntaxhighlight lang="lua">iNumLeftToPlace = self:PlaceSpecificNumberOfResources(res_ID, 1, iNumLeftToPlace, 0.4, 2, 0, 2, shuf_list);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|8737}}<syntaxhighlight lang="lua">iNumLeftToPlace = self:PlaceSpecificNumberOfResources(res_ID, 1, iNumLeftToPlace, 0.5, 2, 0, 2, shuf_list);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|8779}}<syntaxhighlight lang="lua">iNumLeftToPlace = self:PlaceSpecificNumberOfResources(res_ID, 1, iNumThisLuxToPlace, 0.25, 2, 4, 6, current_list);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|8782}}<syntaxhighlight lang="lua">iNumLeftToPlace = self:PlaceSpecificNumberOfResources(res_ID, 1, iNumLeftToPlace, 0.25, 2, 4, 6, current_list);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|8790}}<syntaxhighlight lang="lua">iNumLeftToPlace = self:PlaceSpecificNumberOfResources(res_ID, 1, iNumLeftToPlace, 0.3, 2, 4, 6, current_list);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|9274}}<syntaxhighlight lang="lua">local iNumLeftToPlace = self:PlaceSpecificNumberOfResources(self.fish_ID, 1, 1, 1, -1, 0, 0, shuf_list);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|9474}}<syntaxhighlight lang="lua">local iNumLeftToPlace = self:PlaceSpecificNumberOfResources(use_this_ID, res_amt, 1, 1, -1, 0, 0, shuf_list);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|9477}}<syntaxhighlight lang="lua">iNumLeftToPlace = self:PlaceSpecificNumberOfResources(use_this_ID, res_amt, 1, 1, -1, 0, 0, shuf_list);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|Skirmish.lua}}
:<code>Maps/Skirmish.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1181}}<syntaxhighlight lang="lua">iNumLeftToPlace = self:PlaceSpecificNumberOfResources(res_ID, res_amt, iNumThisLuxToPlace, 0.3, 1, 1, 1, shuf_list);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1184}}<syntaxhighlight lang="lua">iNumLeftToPlace = self:PlaceSpecificNumberOfResources(res_ID, res_amt, iNumLeftToPlace, 0.3, 1, 1, 1, shuf_list);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1188}}<syntaxhighlight lang="lua">iNumLeftToPlace = self:PlaceSpecificNumberOfResources(res_ID, res_amt, iNumLeftToPlace, 0.4, 1, 1, 1, shuf_list);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1192}}<syntaxhighlight lang="lua">iNumLeftToPlace = self:PlaceSpecificNumberOfResources(res_ID, res_amt, iNumLeftToPlace, 0.5, 1, 1, 1, shuf_list);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1197}}<syntaxhighlight lang="lua">iNumLeftToPlace = self:PlaceSpecificNumberOfResources(res_ID, res_sm, iNumThisLuxToPlace, 0.3, 1, 0, 0, shuf_list);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1200}}<syntaxhighlight lang="lua">iNumLeftToPlace = self:PlaceSpecificNumberOfResources(res_ID, res_sm, iNumLeftToPlace, 0.3, 1, 0, 0, shuf_list);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1204}}<syntaxhighlight lang="lua">iNumLeftToPlace = self:PlaceSpecificNumberOfResources(res_ID, res_sm, iNumLeftToPlace, 0.4, 1, 0, 0, shuf_list);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1208}}<syntaxhighlight lang="lua">iNumLeftToPlace = self:PlaceSpecificNumberOfResources(res_ID, res_sm, iNumLeftToPlace, 0.5, 1, 0, 0, shuf_list);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|PlaceSpecificNumberOfResources]]
[[Category:Civ5 Resources API|PlaceSpecificNumberOfResources]]