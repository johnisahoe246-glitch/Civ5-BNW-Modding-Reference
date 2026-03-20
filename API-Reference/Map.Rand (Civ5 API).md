{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Map}}.<br/>
This is a static method, invoke it with a dot.<br/>
Generates a random number.
}}


=Usage=
<code>'''int''' Map.Rand<b>(</b>'''int''' maxValues, '''string''' logEntry<b>)</b></code>


'''Returned Value'''
:A random number between 0 and maxValues - 1.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|maxValues:
|valign="top"| ''The number of possible random values to make.''
|-
|valign="top" style="padding-right:6px;"|logEntry:
|valign="top"| ''Not optional, but in what log does this appear? May need to set RandLog = 1 in config.ini.''
|}
'''Wrapper'''<br/>
This is a wrapper function for working with Map.Rand which makes it much easier to use. Returns a random number between lower and upper and including both.
<syntaxhighlight lang="lua" class="civ5-example">
function GetRandom(lower, upper)
	return Map.Rand((upper + 1) - lower, "") + lower
end
</syntaxhighlight>

=Source code samples=
''Too many occurences. Only 50 out of 668 are listed.''

{{PseudoH4|Amazon_XP.lua (G&K)}}
:<code>DLC/Expansion/Maps/Amazon_XP.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1134}}<syntaxhighlight lang="lua">local diceroll = Map.Rand(10000, "Choose resource type - Assign Luxury To Region - Lua");</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1390}}<syntaxhighlight lang="lua">local diceroll = Map.Rand(3, "Resource selection - Place Small Quantities LUA");</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1417}}<syntaxhighlight lang="lua">local strat_radius = Map.Rand(4, "Resource Radius - Place Small Quantities LUA");</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|Arborea.lua (G&K)}}
:<code>DLC/Expansion/Maps/Arborea.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0115}}<syntaxhighlight lang="lua">sea_level = 1 + Map.Rand(3, "Random Sea Level - Lua");</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0529}}<syntaxhighlight lang="lua">local grain_dice = Map.Rand(7, "Continental Grain roll - LUA Continents");</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0535}}<syntaxhighlight lang="lua">local rift_dice = Map.Rand(3, "Rift Grain roll - LUA Continents");</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0679}}<syntaxhighlight lang="lua">age = 1 + Map.Rand(3, "Random World Age - Lua");</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0721}}<syntaxhighlight lang="lua">temp = 1 + Map.Rand(3, "Random Temperature - Lua");</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|AssignStartingPlots.lua (G&K)}}
:<code>DLC/Expansion/Gameplay/Lua/AssignStartingPlots.lua</code>
:{{CodeBegin5}}
{{CodeLine5|4291}}<syntaxhighlight lang="lua">local diceroll = 1 + Map.Rand(iNumConversionCandidates, "Choosing plot to convert to Grass near food-poor Plains start - LUA");</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|4971}}<syntaxhighlight lang="lua">local diceroll = 1 + Map.Rand(table.maxn(candidate_regions), "Choosing from among Candidate Regions for start bias - LUA");</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|7671}}<syntaxhighlight lang="lua">res_addition = Map.Rand(1 + (max_radius - min_radius), "Resource Radius - Place Resource LUA");</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|Boreal.lua (G&K)}}
:<code>DLC/Expansion/Maps/Boreal.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0532}}<syntaxhighlight lang="lua">x_target = math.floor(iW / 5 + Map.Rand((iW * 0.6), "River Target - Lua"));</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|Europe.lua (G&K)}}
:<code>DLC/Expansion/Maps/Europe.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0074}}<syntaxhighlight lang="lua">west_edge[y] = math.ceil(iW * 0.08) - 1 + Map.Rand(4, "Roughen coastline - Mediterranean LUA");</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|FeatureGenerator.lua (G&K)}}
:<code>DLC/Expansion/Gameplay/Lua/FeatureGenerator.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0340}}<syntaxhighlight lang="lua">local atoll_number = atoll_target + Map.Rand(atoll_target, "Number of Atolls to place - LUA");</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0435}}<syntaxhighlight lang="lua">local diceroll = 1 + Map.Rand(100, "Atoll Placement Type - LUA");</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|FractalWorld.lua}}
:<code>Gameplay/Lua/FractalWorld.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0341}}<syntaxhighlight lang="lua">local segmentLength = Map.Rand(primaryMaxLength + 1, "FractalWorld Center Rift Segment Length - Lua");</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0346}}<syntaxhighlight lang="lua">local dice = Map.Rand(2, "FractalWorld Center Rift Direction - Lua");</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|Great_Plains.lua}}
:<code>Maps/Great_Plains.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0179}}<syntaxhighlight lang="lua">rightSeed = Map.Rand(5, "Ozarks Shape - Great Plains Lua");</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0517}}<syntaxhighlight lang="lua">if Map.Rand(100, "Add Oasis Lua") <= 5 then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|Hemispheres.lua (G&K)}}
:<code>DLC/Expansion/Maps/Hemispheres.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0172}}<syntaxhighlight lang="lua">island_setting = 1 + Map.Rand(4, "Random Temperature - Lua");</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0389}}<syntaxhighlight lang="lua">local x_shrinkage = Map.Rand(8, "Cell Width adjustment - Lua");</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0435}}<syntaxhighlight lang="lua">local die_1 = Map.Rand(4, "Diceroll - Lua");</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0547}}<syntaxhighlight lang="lua">local y_shrinkage = Map.Rand(9, "Cell Height adjustment - Lua");</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0561}}<syntaxhighlight lang="lua">fTilt = 70 + Map.Rand(41, "Angle for island chain axis - LUA");</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0580}}<syntaxhighlight lang="lua">local iInnerSouth2 = iCellHeight + 2 + Map.Rand(iCellHeight - 3, "Shift for sub island group - Lua");</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0615}}<syntaxhighlight lang="lua">local iInnerWest1 = 3 + Map.Rand(iCellWidth - 2, "Shift for sub island group - Lua");</syntaxhighlight>
{{CodeLine5|0616}}<syntaxhighlight lang="lua">local iInnerSouth1 = 3 + Map.Rand(iCellHeight - 2, "Shift for sub island group - Lua");</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0683}}<syntaxhighlight lang="lua">local iInnerWest2 = 4 + Map.Rand(iCellWidth + 2, "Shift for sub island group - Lua");</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0687}}<syntaxhighlight lang="lua">local die_2 = Map.Rand(7, "Diceroll - Lua");</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|Highlands.lua}}
:<code>Maps/Highlands.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0093}}<syntaxhighlight lang="lua">local shiftRoll = Map.Rand(2, "North or South climate shift - Highlands LUA");</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0127}}<syntaxhighlight lang="lua">userInputLakes = 1 + Map.Rand(3, "Highlands Random Lake Size - Lua");</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|IslandMaker.lua}}
:<code>Gameplay/Lua/IslandMaker.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0136}}<syntaxhighlight lang="lua">local diceroll = Map.Rand(5, "Island Making - Lua");</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0202}}<syntaxhighlight lang="lua">local randomX = westX + Map.Rand(iInnerWidth, "Random X coord for Dot - Lua");</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0259}}<syntaxhighlight lang="lua">local randomY = iInnerSouth2 + Map.Rand(iInnerHeight2, "Random Y coord for Dot - Lua");</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|MapGenerator.lua (G&K)}}
:<code>DLC/Expansion/Gameplay/Lua/MapGenerator.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0207}}<syntaxhighlight lang="lua">if(plot:IsAdjacentToShallowWater() and Map.Rand(iExpansionDiceroll, "add shallows") == 0) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|MapmakerUtilities.lua}}
:<code>Gameplay/Lua/MapmakerUtilities.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0563}}<syntaxhighlight lang="lua">local random_index = 1 + Map.Rand(left_to_do, "Shuffling table entry - Lua");</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|MultilayeredFractal.lua (G&K)}}
:<code>DLC/Expansion/Gameplay/Lua/MultilayeredFractal.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0866}}<syntaxhighlight lang="lua">local scRoll = Map.Rand((regiononeWidth - scLargeWidth), "Large Subcontinent Placement - Map_Script_Name LUA");</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|Ring.lua}}
:<code>Maps/Ring.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0132}}<syntaxhighlight lang="lua">dominant_terrain = 1 + Map.Rand(4, "Random Type of Dominant Terrain - Ring LUA");</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0140}}<syntaxhighlight lang="lua">bridge_width = 2 + Map.Rand(3, "Random Bridge Width - Ring LUA");</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|Shuffle.lua (G&K)}}
:<code>DLC/Expansion/Maps/Shuffle.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0076}}<syntaxhighlight lang="lua">local world_age =  1 + Map.Rand(3, "Random World Age - Lua");</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0581}}<syntaxhighlight lang="lua">userInputLandmass = 1 + Map.Rand(4, "Random Landmass Type - Lua");</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0668}}<syntaxhighlight lang="lua">local rain = 1 + Map.Rand(3, "Random Rainfall - Lua");</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|Skirmish.lua}}
:<code>Maps/Skirmish.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0355}}<syntaxhighlight lang="lua">local random_factor = Map.Rand(3, "River direction random factor - Skirmish LUA");</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|Terra.lua}}
:<code>Maps/Terra.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0083}}<syntaxhighlight lang="lua">local roll1 = Map.Rand(2, "Eurasian Hemisphere N/S - Terra Lua");</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0329}}<syntaxhighlight lang="lua">local nwcRoll = Map.Rand(2, "Central America and Carribean Placement - Terra Lua");</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0432}}<syntaxhighlight lang="lua">local scsRoll = Map.Rand((eurasiaWidth - scSmallWidth), "Small Subcontinent Placement - Terra Lua");</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0477}}<syntaxhighlight lang="lua">local extras = 2 + Map.Rand(3, "Number of Minor Regions - Terra Lua");</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0483}}<syntaxhighlight lang="lua">local twRoll = Map.Rand((eurasiaWidth - twWidth), "Minor Region Placement - Terra Lua");</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|WorldBuilderRandomItems.lua}}
:<code>Gameplay/Lua/WorldBuilderRandomItems.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0018}}<syntaxhighlight lang="lua">local rand1 = Map.Rand(resource.RandApp1, "MapGenerator CalculateNumResourcesToAdd-1");</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0021}}<syntaxhighlight lang="lua">local rand4 = Map.Rand(resource.RandApp4, "MapGenerator CalculateNumResourcesToAdd-4");</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|Rand]]