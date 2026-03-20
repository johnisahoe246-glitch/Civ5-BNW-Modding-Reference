{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Player}}.<br/>
This is an instance method, invoke it with a colon.<br/>
}}

Creates a new unit for the calling player. Note: Using this function in a map script may crash WorldBuilder.

=Usage=
<code>{{Type5|Unit}} Player:InitUnit<b>(</b>{{Type5|UnitType}} unit, '''int''' x, '''int''' y, {{Type5|UnitAIType}} unitAI = NO_UNITAI, {{Type5|DirectionType}} facingDirection = NO_DIRECTION<b>)</b></code>

'''Returned Value'''
:Returns a reference to the created unit.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|unit:
|valign="top"| ''The {{Type5|UnitType}} ID of the unit to be created.''
|-
|valign="top" style="padding-right:6px;"|x:
|valign="top"| ''The X coordinate on the map where the unit is to be created.''
|-
|valign="top" style="padding-right:6px;"|y:
|valign="top"| ''The Y coordinate on the map where the unit is to be created.''
|-
|valign="top" style="padding-right:6px;"|unitAI:
|valign="top"| ''Optional. The AI tactics for the unit to use upon being created. If not specified, it will be the default AI for this unit type.''
|-
|valign="top" style="padding-right:6px;"|facingDirection:
|valign="top"| ''Optional. The direction for the newly created unit to be facing. If not specified, it will be random.''
|}


=Source code samples=
''Too many occurences. Only 50 out of 350 are listed.''

