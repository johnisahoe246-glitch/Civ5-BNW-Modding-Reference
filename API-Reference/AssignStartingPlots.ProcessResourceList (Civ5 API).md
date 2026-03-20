{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|AssignStartingPlots}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''void''' AssignStartingPlots:ProcessResourceList<b>(</b>'''int''' frequency, '''int''' impact_table_number, table('''int''' => '''int''') plot_list, table('''int''' => table('''int''' => {{Type5|ResourceType}})) resources_to_place<b>)</b></code>


'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|frequency:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|impact_table_number:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|plot_list:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|resources_to_place:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Too many occurences. Only 50 out of 146 are listed.''

{{PseudoH4|Amazon_XP.lua (G&K)}}
:<code>DLC/Expansion/Maps/Amazon_XP.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1442}}<syntaxhighlight lang="lua">self:ProcessResourceList(10, 1, self.marsh_list, resources_to_place)</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1444}}<syntaxhighlight lang="lua">local resources_to_place = {</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1447}}<syntaxhighlight lang="lua">self:ProcessResourceList(13, 1, self.desert_flat_no_feature, resources_to_place)</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1449}}<syntaxhighlight lang="lua">local resources_to_place = {</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1453}}<syntaxhighlight lang="lua">self:ProcessResourceList(22, 1, self.hills_list, resources_to_place)</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1455}}<syntaxhighlight lang="lua">local resources_to_place = {</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1458}}<syntaxhighlight lang="lua">self:ProcessResourceList(75, 1, self.jungle_flat_list, resources_to_place)</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1460}}<syntaxhighlight lang="lua">self:AddModernMinorStrategicsToCityStates()</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1471}}<syntaxhighlight lang="lua">self:ProcessResourceList(99999, 1, self.hills_list, resources_to_place) -- 99999 means one per that many tiles: a single instance.</syntaxhighlight>
{{CodeLine5|1472}}<syntaxhighlight lang="lua">end</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1476}}<syntaxhighlight lang="lua">self:ProcessResourceList(99999, 1, self.land_list, resources_to_place)</syntaxhighlight>
{{CodeLine5|1477}}<syntaxhighlight lang="lua">end</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1481}}<syntaxhighlight lang="lua">self:ProcessResourceList(99999, 1, self.hills_list, resources_to_place)</syntaxhighlight>
{{CodeLine5|1482}}<syntaxhighlight lang="lua">end</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1513}}<syntaxhighlight lang="lua">self:ProcessResourceList(10, 3, self.desert_wheat_list, resources_to_place)</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1515}}<syntaxhighlight lang="lua">local resources_to_place = {</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1517}}<syntaxhighlight lang="lua">self:ProcessResourceList(17, 3, self.banana_list, resources_to_place)</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1519}}<syntaxhighlight lang="lua">local resources_to_place = {</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1521}}<syntaxhighlight lang="lua">self:ProcessResourceList(17, 3, self.plains_flat_no_feature, resources_to_place)</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1523}}<syntaxhighlight lang="lua">local resources_to_place = {</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1525}}<syntaxhighlight lang="lua">self:ProcessResourceList(20, 3, self.grass_flat_no_feature, resources_to_place)</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1527}}<syntaxhighlight lang="lua">local resources_to_place = {</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1529}}<syntaxhighlight lang="lua">self:ProcessResourceList(20, 3, self.dry_grass_flat_no_feature, resources_to_place)</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1531}}<syntaxhighlight lang="lua">local resources_to_place = {</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1533}}<syntaxhighlight lang="lua">self:ProcessResourceList(11, 3, self.hills_open_list, resources_to_place)</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1535}}<syntaxhighlight lang="lua">local resources_to_place = {</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1537}}<syntaxhighlight lang="lua">self:ProcessResourceList(19, 3, self.desert_flat_no_feature, resources_to_place)</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1539}}<syntaxhighlight lang="lua">local resources_to_place = {</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1541}}<syntaxhighlight lang="lua">self:ProcessResourceList(20, 3, self.forest_flat_that_are_not_tundra, resources_to_place)</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1543}}<syntaxhighlight lang="lua">end</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|AssignStartingPlots.lua (G&K)}}
:<code>DLC/Expansion/Gameplay/Lua/AssignStartingPlots.lua</code>
:{{CodeBegin5}}
{{CodeLine5|9406}}<syntaxhighlight lang="lua">self:ProcessResourceList(9 / infertility_quotient, 3, dry_hills, resources_to_place)</syntaxhighlight>
{{CodeLine5|9407}}<syntaxhighlight lang="lua">end</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|9411}}<syntaxhighlight lang="lua">self:ProcessResourceList(14 / infertility_quotient, 3, jungles, resources_to_place)</syntaxhighlight>
{{CodeLine5|9412}}<syntaxhighlight lang="lua">end</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|9416}}<syntaxhighlight lang="lua">self:ProcessResourceList(14 / infertility_quotient, 3, flat_tundra, resources_to_place)</syntaxhighlight>
{{CodeLine5|9417}}<syntaxhighlight lang="lua">end</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|9421}}<syntaxhighlight lang="lua">self:ProcessResourceList(18 / infertility_quotient, 3, flat_plains, resources_to_place)</syntaxhighlight>
{{CodeLine5|9422}}<syntaxhighlight lang="lua">end</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|9426}}<syntaxhighlight lang="lua">self:ProcessResourceList(20 / infertility_quotient, 3, flat_grass, resources_to_place)</syntaxhighlight>
{{CodeLine5|9427}}<syntaxhighlight lang="lua">end</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|9431}}<syntaxhighlight lang="lua">self:ProcessResourceList(24 / infertility_quotient, 3, forests, resources_to_place)</syntaxhighlight>
{{CodeLine5|9432}}<syntaxhighlight lang="lua">end</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|9670}}<syntaxhighlight lang="lua">self:ProcessResourceList(9, 1, self.marsh_list, resources_to_place)</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|9672}}<syntaxhighlight lang="lua">local resources_to_place = {</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|9676}}<syntaxhighlight lang="lua">self:ProcessResourceList(16, 1, self.tundra_flat_no_feature, resources_to_place)</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|9678}}<syntaxhighlight lang="lua">local resources_to_place = {</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|9682}}<syntaxhighlight lang="lua">self:ProcessResourceList(17, 1, self.snow_flat_list, resources_to_place)</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|9684}}<syntaxhighlight lang="lua">local resources_to_place = {</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|9698}}<syntaxhighlight lang="lua">self:ProcessResourceList(33, 1, self.jungle_flat_list, resources_to_place)</syntaxhighlight>
{{CodeLine5|9699}}<syntaxhighlight lang="lua">local resources_to_place = {</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|9702}}<syntaxhighlight lang="lua">self:ProcessResourceList(39, 1, self.forest_flat_list, resources_to_place)</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|9704}}<syntaxhighlight lang="lua">local resources_to_place = {</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|9706}}<syntaxhighlight lang="lua">self:ProcessResourceList(33, 1, self.dry_grass_flat_no_feature, resources_to_place)</syntaxhighlight>
{{CodeLine5|9707}}<syntaxhighlight lang="lua">local resources_to_place = {</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|9709}}<syntaxhighlight lang="lua">self:ProcessResourceList(33, 1, self.plains_flat_no_feature, resources_to_place)</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|9711}}<syntaxhighlight lang="lua">self:AddModernMinorStrategicsToCityStates() -- Added spring 2011</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|9732}}<syntaxhighlight lang="lua">self:ProcessResourceList(99999, 1, self.plains_flat_no_feature, resources_to_place)</syntaxhighlight>
{{CodeLine5|9733}}<syntaxhighlight lang="lua">end</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|9737}}<syntaxhighlight lang="lua">self:ProcessResourceList(99999, 1, self.dry_grass_flat_no_feature, resources_to_place)</syntaxhighlight>
{{CodeLine5|9738}}<syntaxhighlight lang="lua">end</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|9774}}<syntaxhighlight lang="lua">self:ProcessResourceList(8 * bonus_multiplier, 3, self.extra_deer_list, resources_to_place)</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|9776}}<syntaxhighlight lang="lua">local resources_to_place = {</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|9778}}<syntaxhighlight lang="lua">self:ProcessResourceList(10 * bonus_multiplier, 3, self.desert_wheat_list, resources_to_place)</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|9780}}<syntaxhighlight lang="lua">local resources_to_place = {</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|9782}}<syntaxhighlight lang="lua">self:ProcessResourceList(12 * bonus_multiplier, 3, self.tundra_flat_no_feature, resources_to_place)</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|9784}}<syntaxhighlight lang="lua">local resources_to_place = {</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|9786}}<syntaxhighlight lang="lua">self:ProcessResourceList(14 * bonus_multiplier, 3, self.banana_list, resources_to_place)</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|9788}}<syntaxhighlight lang="lua">local resources_to_place = {</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|9790}}<syntaxhighlight lang="lua">self:ProcessResourceList(27 * bonus_multiplier, 3, self.plains_flat_no_feature, resources_to_place)</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|9792}}<syntaxhighlight lang="lua">local resources_to_place = {</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|9794}}<syntaxhighlight lang="lua">self:ProcessResourceList(18 * bonus_multiplier, 3, self.grass_flat_no_feature, resources_to_place)</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|9796}}<syntaxhighlight lang="lua">local resources_to_place = {</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|9798}}<syntaxhighlight lang="lua">self:ProcessResourceList(20 * bonus_multiplier, 3, self.dry_grass_flat_no_feature, resources_to_place)</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|9800}}<syntaxhighlight lang="lua">local resources_to_place = {</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|9802}}<syntaxhighlight lang="lua">self:ProcessResourceList(13 * bonus_multiplier, 3, self.hills_open_list, resources_to_place)</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|9804}}<syntaxhighlight lang="lua">local resources_to_place = {</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|9806}}<syntaxhighlight lang="lua">self:ProcessResourceList(15 * bonus_multiplier, 3, self.tundra_flat_no_feature, resources_to_place)</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|9808}}<syntaxhighlight lang="lua">local resources_to_place = {</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|9810}}<syntaxhighlight lang="lua">self:ProcessResourceList(19 * bonus_multiplier, 3, self.desert_flat_no_feature, resources_to_place)</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|9812}}<syntaxhighlight lang="lua">local resources_to_place = {</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|9814}}<syntaxhighlight lang="lua">self:ProcessResourceList(25 * bonus_multiplier, 3, self.forest_flat_that_are_not_tundra, resources_to_place)</syntaxhighlight>
{{CodeLine5|9815}}<syntaxhighlight lang="lua">end</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|Great_Plains.lua}}
:<code>Maps/Great_Plains.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1422}}<syntaxhighlight lang="lua">self:ProcessResourceList(40, 1, self.dry_grass_flat_no_feature, resources_to_place)</syntaxhighlight>
{{CodeLine5|1423}}<syntaxhighlight lang="lua">local resources_to_place = {</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1425}}<syntaxhighlight lang="lua">self:ProcessResourceList(67, 1, self.plains_flat_no_feature, resources_to_place)</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1427}}<syntaxhighlight lang="lua">self:AddModernMinorStrategicsToCityStates()</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1546}}<syntaxhighlight lang="lua">self:ProcessResourceList(39, 3, self.plains_flat_no_feature, resources_to_place)</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1548}}<syntaxhighlight lang="lua">local resources_to_place = {</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1550}}<syntaxhighlight lang="lua">self:ProcessResourceList(13, 3, self.desert_wheat_list, resources_to_place)</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1552}}<syntaxhighlight lang="lua">local resources_to_place = {</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1554}}<syntaxhighlight lang="lua">self:ProcessResourceList(37, 3, self.plains_flat_no_feature, resources_to_place)</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1556}}<syntaxhighlight lang="lua">local resources_to_place = {</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|ProcessResourceList]]
[[Category:Civ5 Resources API|ProcessResourceList]]