{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a global function. Use: <code>include("MapmakerUtilities.lua")</code>
}}


=Usage=
<code>table('''int''' => {{Type5|PlayerID}}) GetShuffledCopyOfTable<b>(</b>table('''int''' => '''int''') incoming_table<b>)</b></code>


'''Returned Value'''
:No description available.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|incoming_table:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Too many occurences. Only 50 out of 322 are listed.''

{{PseudoH4|Amazon_XP.lua (G&K)}}
:<code>DLC/Expansion/Maps/Amazon_XP.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1233}}<syntaxhighlight lang="lua">local randomized_version = GetShuffledCopyOfTable(remaining_resource_IDs)</syntaxhighlight>
{{CodeLine5|1234}}<syntaxhighlight lang="lua">local countdown = math.min(self.iNumTypesUnassigned, maxToDisable);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|AssignStartingPlots.lua}}
:<code>Gameplay/Lua/AssignStartingPlots.lua</code>
:{{CodeBegin5}}
{{CodeLine5|5525}}<syntaxhighlight lang="lua">local candidate_plot_list = GetShuffledCopyOfTable(self.geyser_list)</syntaxhighlight>
{{CodeLine5|5526}}<syntaxhighlight lang="lua">for loop, plotIndex in ipairs(candidate_plot_list) do</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|5781}}<syntaxhighlight lang="lua">local candidate_plot_list = GetShuffledCopyOfTable(self.krakatoa_list)</syntaxhighlight>
{{CodeLine5|5782}}<syntaxhighlight lang="lua">for loop, plotIndex in ipairs(candidate_plot_list) do</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|5822}}<syntaxhighlight lang="lua">local candidate_plot_list = GetShuffledCopyOfTable(self.mystical_list)</syntaxhighlight>
{{CodeLine5|5823}}<syntaxhighlight lang="lua">for loop, plotIndex in ipairs(candidate_plot_list) do</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|AssignStartingPlots.lua (G&K)}}
:<code>DLC/Expansion/Gameplay/Lua/AssignStartingPlots.lua</code>
:{{CodeBegin5}}
{{CodeLine5|3750}}<syntaxhighlight lang="lua">shuf_list = GetShuffledCopyOfTable(oil_list)</syntaxhighlight>
{{CodeLine5|3751}}<syntaxhighlight lang="lua">iNumLeftToPlace = self:PlaceSpecificNumberOfResources(self.oil_ID, oil_amt, 1, 1, -1, 0, 0, shuf_list);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|3757}}<syntaxhighlight lang="lua">shuf_list = GetShuffledCopyOfTable(iron_fallback)</syntaxhighlight>
{{CodeLine5|3758}}<syntaxhighlight lang="lua">iNumLeftToPlace = self:PlaceSpecificNumberOfResources(self.iron_ID, iron_amt, 1, 1, -1, 0, 0, shuf_list);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|3761}}<syntaxhighlight lang="lua">shuf_list = GetShuffledCopyOfTable(horse_fallback)</syntaxhighlight>
{{CodeLine5|3762}}<syntaxhighlight lang="lua">iNumLeftToPlace = self:PlaceSpecificNumberOfResources(self.horse_ID, horse_amt, 1, 1, -1, 0, 0, shuf_list);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|4181}}<syntaxhighlight lang="lua">randomized_second_ring_adjustments = GetShuffledCopyOfTable(self.secondRingYIsEven);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|4313}}<syntaxhighlight lang="lua">randomized_third_ring_adjustments = GetShuffledCopyOfTable(self.thirdRingYIsEven);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|4715}}<syntaxhighlight lang="lua">local shuffled_coastal_civs = GetShuffledCopyOfTable(civs_needing_coastal_start);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|4719}}<syntaxhighlight lang="lua">shuffled_coastal_regions = GetShuffledCopyOfTable(regions_with_coastal_start);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|4805}}<syntaxhighlight lang="lua">local shuffled_river_civs = GetShuffledCopyOfTable(civs_needing_river_start);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|4808}}<syntaxhighlight lang="lua">shuffled_river_regions = GetShuffledCopyOfTable(regions_with_river_start);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|4811}}<syntaxhighlight lang="lua">shuffled_near_river_regions = GetShuffledCopyOfTable(regions_with_near_river_start);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|6478}}<syntaxhighlight lang="lua">local randomized_inland = GetShuffledCopyOfTable(inland_plot_list);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|7236}}<syntaxhighlight lang="lua">self.coast_next_to_land_list = GetShuffledCopyOfTable(temp_coast_next_to_land_list)</syntaxhighlight>
{{CodeLine5|7237}}<syntaxhighlight lang="lua">self.marsh_list = GetShuffledCopyOfTable(temp_marsh_list)</syntaxhighlight>
{{CodeLine5|7238}}<syntaxhighlight lang="lua">self.flood_plains_list = GetShuffledCopyOfTable(temp_flood_plains_list)</syntaxhighlight>
{{CodeLine5|7239}}<syntaxhighlight lang="lua">self.hills_open_list = GetShuffledCopyOfTable(temp_hills_open_list)</syntaxhighlight>
{{CodeLine5|7240}}<syntaxhighlight lang="lua">self.hills_covered_list = GetShuffledCopyOfTable(temp_hills_covered_list)</syntaxhighlight>
{{CodeLine5|7241}}<syntaxhighlight lang="lua">self.hills_jungle_list = GetShuffledCopyOfTable(temp_hills_jungle_list)</syntaxhighlight>
{{CodeLine5|7242}}<syntaxhighlight lang="lua">self.hills_forest_list = GetShuffledCopyOfTable(temp_hills_forest_list)</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|7246}}<syntaxhighlight lang="lua">self.plains_flat_no_feature = GetShuffledCopyOfTable(temp_plains_flat_no_feature)</syntaxhighlight>
{{CodeLine5|7247}}<syntaxhighlight lang="lua">self.dry_grass_flat_no_feature = GetShuffledCopyOfTable(temp_dry_grass_flat_no_feature)</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|7249}}<syntaxhighlight lang="lua">self.tundra_flat_including_forests = GetShuffledCopyOfTable(temp_tundra_flat_including_forests)</syntaxhighlight>
{{CodeLine5|7250}}<syntaxhighlight lang="lua">self.forest_flat_that_are_not_tundra = GetShuffledCopyOfTable(temp_forest_flat_that_are_not_tundra)</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|7252}}<syntaxhighlight lang="lua">self.grass_flat_no_feature = GetShuffledCopyOfTable(temp_grass_flat_no_feature)</syntaxhighlight>
{{CodeLine5|7253}}<syntaxhighlight lang="lua">self.tundra_flat_no_feature = GetShuffledCopyOfTable(temp_tundra_flat_no_feature)</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|7256}}<syntaxhighlight lang="lua">self.land_list = GetShuffledCopyOfTable(temp_land_list)</syntaxhighlight>
{{CodeLine5|7257}}<syntaxhighlight lang="lua">self.coast_list = GetShuffledCopyOfTable(temp_coast_list)</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|7260}}<syntaxhighlight lang="lua">self.desert_wheat_list = GetShuffledCopyOfTable(temp_desert_wheat_list)</syntaxhighlight>
{{CodeLine5|7261}}<syntaxhighlight lang="lua">self.banana_list = GetShuffledCopyOfTable(temp_banana_list)</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|8548}}<syntaxhighlight lang="lua">shuf_list = GetShuffledCopyOfTable(luxury_plot_lists[primary])</syntaxhighlight>
{{CodeLine5|8549}}<syntaxhighlight lang="lua">iNumLeftToPlace = self:PlaceSpecificNumberOfResources(this_region_luxury, 1, iNumLeftToPlace, 1, -1, 0, 0, shuf_list);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|8551}}<syntaxhighlight lang="lua">shuf_list = GetShuffledCopyOfTable(luxury_plot_lists[secondary])</syntaxhighlight>
{{CodeLine5|8552}}<syntaxhighlight lang="lua">iNumLeftToPlace = self:PlaceSpecificNumberOfResources(this_region_luxury, 1, iNumLeftToPlace, 1, -1, 0, 0, shuf_list);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|8559}}<syntaxhighlight lang="lua">shuf_list = GetShuffledCopyOfTable(luxury_plot_lists[quaternary])</syntaxhighlight>
{{CodeLine5|8560}}<syntaxhighlight lang="lua">iNumLeftToPlace = self:PlaceSpecificNumberOfResources(this_region_luxury, 1, iNumLeftToPlace, 1, -1, 0, 0, shuf_list);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|8581}}<syntaxhighlight lang="lua">shuf_list = GetShuffledCopyOfTable(luxury_plot_lists[secondary])</syntaxhighlight>
{{CodeLine5|8582}}<syntaxhighlight lang="lua">randoms_to_place = self:PlaceSpecificNumberOfResources(random_res, 1, 1, 1, -1, 0, 0, shuf_list);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|8585}}<syntaxhighlight lang="lua">shuf_list = GetShuffledCopyOfTable(luxury_plot_lists[tertiary])</syntaxhighlight>
{{CodeLine5|8586}}<syntaxhighlight lang="lua">randoms_to_place = self:PlaceSpecificNumberOfResources(random_res, 1, 1, 1, -1, 0, 0, shuf_list);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|8589}}<syntaxhighlight lang="lua">shuf_list = GetShuffledCopyOfTable(luxury_plot_lists[quaternary])</syntaxhighlight>
{{CodeLine5|8590}}<syntaxhighlight lang="lua">randoms_to_place = self:PlaceSpecificNumberOfResources(random_res, 1, 1, 1, -1, 0, 0, shuf_list);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|8678}}<syntaxhighlight lang="lua">shuf_list = GetShuffledCopyOfTable(luxury_plot_lists[primary])</syntaxhighlight>
{{CodeLine5|8679}}<syntaxhighlight lang="lua">local iNumLeftToPlace = self:PlaceSpecificNumberOfResources(use_this_ID, 1, 1, 1, -1, 0, 0, shuf_list);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|8685}}<syntaxhighlight lang="lua">shuf_list = GetShuffledCopyOfTable(luxury_plot_lists[tertiary])</syntaxhighlight>
{{CodeLine5|8686}}<syntaxhighlight lang="lua">iNumLeftToPlace = self:PlaceSpecificNumberOfResources(use_this_ID, 1, 1, 1, -1, 0, 0, shuf_list);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|8728}}<syntaxhighlight lang="lua">shuf_list = GetShuffledCopyOfTable(luxury_plot_lists[secondary])</syntaxhighlight>
{{CodeLine5|8729}}<syntaxhighlight lang="lua">iNumLeftToPlace = self:PlaceSpecificNumberOfResources(res_ID, 1, iNumLeftToPlace, 0.3, 2, 0, 3, shuf_list);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|8732}}<syntaxhighlight lang="lua">shuf_list = GetShuffledCopyOfTable(luxury_plot_lists[tertiary])</syntaxhighlight>
{{CodeLine5|8733}}<syntaxhighlight lang="lua">iNumLeftToPlace = self:PlaceSpecificNumberOfResources(res_ID, 1, iNumLeftToPlace, 0.4, 2, 0, 2, shuf_list);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|8736}}<syntaxhighlight lang="lua">shuf_list = GetShuffledCopyOfTable(luxury_plot_lists[quaternary])</syntaxhighlight>
{{CodeLine5|8737}}<syntaxhighlight lang="lua">iNumLeftToPlace = self:PlaceSpecificNumberOfResources(res_ID, 1, iNumLeftToPlace, 0.5, 2, 0, 2, shuf_list);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|9273}}<syntaxhighlight lang="lua">local shuf_list = GetShuffledCopyOfTable(fish_list)</syntaxhighlight>
{{CodeLine5|9274}}<syntaxhighlight lang="lua">local iNumLeftToPlace = self:PlaceSpecificNumberOfResources(self.fish_ID, 1, 1, 1, -1, 0, 0, shuf_list);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|9298}}<syntaxhighlight lang="lua">local shuffled_hills_regions = GetShuffledCopyOfTable(hills_regions)</syntaxhighlight>
{{CodeLine5|9299}}<syntaxhighlight lang="lua">for loop, region_number in ipairs(shuffled_hills_regions) do</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|Europe.lua (G&K)}}
:<code>DLC/Expansion/Maps/Europe.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1157}}<syntaxhighlight lang="lua">local candidate_plot_list = GetShuffledCopyOfTable(self.sinai_list)</syntaxhighlight>
{{CodeLine5|1158}}<syntaxhighlight lang="lua">for loop, plotIndex in ipairs(candidate_plot_list) do</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1215}}<syntaxhighlight lang="lua">local NW_shuffled_order = GetShuffledCopyOfTable(NW_eligibility_order);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|FeatureGenerator.lua (G&K)}}
:<code>DLC/Expansion/Gameplay/Lua/FeatureGenerator.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0418}}<syntaxhighlight lang="lua">local beta_list = GetShuffledCopyOfTable(temp_beta_list)</syntaxhighlight>
{{CodeLine5|0419}}<syntaxhighlight lang="lua">local gamma_list = GetShuffledCopyOfTable(temp_gamma_list)</syntaxhighlight>
{{CodeLine5|0420}}<syntaxhighlight lang="lua">local delta_list = GetShuffledCopyOfTable(temp_delta_list)</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|Hemispheres.lua (G&K)}}
:<code>DLC/Expansion/Maps/Hemispheres.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1149}}<syntaxhighlight lang="lua">local westListShuffled = GetShuffledCopyOfTable(westList)</syntaxhighlight>
{{CodeLine5|1150}}<syntaxhighlight lang="lua">local eastListShuffled = GetShuffledCopyOfTable(eastList)</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|North_vs_South.lua}}
:<code>Maps/North_vs_South.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0622}}<syntaxhighlight lang="lua">local northListShuffled = GetShuffledCopyOfTable(northList)</syntaxhighlight>
{{CodeLine5|0623}}<syntaxhighlight lang="lua">local southListShuffled = GetShuffledCopyOfTable(southList)</syntaxhighlight>
{{CodeLine5|0624}}<syntaxhighlight lang="lua">for region_number, player_ID in ipairs(southListShuffled) do</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|Skirmish.lua}}
:<code>Maps/Skirmish.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0206}}<syntaxhighlight lang="lua">local east_shuffled = GetShuffledCopyOfTable(east_half)</syntaxhighlight>
{{CodeLine5|0207}}<syntaxhighlight lang="lua">local iNumMountainsPerColumn = math.max(math.floor(iH * 0.225), math.floor((iH / 4) - 1));</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1180}}<syntaxhighlight lang="lua">shuf_list = GetShuffledCopyOfTable(luxury_plot_lists[primary])</syntaxhighlight>
{{CodeLine5|1181}}<syntaxhighlight lang="lua">iNumLeftToPlace = self:PlaceSpecificNumberOfResources(res_ID, res_amt, iNumThisLuxToPlace, 0.3, 1, 1, 1, shuf_list);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1199}}<syntaxhighlight lang="lua">shuf_list = GetShuffledCopyOfTable(luxury_plot_lists[secondary])</syntaxhighlight>
{{CodeLine5|1200}}<syntaxhighlight lang="lua">iNumLeftToPlace = self:PlaceSpecificNumberOfResources(res_ID, res_sm, iNumLeftToPlace, 0.3, 1, 0, 0, shuf_list);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1203}}<syntaxhighlight lang="lua">shuf_list = GetShuffledCopyOfTable(luxury_plot_lists[tertiary])</syntaxhighlight>
{{CodeLine5|1204}}<syntaxhighlight lang="lua">iNumLeftToPlace = self:PlaceSpecificNumberOfResources(res_ID, res_sm, iNumLeftToPlace, 0.4, 1, 0, 0, shuf_list);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1207}}<syntaxhighlight lang="lua">shuf_list = GetShuffledCopyOfTable(luxury_plot_lists[quaternary])</syntaxhighlight>
{{CodeLine5|1208}}<syntaxhighlight lang="lua">iNumLeftToPlace = self:PlaceSpecificNumberOfResources(res_ID, res_sm, iNumLeftToPlace, 0.5, 1, 0, 0, shuf_list);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetShuffledCopyOfTable]]