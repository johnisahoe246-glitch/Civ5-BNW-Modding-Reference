{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Map}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>{{Type5|Plot}} Map.GetPlot<b>(</b>'''int''' x, '''int''' y = nil<b>)</b></code>


'''Returned Value'''
:No description available.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|x:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|y:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Too many occurences. Only 50 out of 678 are listed.''

{{PseudoH4|AssignStartingPlots.lua (G&K)}}
:<code>DLC/Expansion/Gameplay/Lua/AssignStartingPlots.lua</code>
:{{CodeBegin5}}
{{CodeLine5|2853}}<syntaxhighlight lang="lua">local forcePlot = Map.GetPlot(iWestX, iSouthY);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|4595}}<syntaxhighlight lang="lua">local start_plot = Map.GetPlot(x, y)</syntaxhighlight>
{{CodeLine5|4596}}<syntaxhighlight lang="lua">local player = Players[player_ID]</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|7499}}<syntaxhighlight lang="lua">local res_plot = Map.GetPlot(x, y)</syntaxhighlight>
{{CodeLine5|7500}}<syntaxhighlight lang="lua">if res_plot:GetResourceType(-1) == -1 then -- Placing this strategic resource in this plot.</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CityBannerManager.lua}}
:<code>UI/InGame/CityBannerManager.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1089}}<syntaxhighlight lang="lua">local plot = Map.GetPlot( x, y );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CityStateDiploPopup.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/Popups/CityStateDiploPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0611}}<syntaxhighlight lang="lua">local pPlot = Map.GetPlot(iQuestData1, iQuestData2);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|Europe_Scenario.lua (G&K)}}
:<code>DLC/Expansion/Scenarios/MedievalScenario/Europe_Scenario.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1215}}<syntaxhighlight lang="lua">local start_plot = Map.GetPlot(x, y)</syntaxhighlight>
{{CodeLine5|1216}}<syntaxhighlight lang="lua">local player = Players[Celts_PlayerID];</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|FeatureGenerator.lua (G&K)}}
:<code>DLC/Expansion/Gameplay/Lua/FeatureGenerator.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0535}}<syntaxhighlight lang="lua">local plot = Map.GetPlot(x, y)</syntaxhighlight>
{{CodeLine5|0536}}<syntaxhighlight lang="lua">plot:SetFeatureType(feature_atoll, -1);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|MapmakerUtilities.lua}}
:<code>Gameplay/Lua/MapmakerUtilities.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0096}}<syntaxhighlight lang="lua">local plotFirst = Map.GetPlot(0, y);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|PlotHelpManager.lua}}
:<code>UI/InGame/PlotHelpManager.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0122}}<syntaxhighlight lang="lua">local plot = Map.GetPlot(m_iCurrentX, m_iCurrentY);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0327}}<syntaxhighlight lang="lua">local plot = Map.GetPlot( hexX, hexY );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|Rainforest.lua (G&K)}}
:<code>DLC/Expansion/Maps/Rainforest.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0732}}<syntaxhighlight lang="lua">local plot = Map.GetPlot(iX, iY)</syntaxhighlight>
{{CodeLine5|0733}}<syntaxhighlight lang="lua">local terrain_type = plot:GetTerrainType()</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|Skirmish.lua}}
:<code>Maps/Skirmish.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0236}}<syntaxhighlight lang="lua">local plot = Map.GetPlot(x, y)</syntaxhighlight>
{{CodeLine5|0237}}<syntaxhighlight lang="lua">if plot:IsFlatlands() then -- Check for adjacent Mountain plot; if found, change this plot to Hills.</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TurnsRemaining.lua - DLC_04 DLC}}
:<code>DLC/DLC_04/Scenarios/1066Scenario/TurnsRemaining.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0342}}<syntaxhighlight lang="lua">pCity = Map.GetPlot(29,73):GetPlotCity();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0344}}<syntaxhighlight lang="lua">pCity = Map.GetPlot(30,77):GetPlotCity();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0348}}<syntaxhighlight lang="lua">pCity = Map.GetPlot(61,62):GetPlotCity();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0366}}<syntaxhighlight lang="lua">pCity = Map.GetPlot(40,1):GetPlotCity();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0452}}<syntaxhighlight lang="lua">pCity = Map.GetPlot(35,27):GetPlotCity();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0493}}<syntaxhighlight lang="lua">pPlot = Map.GetPlot(44,18);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0751}}<syntaxhighlight lang="lua">Map.GetPlot(42,38):GetUnit(0):SetDeployFromOperationTurn(1);</syntaxhighlight>
{{CodeLine5|0752}}<syntaxhighlight lang="lua">Map.GetPlot(43,38):GetUnit(0):SetDeployFromOperationTurn(1);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0760}}<syntaxhighlight lang="lua">Map.GetPlot(45,36):GetUnit(0):SetDeployFromOperationTurn(1);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TurnsRemaining.lua (G&K)}}
:<code>DLC/Expansion/Scenarios/MedievalScenario/TurnsRemaining.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0484}}<syntaxhighlight lang="lua">local pJerusalemPlot = Map.GetPlot(iJerusalemX, iJerusalemY);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TurnsRemaining.lua (G&K)}}
:<code>DLC/Expansion/Scenarios/FallOfRomeScenario/TurnsRemaining.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0513}}<syntaxhighlight lang="lua">pCity = Map.GetPlot(13,25):GetPlotCity(); -- Carthago Nova</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0515}}<syntaxhighlight lang="lua">pCity = Map.GetPlot(37,27):GetPlotCity(); -- Neapoli</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0517}}<syntaxhighlight lang="lua">pCity = Map.GetPlot(41,27):GetPlotCity(); -- Brundisium</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0553}}<syntaxhighlight lang="lua">pCity = Map.GetPlot(21,48):GetPlotCity(); -- Lutetia</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0557}}<syntaxhighlight lang="lua">pCity = Map.GetPlot(17,52):GetPlotCity(); -- Coriallum</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0567}}<syntaxhighlight lang="lua">pCity = Map.GetPlot(48,7):GetPlotCity();  -- Cyrene</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0571}}<syntaxhighlight lang="lua">pCity = Map.GetPlot(79,13):GetPlotCity(); -- Palmyra</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0573}}<syntaxhighlight lang="lua">pCity = Map.GetPlot(74,14):GetPlotCity(); -- Damascus</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0591}}<syntaxhighlight lang="lua">pCity = Map.GetPlot(67,24):GetPlotCity(); -- Iconium</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0597}}<syntaxhighlight lang="lua">pCity = Map.GetPlot(50,28):GetPlotCity(); -- Thessalonica</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0599}}<syntaxhighlight lang="lua">pCity = Map.GetPlot(58,29):GetPlotCity(); -- Constantinople</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0601}}<syntaxhighlight lang="lua">pCity = Map.GetPlot(45,30):GetPlotCity(); -- Dyrrachium</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0625}}<syntaxhighlight lang="lua">pCity = Map.GetPlot(85,20):GetPlotCity(); -- Singara</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1042}}<syntaxhighlight lang="lua">pPlot = Map.GetPlot(40,36); -- legion</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1098}}<syntaxhighlight lang="lua">pPlot = Map.GetPlot(54,31); -- legion</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1100}}<syntaxhighlight lang="lua">pPlot = Map.GetPlot(71,20); -- boat</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1111}}<syntaxhighlight lang="lua">pPlot = Map.GetPlot(88,17); -- composite bowman</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1127}}<syntaxhighlight lang="lua">pPlot = Map.GetPlot(84,20); -- Clib</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1161}}<syntaxhighlight lang="lua">pPlot = Map.GetPlot(47,44); -- catapult</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1177}}<syntaxhighlight lang="lua">pPlot = Map.GetPlot(1,17); -- Trih</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1197}}<syntaxhighlight lang="lua">pPlot = Map.GetPlot(6,14); -- composite bowman</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1215}}<syntaxhighlight lang="lua">pPlot = Map.GetPlot(29,56); -- seaxman</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1227}}<syntaxhighlight lang="lua">pPlot = Map.GetPlot(31,53); -- seaxman</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1229}}<syntaxhighlight lang="lua">pPlot = Map.GetPlot(37,57); -- seaxman</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1245}}<syntaxhighlight lang="lua">pPlot = Map.GetPlot(15,57); -- archer</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1261}}<syntaxhighlight lang="lua">pPlot = Map.GetPlot(20,56); -- boat</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1293}}<syntaxhighlight lang="lua">pPlot = Map.GetPlot(81,58); -- worker</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TutorialChecks.lua}}
:<code>Tutorial/TutorialChecks.lua</code>
:{{CodeBegin5}}
{{CodeLine5|2039}}<syntaxhighlight lang="lua">local pPlot = Map.GetPlot( gridPosX, gridPosY );</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetPlot]]