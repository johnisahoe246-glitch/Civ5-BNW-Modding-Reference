{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Plot}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''int''' Plot:GetX<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
''Too many occurences. Only 50 out of 364 are listed.''

{{PseudoH4|ActionInfoPanel.lua}}
:<code>UI/InGame/WorldView/ActionInfoPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0110}}<syntaxhighlight lang="lua">local hex = ToHexFromGrid( Vector2(pPlot:GetX(), pPlot:GetY() ) );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|Amazon_XP.lua (G&K)}}
:<code>DLC/Expansion/Maps/Amazon_XP.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0490}}<syntaxhighlight lang="lua">local adjacentPlot = Map.PlotDirection(riverPlot:GetX(), riverPlot:GetY(), DirectionTypes.DIRECTION_EAST);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0544}}<syntaxhighlight lang="lua">local adjacentPlot = Map.PlotDirection(plot:GetX(), plot:GetY(), direction);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0586}}<syntaxhighlight lang="lua">riverPlot = Map.PlotDirection(riverPlot:GetX(), riverPlot:GetY(), DirectionTypes.DIRECTION_NORTHEAST);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0591}}<syntaxhighlight lang="lua">local adjacentPlot = Map.PlotDirection(riverPlot:GetX(), riverPlot:GetY(), DirectionTypes.DIRECTION_SOUTHEAST);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0602}}<syntaxhighlight lang="lua">riverPlot = Map.PlotDirection(startPlot:GetX(), startPlot:GetY(), DirectionTypes.DIRECTION_EAST);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0618}}<syntaxhighlight lang="lua">riverPlot = Map.PlotDirection(startPlot:GetX(), startPlot:GetY(), DirectionTypes.DIRECTION_SOUTHWEST);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0668}}<syntaxhighlight lang="lua">local riverPlotX = riverPlot:GetX();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0843}}<syntaxhighlight lang="lua">local current_x = plot:GetX()</syntaxhighlight>
{{CodeLine5|0844}}<syntaxhighlight lang="lua">local current_y = plot:GetY()</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0855}}<syntaxhighlight lang="lua">local start_x = inlandCorner:GetX()</syntaxhighlight>
{{CodeLine5|0856}}<syntaxhighlight lang="lua">local start_y = inlandCorner:GetY()</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|AssignStartingPlots.lua (G&K)}}
:<code>DLC/Expansion/Gameplay/Lua/AssignStartingPlots.lua</code>
:{{CodeBegin5}}
{{CodeLine5|5198}}<syntaxhighlight lang="lua">local adjX = adjPlot:GetX();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CityStateDiploPopup.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/Popups/CityStateDiploPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0614}}<syntaxhighlight lang="lua">local hex = ToHexFromGrid(Vector2(pPlot:GetX(), pPlot:GetY()));</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CityView.lua}}
:<code>UI/InGame/CityView/CityView.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1696}}<syntaxhighlight lang="lua">local plotX = plot:GetX();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1729}}<syntaxhighlight lang="lua">local hexPos = ToHexFromGrid( Vector2( plot:GetX(), plot:GetY() ) );</syntaxhighlight>
{{CodeBreak5}}
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


{{PseudoH4|FractalWorld.lua}}
:<code>Gameplay/Lua/FractalWorld.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0330}}<syntaxhighlight lang="lua">currentX = nextPlot:GetX();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|InGame.lua}}
:<code>UI/InGame/InGame.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0458}}<syntaxhighlight lang="lua">local evalPlotX = evalPlot:GetX();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|InGame.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/InGame.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0271}}<syntaxhighlight lang="lua">local iPlotX = pPlot:GetX();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|MapmakerUtilities.lua}}
:<code>Gameplay/Lua/MapmakerUtilities.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0381}}<syntaxhighlight lang="lua">local adjX = NEPlot:GetX();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0409}}<syntaxhighlight lang="lua">local adjX = SWPlot:GetX();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0418}}<syntaxhighlight lang="lua">local adjX = WPlot:GetX();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0427}}<syntaxhighlight lang="lua">local adjX = NWPlot:GetX();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|PlotHelpText.lua}}
:<code>UI/InGame/WorldView/PlotHelpText.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0058}}<syntaxhighlight lang="lua">TextString = TextString .. tostring(plot:GetX());</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|PlotMouseoverInclude.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/PlotMouseoverInclude.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0018}}<syntaxhighlight lang="lua">if (iQuestData1 == plot:GetX() and iQuestData2 == plot:GetY()) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TurnsRemaining.lua - DLC_02 DLC}}
:<code>DLC/DLC_02/Scenarios/NewWorldScenario/TurnsRemaining.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0089}}<syntaxhighlight lang="lua">if (pPlayer1:GetStartingPlot():GetX() < 50 and pPlayer2:GetStartingPlot():GetX() > 50) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0335}}<syntaxhighlight lang="lua">if (pLoopPlayer:IsAlive() and pLoopPlayer:GetStartingPlot():GetX() > 50) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0338}}<syntaxhighlight lang="lua">unit = pLoopPlayer:InitUnit (iUnitID, pLoopPlayer:GetStartingPlot():GetX(), pLoopPlayer:GetStartingPlot():GetY());</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0446}}<syntaxhighlight lang="lua">if (newPlayer:GetStartingPlot():GetX() < 50) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0448}}<syntaxhighlight lang="lua">elseif (oldPlayer:GetStartingPlot():GetX() < 50 and newPlayer:GetStartingPlot():GetX() > 50) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TurnsRemaining.lua - DLC_04 DLC}}
:<code>DLC/DLC_04/Scenarios/1066Scenario/TurnsRemaining.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0092}}<syntaxhighlight lang="lua">if (playerStartPlot:GetX() == iLondonX and playerStartPlot:GetY() == iLondonY) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0353}}<syntaxhighlight lang="lua">if (playerStartPlot:GetX() == 59 and playerStartPlot:GetY() == 39) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0363}}<syntaxhighlight lang="lua">if (playerStartPlot:GetX() == 44 and playerStartPlot:GetY() == 0) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0518}}<syntaxhighlight lang="lua">unit = player:InitUnit (iUnitID, playerStartPlot:GetX(), playerStartPlot:GetY(), UNITAI_RANGED, DirectionTypes.DIRECTION_WEST);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TurnsRemaining.lua (G&K)}}
:<code>DLC/Expansion/Scenarios/MedievalScenario/TurnsRemaining.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0817}}<syntaxhighlight lang="lua">SetPersistentProperty("JerusalemX", pJerusalemPlot:GetX());</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1036}}<syntaxhighlight lang="lua">print ("Team: ", iTeam, "; Revealing x: ", pPlot:GetX(), ", y: ", pPlot:GetY());</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1042}}<syntaxhighlight lang="lua">local adjPlot = Map.PlotDirection(pPlot:GetX(), pPlot:GetY(), direction);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1070}}<syntaxhighlight lang="lua">local capital = pPlayer:InitCity(startPlot:GetX(), startPlot:GetY());</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1147}}<syntaxhighlight lang="lua">SetZurichLocation(startPlot:GetX(), startPlot:GetY());</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1153}}<syntaxhighlight lang="lua">SetVaticanLocation(startPlot:GetX(), startPlot:GetY());</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TurnsRemaining.lua (G&K)}}
:<code>DLC/Expansion/Scenarios/SteampunkScenario/TurnsRemaining.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0850}}<syntaxhighlight lang="lua">local pUnit = pPlayer:InitUnit(eUnitType, pPlot:GetX(), pPlot:GetY());</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TutorialChecks.lua}}
:<code>Tutorial/TutorialChecks.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1432}}<syntaxhighlight lang="lua">local iX = pPlot:GetX();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1560}}<syntaxhighlight lang="lua">if (Map.PlotDistance(pFirstUnitPlot:GetX(), pFirstUnitPlot:GetY(), pSecondUnitPlot:GetX(), pSecondUnitPlot:GetY()) <= iMovesLeft ) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|UnitFlagManager.lua}}
:<code>UI/InGame/UnitFlagManager.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1033}}<syntaxhighlight lang="lua">local cityFlagInstance = g_CityFlags[ pPlot:GetX() .. " " .. pPlot:GetY() ];</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1039}}<syntaxhighlight lang="lua">g_CityFlags[ pPlot:GetX() .. " " .. pPlot:GetY() ] = cityFlagInstance;</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1042}}<syntaxhighlight lang="lua">local worldPos = Vector4( GridToWorld( pPlot:GetX(), pPlot:GetY() ) );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|WorldView.lua}}
:<code>UI/InGame/WorldView/WorldView.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0162}}<syntaxhighlight lang="lua">local unit = player:InitUnit(g_UnitPlopper.UnitType, plot:GetX(), plot:GetY());</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetX]]