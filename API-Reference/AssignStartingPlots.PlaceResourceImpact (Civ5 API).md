{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|AssignStartingPlots}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''void''' AssignStartingPlots:PlaceResourceImpact<b>(</b>'''int''' x, '''int''' y, '''int''' impact_table_number, '''int''' radius<b>)</b></code>


'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|x:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|y:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|impact_table_number:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|radius:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Too many occurences. Only 50 out of 176 are listed.''

{{PseudoH4|Amazon_XP.lua (G&K)}}
:<code>DLC/Expansion/Maps/Amazon_XP.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1422}}<syntaxhighlight lang="lua">self:PlaceResourceImpact(x, y, 1, strat_radius);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|AssignStartingPlots.lua}}
:<code>Gameplay/Lua/AssignStartingPlots.lua</code>
:{{CodeBegin5}}
{{CodeLine5|5648}}<syntaxhighlight lang="lua">self:PlaceResourceImpact(x, y, 6, math.floor(iH / 5))   -- Natural Wonders layer</syntaxhighlight>
{{CodeLine5|5649}}<syntaxhighlight lang="lua">self:PlaceResourceImpact(x, y, 1, 0)               -- Strategic layer</syntaxhighlight>
{{CodeLine5|5650}}<syntaxhighlight lang="lua">self:PlaceResourceImpact(x, y, 2, 0)               -- Luxury layer</syntaxhighlight>
{{CodeLine5|5651}}<syntaxhighlight lang="lua">self:PlaceResourceImpact(x, y, 3, 0)               -- Bonus layer</syntaxhighlight>
{{CodeLine5|5652}}<syntaxhighlight lang="lua">self:PlaceResourceImpact(x, y, 5, 0)               -- City State layer</syntaxhighlight>
{{CodeLine5|5653}}<syntaxhighlight lang="lua">self:PlaceResourceImpact(x, y, 7, 1)               -- Marble layer</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|5765}}<syntaxhighlight lang="lua">self:PlaceResourceImpact(x, y, 3, 1)               -- Bonus layer</syntaxhighlight>
{{CodeLine5|5766}}<syntaxhighlight lang="lua">self:PlaceResourceImpact(x, y, 4, 1)               -- Fish layer</syntaxhighlight>
{{CodeLine5|5767}}<syntaxhighlight lang="lua">self:PlaceResourceImpact(x, y, 5, 1)               -- City State layer</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|AssignStartingPlots.lua (G&K)}}
:<code>DLC/Expansion/Gameplay/Lua/AssignStartingPlots.lua</code>
:{{CodeBegin5}}
{{CodeLine5|2113}}<syntaxhighlight lang="lua">self:PlaceResourceImpact(x, y, 1, 0) -- Strategic layer, at impact site only.</syntaxhighlight>
{{CodeLine5|2114}}<syntaxhighlight lang="lua">self:PlaceResourceImpact(x, y, 2, 3) -- Luxury layer, set all plots within this civ start as off limits.</syntaxhighlight>
{{CodeLine5|2115}}<syntaxhighlight lang="lua">self:PlaceResourceImpact(x, y, 3, 3) -- Bonus layer</syntaxhighlight>
{{CodeLine5|2116}}<syntaxhighlight lang="lua">self:PlaceResourceImpact(x, y, 4, 3) -- Fish layer</syntaxhighlight>
{{CodeLine5|2117}}<syntaxhighlight lang="lua">self:PlaceResourceImpact(x, y, 6, 4) -- Natural Wonders layer, set a minimum distance of 5 plots (4 ripples) away.</syntaxhighlight>
{{CodeLine5|2118}}<syntaxhighlight lang="lua">-- Now the main data layer, for start points themselves, and the City State data layer.</syntaxhighlight>
{{CodeLine5|2119}}<syntaxhighlight lang="lua">-- Place Impact!</syntaxhighlight>
{{CodeLine5|2120}}<syntaxhighlight lang="lua">local impactPlotIndex = y * iW + x + 1;</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|4297}}<syntaxhighlight lang="lua">self:PlaceResourceImpact(conv_x, conv_y, 1, 0) -- Disallow strategic resources at this plot, to keep it a farm plot.</syntaxhighlight>
{{CodeLine5|4298}}<syntaxhighlight lang="lua">end</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|5974}}<syntaxhighlight lang="lua">self:PlaceResourceImpact(x, y, 6, math.floor(iH / 5))   -- Natural Wonders layer</syntaxhighlight>
{{CodeLine5|5975}}<syntaxhighlight lang="lua">self:PlaceResourceImpact(x, y, 1, 1)               -- Strategic layer</syntaxhighlight>
{{CodeLine5|5976}}<syntaxhighlight lang="lua">self:PlaceResourceImpact(x, y, 2, 1)               -- Luxury layer</syntaxhighlight>
{{CodeLine5|5977}}<syntaxhighlight lang="lua">self:PlaceResourceImpact(x, y, 3, 1)               -- Bonus layer</syntaxhighlight>
{{CodeLine5|5978}}<syntaxhighlight lang="lua">self:PlaceResourceImpact(x, y, 5, 1)               -- City State layer</syntaxhighlight>
{{CodeLine5|5979}}<syntaxhighlight lang="lua">self:PlaceResourceImpact(x, y, 7, 1)               -- Marble layer</syntaxhighlight>
{{CodeLine5|5980}}<syntaxhighlight lang="lua">local plotIndex = y * iW + x + 1;</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|6632}}<syntaxhighlight lang="lua">self:PlaceResourceImpact(x, y, 5, 4) -- City State layer</syntaxhighlight>
{{CodeLine5|6633}}<syntaxhighlight lang="lua">self:PlaceResourceImpact(x, y, 2, 3) -- Luxury layer</syntaxhighlight>
{{CodeLine5|6634}}<syntaxhighlight lang="lua">self:PlaceResourceImpact(x, y, 1, 0) -- Strategic layer, at start point only.</syntaxhighlight>
{{CodeLine5|6635}}<syntaxhighlight lang="lua">self:PlaceResourceImpact(x, y, 3, 3) -- Bonus layer</syntaxhighlight>
{{CodeLine5|6636}}<syntaxhighlight lang="lua">self:PlaceResourceImpact(x, y, 4, 3) -- Fish layer</syntaxhighlight>
{{CodeLine5|6637}}<syntaxhighlight lang="lua">self:PlaceResourceImpact(x, y, 7, 3) -- Marble layer</syntaxhighlight>
{{CodeLine5|6638}}<syntaxhighlight lang="lua">local impactPlotIndex = y * iW + x + 1;</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|6687}}<syntaxhighlight lang="lua">self:PlaceResourceImpact(cs_x, cs_y, 5, 4) -- City State layer</syntaxhighlight>
{{CodeLine5|6688}}<syntaxhighlight lang="lua">self:PlaceResourceImpact(cs_x, cs_y, 2, 3) -- Luxury layer</syntaxhighlight>
{{CodeLine5|6689}}<syntaxhighlight lang="lua">self:PlaceResourceImpact(cs_x, cs_y, 1, 0) -- Strategic layer, at start point only.</syntaxhighlight>
{{CodeLine5|6690}}<syntaxhighlight lang="lua">self:PlaceResourceImpact(cs_x, cs_y, 3, 3) -- Bonus layer</syntaxhighlight>
{{CodeLine5|6691}}<syntaxhighlight lang="lua">self:PlaceResourceImpact(cs_x, cs_y, 4, 3) -- Fish layer</syntaxhighlight>
{{CodeLine5|6692}}<syntaxhighlight lang="lua">self:PlaceResourceImpact(cs_x, cs_y, 7, 3) -- Marble layer</syntaxhighlight>
{{CodeLine5|6693}}<syntaxhighlight lang="lua">local impactPlotIndex = cs_y * iW + cs_x + 1;</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|7510}}<syntaxhighlight lang="lua">self:PlaceResourceImpact(x, y, impact_table_number, res_min[use_this_res_index] + res_addition);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|7674}}<syntaxhighlight lang="lua">self:PlaceResourceImpact(x, y, impact_table_number, rad)</syntaxhighlight>
{{CodeLine5|7675}}<syntaxhighlight lang="lua">end</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|8936}}<syntaxhighlight lang="lua">self:PlaceResourceImpact(x, y, 2, 1)</syntaxhighlight>
{{CodeLine5|8937}}<syntaxhighlight lang="lua">self:PlaceResourceImpact(x, y, 7, 6)</syntaxhighlight>
{{CodeLine5|8938}}<syntaxhighlight lang="lua">break</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|9147}}<syntaxhighlight lang="lua">self:PlaceResourceImpact(x, y, 4, fish_radius);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|Europe_Scenario.lua (G&K)}}
:<code>DLC/Expansion/Scenarios/MedievalScenario/Europe_Scenario.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1730}}<syntaxhighlight lang="lua">self:PlaceResourceImpact(x, y, 5, 3) -- City State layer *** Custom for Europe Scenario, down from 4 ***</syntaxhighlight>
{{CodeLine5|1731}}<syntaxhighlight lang="lua">self:PlaceResourceImpact(x, y, 2, 3) -- Luxury layer</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|PlaceResourceImpact]]
[[Category:Civ5 Resources API|PlaceResourceImpact]]