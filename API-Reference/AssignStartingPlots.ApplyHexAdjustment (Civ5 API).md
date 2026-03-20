{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|AssignStartingPlots}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''int''', '''int''' AssignStartingPlots:ApplyHexAdjustment<b>(</b>'''int''' x, '''int''' y, table('''int''' => '''int''') plot_adjustments<b>)</b></code>


'''Returned Values'''
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
|valign="top" style="padding-right:6px;"|plot_adjustments:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|AssignStartingPlots.lua (G&K)}}
:<code>DLC/Expansion/Gameplay/Lua/AssignStartingPlots.lua</code>
:{{CodeBegin5}}
{{CodeLine5|3870}}<syntaxhighlight lang="lua">local searchX, searchY = self:ApplyHexAdjustment(x, y, plot_adjustments)</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|3872}}<syntaxhighlight lang="lua">if searchX < 0 or searchX >= iW or searchY < 0 or searchY >= iH then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|4012}}<syntaxhighlight lang="lua">local searchX, searchY = self:ApplyHexAdjustment(x, y, plot_adjustments)</syntaxhighlight>
{{CodeLine5|4013}}<syntaxhighlight lang="lua">local plot = Map.GetPlot(x, y);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|4160}}<syntaxhighlight lang="lua">local searchX, searchY = self:ApplyHexAdjustment(x, y, plot_adjustments)</syntaxhighlight>
{{CodeLine5|4161}}<syntaxhighlight lang="lua">-- Attempt to place a Hill at the currently chosen plot.</syntaxhighlight>
{{CodeLine5|4162}}<syntaxhighlight lang="lua">local placedHill = self:AttemptToPlaceHillsAtPlot(searchX, searchY);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|4187}}<syntaxhighlight lang="lua">local searchX, searchY = self:ApplyHexAdjustment(x, y, plot_adjustments)</syntaxhighlight>
{{CodeLine5|4188}}<syntaxhighlight lang="lua">-- Attempt to place a Hill at the currently chosen plot.</syntaxhighlight>
{{CodeLine5|4189}}<syntaxhighlight lang="lua">local placedStrategic = self:AttemptToPlaceSmallStrategicAtPlot(searchX, searchY);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|4330}}<syntaxhighlight lang="lua">local searchX, searchY = self:ApplyHexAdjustment(x, y, plot_adjustments)</syntaxhighlight>
{{CodeLine5|4331}}<syntaxhighlight lang="lua">-- Attempt to place a Bonus at the currently chosen plot.</syntaxhighlight>
{{CodeLine5|4332}}<syntaxhighlight lang="lua">local placedBonus, placedOasis = self:AttemptToPlaceBonusResourceAtPlot(searchX, searchY, allow_oasis);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|4418}}<syntaxhighlight lang="lua">local searchX, searchY = self:ApplyHexAdjustment(x, y, plot_adjustments)</syntaxhighlight>
{{CodeLine5|4419}}<syntaxhighlight lang="lua">-- Attempt to place Cows at the currently chosen plot.</syntaxhighlight>
{{CodeLine5|4420}}<syntaxhighlight lang="lua">local placedBonus = self:AttemptToPlaceStoneAtGrassPlot(searchX, searchY);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|4435}}<syntaxhighlight lang="lua">local searchX, searchY = self:ApplyHexAdjustment(x, y, plot_adjustments)</syntaxhighlight>
{{CodeLine5|4436}}<syntaxhighlight lang="lua">-- Attempt to place Stone at the currently chosen plot.</syntaxhighlight>
{{CodeLine5|4437}}<syntaxhighlight lang="lua">local placedBonus = self:AttemptToPlaceStoneAtGrassPlot(searchX, searchY);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|6803}}<syntaxhighlight lang="lua">local searchX, searchY = self:ApplyHexAdjustment(x, y, plot_adjustments)</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|6805}}<syntaxhighlight lang="lua">if searchX < 0 or searchX >= iW or searchY < 0 or searchY >= iH then -- This plot's off the map edge.</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|ApplyHexAdjustment]]