{{PseudoH4|TurnsRemaining.lua - DLC_02 DLC}}
:<code>DLC/DLC_02/Scenarios/NewWorldScenario/TurnsRemaining.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0338}}<syntaxhighlight lang="lua">unit = pLoopPlayer:InitUnit (iUnitID, pLoopPlayer:GetStartingPlot():GetX(), pLoopPlayer:GetStartingPlot():GetY());</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0413}}<syntaxhighlight lang="lua">pPlayer:InitUnit (iUnitID, adjacentPlot:GetX(), adjacentPlot:GetY());</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TurnsRemaining.lua - DLC_04 DLC}}
:<code>DLC/DLC_04/Scenarios/1066Scenario/TurnsRemaining.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0515}}<syntaxhighlight lang="lua">unit = player:InitUnit (iUnitID, playerStartPlot:GetX(), playerStartPlot:GetY(), UNITAI_DEFENSE, DirectionTypes.DIRECTION_WEST);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0545}}<syntaxhighlight lang="lua">unit = player:InitUnit (iUnitID, 36, 6, UNITAI_DEFENSE, DirectionTypes.DIRECTION_WEST);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0549}}<syntaxhighlight lang="lua">unit = player:InitUnit (iUnitID, 37, 6, UNITAI_DEFENSE, DirectionTypes.DIRECTION_WEST);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0553}}<syntaxhighlight lang="lua">unit = player:InitUnit (iUnitID, 38, 6, UNITAI_DEFENSE, DirectionTypes.DIRECTION_WEST);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0561}}<syntaxhighlight lang="lua">unit = player:InitUnit (iUnitID, 40, 6, UNITAI_DEFENSE, DirectionTypes.DIRECTION_WEST);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0599}}<syntaxhighlight lang="lua">unit = player:InitUnit (iUnitID, 52, 21, UNITAI_DEFENSE, DirectionTypes.DIRECTION_WEST);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0607}}<syntaxhighlight lang="lua">unit = player:InitUnit (iUnitID, 51, 19, UNITAI_DEFENSE, DirectionTypes.DIRECTION_WEST);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0615}}<syntaxhighlight lang="lua">unit = player:InitUnit (iUnitID, 52, 19, UNITAI_RANGED, DirectionTypes.DIRECTION_WEST);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0623}}<syntaxhighlight lang="lua">unit = player:InitUnit (iUnitID, 53, 21, UNITAI_RANGED, DirectionTypes.DIRECTION_WEST);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0653}}<syntaxhighlight lang="lua">unit = player:InitUnit (iUnitID, 31, 34, UNITAI_DEFENSE, DirectionTypes.DIRECTION_WEST);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0665}}<syntaxhighlight lang="lua">unit = player:InitUnit (iUnitID, 29, 33, UNITAI_RANGED, DirectionTypes.DIRECTION_WEST);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0669}}<syntaxhighlight lang="lua">unit = player:InitUnit (iUnitID, 30, 34, UNITAI_RANGED, DirectionTypes.DIRECTION_WEST);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0693}}<syntaxhighlight lang="lua">unit = player:InitUnit (iUnitID, 50, 11, UNITAI_DEFENSE, DirectionTypes.DIRECTION_WEST);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0701}}<syntaxhighlight lang="lua">unit = player:InitUnit (iUnitID, 51, 13, UNITAI_DEFENSE, DirectionTypes.DIRECTION_WEST);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0713}}<syntaxhighlight lang="lua">unit = player:InitUnit (iUnitID, 51, 11, UNITAI_RANGED, DirectionTypes.DIRECTION_WEST);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TurnsRemaining.lua (G&K)}}
:<code>DLC/Expansion/Scenarios/SteampunkScenario/TurnsRemaining.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0850}}<syntaxhighlight lang="lua">local pUnit = pPlayer:InitUnit(eUnitType, pPlot:GetX(), pPlot:GetY());</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TurnsRemaining.lua (G&K)}}
:<code>DLC/Expansion/Scenarios/FallOfRomeScenario/TurnsRemaining.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0378}}<syntaxhighlight lang="lua">unit = newPlayer:InitUnit(iUnitID, iX, iY);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1309}}<syntaxhighlight lang="lua">unit = pPlayer:InitUnit(GameInfoTypes["UNIT_ROMAN_LEGION"], 20, 47); -- Legion @ Lutetia</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1323}}<syntaxhighlight lang="lua">unit = pPlayer:InitUnit(GameInfoTypes["UNIT_ROMAN_BALLISTA"], 26, 49); -- Ballista @ Trier</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1330}}<syntaxhighlight lang="lua">unit = pPlayer:InitUnit(GameInfoTypes["UNIT_HORSEMAN"], 22, 42); -- Horseman @ Lugundium</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1344}}<syntaxhighlight lang="lua">unit = pPlayer:InitUnit(GameInfoTypes["UNIT_COMPOSITE_BOWMAN"], 49, 34); -- Archer @ Naissus</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1346}}<syntaxhighlight lang="lua">unit = pPlayer:InitUnit(GameInfoTypes["UNIT_COMPOSITE_BOWMAN"], 75, 26); -- Archer @ Melitene</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1352}}<syntaxhighlight lang="lua">unit = pPlayer:InitUnit(GameInfoTypes["UNIT_CATAPULT"], 76, 21); -- Catapult @ Edessa</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1358}}<syntaxhighlight lang="lua">unit = pPlayer:InitUnit(GameInfoTypes["UNIT_ROMAN_LEGION"], 76, 21); -- Legion @ Edessa</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1369}}<syntaxhighlight lang="lua">unit = pPlayer:InitUnit(GameInfoTypes["UNIT_BYZANTINE_CATAPHRACT"], 49, 34); -- Cataphract @ Naissus</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1371}}<syntaxhighlight lang="lua">unit = pPlayer:InitUnit(GameInfoTypes["UNIT_BYZANTINE_CATAPHRACT"], 71, 30); -- Cataphract @ Amasia</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1388}}<syntaxhighlight lang="lua">unit = pPlayer:InitUnit(GameInfoTypes["UNIT_SWORDSMAN"], 81, 33); -- Swordsman @ Anium</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1413}}<syntaxhighlight lang="lua">unit = pPlayer:InitUnit(GameInfoTypes["UNIT_SWORDSMAN"], 79, 24); -- Swordsman @ Amida</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1432}}<syntaxhighlight lang="lua">unit = pPlayer:InitUnit(GameInfoTypes["UNIT_HORSEMAN"], 84, 58); -- Horseman @ Attila's Court -- extra to encourage an attack</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1442}}<syntaxhighlight lang="lua">unit = pPlayer:InitUnit(GameInfoTypes["UNIT_HUN_HORSE_ARCHER"], 84, 58); -- Horse archer @ Attila's Court</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1448}}<syntaxhighlight lang="lua">unit = pPlayer:InitUnit(GameInfoTypes["UNIT_HUN_BATTERING_RAM"], 84, 58); -- battering ram! @ Attila's Court</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1476}}<syntaxhighlight lang="lua">unit = pPlayer:InitUnit(GameInfoTypes["UNIT_COMPOSITE_BOWMAN"], 17, 57); -- Bowman @ mid-country</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1480}}<syntaxhighlight lang="lua">unit = pPlayer:InitUnit(GameInfoTypes["UNIT_CATAPULT"], 17, 57); -- Catapult @ mid-country</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1528}}<syntaxhighlight lang="lua">unit = pPlayer:InitUnit(GameInfoTypes["UNIT_COMPOSITE_BOWMAN"], 32, 54); -- Bowman @ Tongres</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1556}}<syntaxhighlight lang="lua">unit = pPlayer:InitUnit(GameInfoTypes["UNIT_GOTH_GADRAUHT"], 50, 37); -- Gadrauht @ ERE border</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1586}}<syntaxhighlight lang="lua">unit = pPlayer:InitUnit(GameInfoTypes["UNIT_COMPOSITE_BOWMAN"], 4, 19); -- Bowman @ Caput Vada -- added to get army up to city-attacking size</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1592}}<syntaxhighlight lang="lua">unit = pPlayer:InitUnit(GameInfoTypes["UNIT_CARTHAGINIAN_QUINQUEREME"], 4, 19); -- Tri @ Caput Vada</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1594}}<syntaxhighlight lang="lua">unit = pPlayer:InitUnit(GameInfoTypes["UNIT_VANDAL_AXEMAN"], 4, 19); -- Axeman @ Caput Vada</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1600}}<syntaxhighlight lang="lua">unit = pPlayer:InitUnit(GameInfoTypes["UNIT_CATAPULT"], 4, 19); -- Catapult @ Caput Vada</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1816}}<syntaxhighlight lang="lua">unit = pPlayer:InitUnit(GameInfoTypes["UNIT_CATAPULT"], iSpawnX, iSpawnY);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1819}}<syntaxhighlight lang="lua">unit = pPlayer:InitUnit(GameInfoTypes["UNIT_COMPOSITE_BOWMAN"], iSpawnX, iSpawnY);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|2018}}<syntaxhighlight lang="lua">unit = pPlayer:InitUnit(GameInfoTypes["UNIT_CELT_PICTISH_WARRIOR"], iSpawnX, iSpawnY);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|2108}}<syntaxhighlight lang="lua">unit = pPlayer:InitUnit(GameInfoTypes["UNIT_FRANK_SEAXMAN"], iSpawnX, iSpawnY);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TurnsRemaining.lua (G&K)}}
:<code>DLC/Expansion/Scenarios/MedievalScenario/TurnsRemaining.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1064}}<syntaxhighlight lang="lua">unit = pPlayer:InitUnit (iUnitID, capital:GetX(), capital:GetY(), UNITAI_DEFENSE, DirectionTypes.DIRECTION_EAST);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1276}}<syntaxhighlight lang="lua">unit = pPlayer:InitUnit (iUnitID, capital:GetX(), capital:GetY(), UNITAI_WORKER, DirectionTypes.DIRECTION_WEST);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1300}}<syntaxhighlight lang="lua">unit = pPlayer:InitUnit (iUnitID, capital:GetX(), capital:GetY(), UNITAI_GENERAL, DirectionTypes.DIRECTION_WEST);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1612}}<syntaxhighlight lang="lua">unit = pPlayer:InitUnit (iUnitID, capital:GetX(), capital:GetY(), UNITAI_SETTLE, DirectionTypes.DIRECTION_EAST);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|WorldView.lua}}
:<code>UI/InGame/WorldView/WorldView.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0264}}<syntaxhighlight lang="lua">pActivePlayer:InitUnit(iUnitID, plotX, plotY);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|InitUnit]]
[[Category:Civ5 Units API|InitUnit]]