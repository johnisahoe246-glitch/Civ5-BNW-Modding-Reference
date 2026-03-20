{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|AssignStartingPlots}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''int''', '''int''', '''bool''' AssignStartingPlots:PlaceCityState<b>(</b>table('''int''' => '''int''') coastal_plot_list, table('''int''' => '''int''') inland_plot_list, '''bool''' check_proximity, '''bool''' check_collision<b>)</b></code>


'''Returned Values'''
:No description available.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|coastal_plot_list:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|inland_plot_list:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|check_proximity:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|check_collision:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|AssignStartingPlots.lua (G&K)}}
:<code>DLC/Expansion/Gameplay/Lua/AssignStartingPlots.lua</code>
:{{CodeBegin5}}
{{CodeLine5|6520}}<syntaxhighlight lang="lua">x, y, placed_city_state = self:PlaceCityState(eligible_coastal, eligible_inland, false, false) -- Don't need to re-check collisions.</syntaxhighlight>
{{CodeLine5|6521}}<syntaxhighlight lang="lua">end</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|6666}}<syntaxhighlight lang="lua">cs_x, cs_y, success = self:PlaceCityState(self.uninhabited_areas_coastal_plots, self.uninhabited_areas_inland_plots, true, true)</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|6668}}<syntaxhighlight lang="lua">-- Disabling fallback methods that remove proximity and collision checks. Jon has decided</syntaxhighlight>
{{CodeLine5|6669}}<syntaxhighlight lang="lua">-- that city states that do not fit on the map will simply not be placed, but instead discarded.</syntaxhighlight>
{{CodeLine5|6670}}<syntaxhighlight lang="lua">--[[</syntaxhighlight>
{{CodeLine5|6671}}<syntaxhighlight lang="lua">if not success then -- Try again, this time with proximity checks disabled.</syntaxhighlight>
{{CodeLine5|6672}}<syntaxhighlight lang="lua">cs_x, cs_y, success = self:PlaceCityState(self.uninhabited_areas_coastal_plots, self.uninhabited_areas_inland_plots, false, true)</syntaxhighlight>
{{CodeLine5|6673}}<syntaxhighlight lang="lua">if not success then -- Try a third time, this time with all collision checks disabled.</syntaxhighlight>
{{CodeLine5|6674}}<syntaxhighlight lang="lua">cs_x, cs_y, success = self:PlaceCityState(self.uninhabited_areas_coastal_plots, self.uninhabited_areas_inland_plots, false, false)</syntaxhighlight>
{{CodeLine5|6675}}<syntaxhighlight lang="lua">end</syntaxhighlight>
{{CodeLine5|6676}}<syntaxhighlight lang="lua">end</syntaxhighlight>
{{CodeLine5|6677}}<syntaxhighlight lang="lua">]]--</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|6679}}<syntaxhighlight lang="lua">if success == true then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|6738}}<syntaxhighlight lang="lua">cs_x, cs_y, success = self:PlaceCityState(last_chance_shuffled, {}, true, true)</syntaxhighlight>
{{CodeLine5|6739}}<syntaxhighlight lang="lua">if success == true then</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|PlaceCityState]]
[[Category:Civ5 Cities API|PlaceCityState]]