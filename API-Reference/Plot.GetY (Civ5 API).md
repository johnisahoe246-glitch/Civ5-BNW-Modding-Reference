{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Plot}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''int''' Plot:GetY<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
''Too many occurences. Only 50 out of 350 are listed.''

{{PseudoH4|Amazon_XP.lua (G&K)}}
:<code>DLC/Expansion/Maps/Amazon_XP.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0478}}<syntaxhighlight lang="lua">local adjacentPlot = Map.PlotDirection(riverPlot:GetX(), riverPlot:GetY(), DirectionTypes.DIRECTION_SOUTHWEST);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0544}}<syntaxhighlight lang="lua">local adjacentPlot = Map.PlotDirection(plot:GetX(), plot:GetY(), direction);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0591}}<syntaxhighlight lang="lua">local adjacentPlot = Map.PlotDirection(riverPlot:GetX(), riverPlot:GetY(), DirectionTypes.DIRECTION_SOUTHEAST);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0602}}<syntaxhighlight lang="lua">riverPlot = Map.PlotDirection(startPlot:GetX(), startPlot:GetY(), DirectionTypes.DIRECTION_EAST);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0655}}<syntaxhighlight lang="lua">riverPlot = Map.PlotDirection(riverPlot:GetX(), riverPlot:GetY(), DirectionTypes.DIRECTION_WEST);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0844}}<syntaxhighlight lang="lua">local current_y = plot:GetY()</syntaxhighlight>
{{CodeLine5|0845}}<syntaxhighlight lang="lua">if current_x < 1 or current_x >= iW - 2 or current_y < 2 or current_y >= iH - 1 then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0856}}<syntaxhighlight lang="lua">local start_y = inlandCorner:GetY()</syntaxhighlight>
{{CodeLine5|0857}}<syntaxhighlight lang="lua">if start_x + start_y <= iH * 0.36 then -- Ocean side of Andes</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|Boreal.lua (G&K)}}
:<code>DLC/Expansion/Maps/Boreal.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0227}}<syntaxhighlight lang="lua">local y = plot:GetY()</syntaxhighlight>
{{CodeLine5|0228}}<syntaxhighlight lang="lua">local random_factor = Map.Rand(3, "River direction random factor - Boreal LUA");</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CityStateDiploPopup.lua}}
:<code>UI/InGame/Popups/CityStateDiploPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0306}}<syntaxhighlight lang="lua">local plotY = pTargetPlot:GetY();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CityStateDiploPopup.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/Popups/CityStateDiploPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0614}}<syntaxhighlight lang="lua">local hex = ToHexFromGrid(Vector2(pPlot:GetX(), pPlot:GetY()));</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CityView.lua}}
:<code>UI/InGame/CityView/CityView.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1824}}<syntaxhighlight lang="lua">Events.SerialEventHexHighlight( ToHexFromGrid( Vector2( plot:GetX(), plot:GetY() ) ), false, Vector4( 0.0, 1.0, 0.0, 1 ) );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1838}}<syntaxhighlight lang="lua">if (pCity:CanBuyPlotAt(plot:GetX(), plot:GetY(), false)) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1841}}<syntaxhighlight lang="lua">local iPlotCost = pCity:GetBuyPlotCost( plot:GetX(), plot:GetY() );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1848}}<syntaxhighlight lang="lua">elseif (pCity:CanBuyPlotAt(plot:GetX(), plot:GetY(), true)) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|EnemyUnitPanel.lua}}
:<code>UI/InGame/WorldView/EnemyUnitPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0611}}<syntaxhighlight lang="lua">local pFireSupportUnit = pMyUnit:GetFireSupportUnit(pTheirUnit:GetOwner(), pToPlot:GetX(), pToPlot:GetY());</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|Great_Plains.lua}}
:<code>Maps/Great_Plains.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0561}}<syntaxhighlight lang="lua">local y = plot:GetY()</syntaxhighlight>
{{CodeLine5|0562}}<syntaxhighlight lang="lua">local center = math.floor((iW - 1) * (0.84 + (((iH - y) / iH) * 0.08)));</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|InGame.lua}}
:<code>UI/InGame/InGame.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0459}}<syntaxhighlight lang="lua">local evalPlotY = evalPlot:GetY();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0489}}<syntaxhighlight lang="lua">local hexID = ToHexFromGrid( Vector2( adjacentPlot:GetX(), adjacentPlot:GetY() ) );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|InGame.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/InGame.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0272}}<syntaxhighlight lang="lua">local iPlotY = pPlot:GetY();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|InlandSea.lua}}
:<code>Maps/InlandSea.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0168}}<syntaxhighlight lang="lua">local y = plot:GetY()</syntaxhighlight>
{{CodeLine5|0169}}<syntaxhighlight lang="lua">local random_factor = Map.Rand(3, "River direction random factor - Inland Sea LUA");</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|MapmakerUtilities.lua}}
:<code>Gameplay/Lua/MapmakerUtilities.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0382}}<syntaxhighlight lang="lua">local adjY = NEPlot:GetY();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0392}}<syntaxhighlight lang="lua">local adjY = EPlot:GetY();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0401}}<syntaxhighlight lang="lua">local adjY = SEPlot:GetY();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0410}}<syntaxhighlight lang="lua">local adjY = SWPlot:GetY();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|NaturalWondersCustomMethods.lua (G&K)}}
:<code>DLC/Expansion/Gameplay/Lua/NaturalWondersCustomMethods.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0040}}<syntaxhighlight lang="lua">local southeastY = SEPlot:GetY();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|PlotHelpText.lua}}
:<code>UI/InGame/WorldView/PlotHelpText.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0060}}<syntaxhighlight lang="lua">TextString = TextString .. tostring(plot:GetY());</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|PlotMouseoverInclude.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/PlotMouseoverInclude.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0018}}<syntaxhighlight lang="lua">if (iQuestData1 == plot:GetX() and iQuestData2 == plot:GetY()) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|Skirmish.lua}}
:<code>Maps/Skirmish.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0354}}<syntaxhighlight lang="lua">local y = plot:GetY()</syntaxhighlight>
{{CodeLine5|0355}}<syntaxhighlight lang="lua">local random_factor = Map.Rand(3, "River direction random factor - Skirmish LUA");</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TurnsRemaining.lua - DLC_02 DLC}}
:<code>DLC/DLC_02/Scenarios/NewWorldScenario/TurnsRemaining.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0338}}<syntaxhighlight lang="lua">unit = pLoopPlayer:InitUnit (iUnitID, pLoopPlayer:GetStartingPlot():GetX(), pLoopPlayer:GetStartingPlot():GetY());</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0401}}<syntaxhighlight lang="lua">local adjacentPlot = Map.PlotDirection(pPlot:GetX(), pPlot:GetY(), direction);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0413}}<syntaxhighlight lang="lua">pPlayer:InitUnit (iUnitID, adjacentPlot:GetX(), adjacentPlot:GetY());</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TurnsRemaining.lua - DLC_04 DLC}}
:<code>DLC/DLC_04/Scenarios/1066Scenario/TurnsRemaining.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0244}}<syntaxhighlight lang="lua">if (playerStartPlot:GetX() == 43 and playerStartPlot:GetY() == 17) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0286}}<syntaxhighlight lang="lua">if (playerStartPlot:GetX() == 60 and playerStartPlot:GetY() == 76) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0353}}<syntaxhighlight lang="lua">if (playerStartPlot:GetX() == 59 and playerStartPlot:GetY() == 39) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0518}}<syntaxhighlight lang="lua">unit = player:InitUnit (iUnitID, playerStartPlot:GetX(), playerStartPlot:GetY(), UNITAI_RANGED, DirectionTypes.DIRECTION_WEST);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TurnsRemaining.lua (G&K)}}
:<code>DLC/Expansion/Scenarios/MedievalScenario/TurnsRemaining.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0818}}<syntaxhighlight lang="lua">SetPersistentProperty("JerusalemY", pJerusalemPlot:GetY());</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1036}}<syntaxhighlight lang="lua">print ("Team: ", iTeam, "; Revealing x: ", pPlot:GetX(), ", y: ", pPlot:GetY());</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1042}}<syntaxhighlight lang="lua">local adjPlot = Map.PlotDirection(pPlot:GetX(), pPlot:GetY(), direction);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1070}}<syntaxhighlight lang="lua">local capital = pPlayer:InitCity(startPlot:GetX(), startPlot:GetY());</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1125}}<syntaxhighlight lang="lua">local cityState = pPlayer:InitCity(startPlot:GetX(), startPlot:GetY());</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1147}}<syntaxhighlight lang="lua">SetZurichLocation(startPlot:GetX(), startPlot:GetY());</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1150}}<syntaxhighlight lang="lua">SetGenevaLocation(startPlot:GetX(), startPlot:GetY());</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1153}}<syntaxhighlight lang="lua">SetVaticanLocation(startPlot:GetX(), startPlot:GetY());</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1239}}<syntaxhighlight lang="lua">local capital = pPlayer:InitCity(start_plot:GetX(), start_plot:GetY());</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TurnsRemaining.lua (G&K)}}
:<code>DLC/Expansion/Scenarios/FallOfRomeScenario/TurnsRemaining.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0101}}<syntaxhighlight lang="lua">local iPlotY = playerStartPlot:GetY();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TurnsRemaining.lua (G&K)}}
:<code>DLC/Expansion/Scenarios/SteampunkScenario/TurnsRemaining.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0850}}<syntaxhighlight lang="lua">local pUnit = pPlayer:InitUnit(eUnitType, pPlot:GetX(), pPlot:GetY());</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TutorialChecks.lua}}
:<code>Tutorial/TutorialChecks.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1560}}<syntaxhighlight lang="lua">if (Map.PlotDistance(pFirstUnitPlot:GetX(), pFirstUnitPlot:GetY(), pSecondUnitPlot:GetX(), pSecondUnitPlot:GetY()) <= iMovesLeft ) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|UnitFlagManager.lua}}
:<code>UI/InGame/UnitFlagManager.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1039}}<syntaxhighlight lang="lua">g_CityFlags[ pPlot:GetX() .. " " .. pPlot:GetY() ] = cityFlagInstance;</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|WorldBuilderRandomItems.lua}}
:<code>Gameplay/Lua/WorldBuilderRandomItems.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0180}}<syntaxhighlight lang="lua">local otherPlot   = Map.PlotXYWithRangeCheck(plot:GetX(), plot:GetY(), dx, dy, groupRange);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|WorldView.lua}}
:<code>UI/InGame/WorldView/WorldView.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0162}}<syntaxhighlight lang="lua">local unit = player:InitUnit(g_UnitPlopper.UnitType, plot:GetX(), plot:GetY());</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetY]]