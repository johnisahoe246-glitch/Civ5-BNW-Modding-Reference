{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Plot}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>{{Type5|FeatureType}} Plot:GetFeatureType<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
''Too many occurences. Only 50 out of 133 are listed.''

{{PseudoH4|Amazon_XP.lua (G&K)}}
:<code>DLC/Expansion/Maps/Amazon_XP.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0390}}<syntaxhighlight lang="lua">if not plot:IsWater() and (plot:GetFeatureType() == FeatureTypes.NO_FEATURE) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0435}}<syntaxhighlight lang="lua">if plot:GetFeatureType() == FeatureTypes.NO_FEATURE and not plot:IsMountain() then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1328}}<syntaxhighlight lang="lua">local featureType = res_plot:GetFeatureType()</syntaxhighlight>
{{CodeLine5|1329}}<syntaxhighlight lang="lua">if featureType == FeatureTypes.FEATURE_MARSH then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|AssignStartingPlots.lua}}
:<code>Gameplay/Lua/AssignStartingPlots.lua</code>
:{{CodeBegin5}}
{{CodeLine5|5148}}<syntaxhighlight lang="lua">local featureType = adjPlot:GetFeatureType()</syntaxhighlight>
{{CodeLine5|5149}}<syntaxhighlight lang="lua">if featureType == FeatureTypes.FEATURE_MARSH then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|5242}}<syntaxhighlight lang="lua">local featureType = adjPlot:GetFeatureType()</syntaxhighlight>
{{CodeLine5|5243}}<syntaxhighlight lang="lua">if featureType == FeatureTypes.FEATURE_ICE then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|AssignStartingPlots.lua (G&K)}}
:<code>DLC/Expansion/Gameplay/Lua/AssignStartingPlots.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1795}}<syntaxhighlight lang="lua">local featureType = plot:GetFeatureType()</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1797}}<syntaxhighlight lang="lua">-- Mountain and Ocean plot types get their own AreaIDs, but we are going to measure them anyway.</syntaxhighlight>
{{CodeLine5|1798}}<syntaxhighlight lang="lua">if plotType == PlotTypes.PLOT_MOUNTAIN then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|2200}}<syntaxhighlight lang="lua">local featureType = plot:GetFeatureType()</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|2202}}<syntaxhighlight lang="lua">if plotType == PlotTypes.PLOT_MOUNTAIN then -- Mountains are Junk.</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|3484}}<syntaxhighlight lang="lua">local featureType = plot:GetFeatureType()</syntaxhighlight>
{{CodeLine5|3485}}<syntaxhighlight lang="lua">if featureType == FeatureTypes.FEATURE_OASIS then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|3596}}<syntaxhighlight lang="lua">local featureType = plot:GetFeatureType()</syntaxhighlight>
{{CodeLine5|3597}}<syntaxhighlight lang="lua">if plotType ~= PlotTypes.PLOT_LAND then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|3673}}<syntaxhighlight lang="lua">local featureType = plot:GetFeatureType()</syntaxhighlight>
{{CodeLine5|3674}}<syntaxhighlight lang="lua">local plotIndex = realY * iW + realX + 1;</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|3785}}<syntaxhighlight lang="lua">local featureType = plot:GetFeatureType()</syntaxhighlight>
{{CodeLine5|3786}}<syntaxhighlight lang="lua">if featureType == FeatureTypes.NO_FEATURE then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|3879}}<syntaxhighlight lang="lua">local featureType = searchPlot:GetFeatureType()</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|3881}}<syntaxhighlight lang="lua">if plotType == PlotTypes.PLOT_MOUNTAIN then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|5318}}<syntaxhighlight lang="lua">local featureType = plot:GetFeatureType()</syntaxhighlight>
{{CodeLine5|5319}}<syntaxhighlight lang="lua">if featureType == FeatureTypes.NO_FEATURE and self.CoreTileCanBeNoFeature[wn] == true then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|5517}}<syntaxhighlight lang="lua">local featureType = adjPlot:GetFeatureType();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|7143}}<syntaxhighlight lang="lua">local featureType = plot:GetFeatureType()</syntaxhighlight>
{{CodeLine5|7144}}<syntaxhighlight lang="lua">if plotType == PlotTypes.PLOT_MOUNTAIN then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|8295}}<syntaxhighlight lang="lua">local featureType = plot:GetFeatureType()</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|8297}}<syntaxhighlight lang="lua">if plotType == PlotTypes.PLOT_OCEAN then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|9206}}<syntaxhighlight lang="lua">local featureType = plot:GetFeatureType()</syntaxhighlight>
{{CodeLine5|9207}}<syntaxhighlight lang="lua">if plot:GetResourceType(-1) == -1 and featureType ~= FeatureTypes.FEATURE_OASIS then -- No resource or Oasis here, safe to proceed.</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|9356}}<syntaxhighlight lang="lua">local featureType = plot:GetFeatureType()</syntaxhighlight>
{{CodeLine5|9357}}<syntaxhighlight lang="lua">if plotType == PlotTypes.PLOT_LAND or plotType == PlotTypes.PLOT_HILLS then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|EnemyUnitPanel.lua}}
:<code>UI/InGame/WorldView/EnemyUnitPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1019}}<syntaxhighlight lang="lua">if (pToPlot:GetFeatureType() ~= -1) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1022}}<syntaxhighlight lang="lua">iModifier = pMyUnit:FeatureAttackModifier(pToPlot:GetFeatureType());</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1025}}<syntaxhighlight lang="lua">local featureTypeBonus = Locale.ConvertTextKey(GameInfo.Features[pToPlot:GetFeatureType()].Description);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1323}}<syntaxhighlight lang="lua">iModifier = pTheirUnit:FeatureDefenseModifier(pToPlot:GetFeatureType());</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1326}}<syntaxhighlight lang="lua">local typeBonus = Locale.ConvertTextKey(GameInfo.Features[pToPlot:GetFeatureType()].Description);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1592}}<syntaxhighlight lang="lua">if (theirPlot:GetFeatureType() ~= -1) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1595}}<syntaxhighlight lang="lua">iModifier = theirUnit:FeatureDefenseModifier(theirPlot:GetFeatureType());</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1598}}<syntaxhighlight lang="lua">local typeBonus = Locale.ConvertTextKey(GameInfo.Features[theirPlot:GetFeatureType()].Description);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|FeatureGenerator.lua (G&K)}}
:<code>DLC/Expansion/Gameplay/Lua/FeatureGenerator.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0209}}<syntaxhighlight lang="lua">if (plot:GetFeatureType() == FeatureTypes.NO_FEATURE) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0294}}<syntaxhighlight lang="lua">if (plot:GetFeatureType() == self.featureJungle) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0357}}<syntaxhighlight lang="lua">local featureType = plot:GetFeatureType()</syntaxhighlight>
{{CodeLine5|0358}}<syntaxhighlight lang="lua">if featureType ~= FeatureTypes.FEATURE_ICE then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0377}}<syntaxhighlight lang="lua">local adjFeatureType = adjPlot:GetFeatureType()</syntaxhighlight>
{{CodeLine5|0378}}<syntaxhighlight lang="lua">if adjFeatureType == FeatureTypes.FEATURE_ICE then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|Great_Plains.lua}}
:<code>Maps/Great_Plains.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1508}}<syntaxhighlight lang="lua">if plot:IsWater() or plot:IsMountain() or plot:GetFeatureType() == FeatureTypes.FEATURE_OASIS then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|NaturalWonderPopup.lua}}
:<code>UI/InGame/Popups/NaturalWonderPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0026}}<syntaxhighlight lang="lua">local feature = pNaturalWonderPlot:GetFeatureType();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|NaturalWondersCustomMethods.lua (G&K)}}
:<code>DLC/Expansion/Gameplay/Lua/NaturalWondersCustomMethods.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0049}}<syntaxhighlight lang="lua">local featureType = adjPlot:GetFeatureType()</syntaxhighlight>
{{CodeLine5|0050}}<syntaxhighlight lang="lua">if featureType ~= FeatureTypes.NO_FEATURE then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0104}}<syntaxhighlight lang="lua">local featureType = adjPlot:GetFeatureType()</syntaxhighlight>
{{CodeLine5|0105}}<syntaxhighlight lang="lua">if terrainType == TerrainTypes.TERRAIN_COAST and plot:IsLake() == false then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0161}}<syntaxhighlight lang="lua">if SEPlot:GetFeatureType() ~= FeatureTypes.NO_FEATURE then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|PlotMouseoverInclude.lua}}
:<code>UI/InGame/PlotMouseoverInclude.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0042}}<syntaxhighlight lang="lua">local iFeature = plot:GetFeatureType();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0052}}<syntaxhighlight lang="lua">local convertedKey = Locale.ConvertTextKey( GameInfo.Features[plot:GetFeatureType()].Description);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0069}}<syntaxhighlight lang="lua">if (GameInfo.Features[plot:GetFeatureType()].NaturalWonder) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0415}}<syntaxhighlight lang="lua">local featureType = plot:GetFeatureType();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ReplayViewer.lua}}
:<code>UI/InGame/Popups/ReplayViewer.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1340}}<syntaxhighlight lang="lua">FeatureType = plot:GetFeatureType(),</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TurnsRemaining.lua - DLC_02 DLC}}
:<code>DLC/DLC_02/Scenarios/NewWorldScenario/TurnsRemaining.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0394}}<syntaxhighlight lang="lua">if (pPlot:GetFeatureType() == iFeatureID) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TutorialChecks.lua}}
:<code>Tutorial/TutorialChecks.lua</code>
:{{CodeBegin5}}
{{CodeLine5|2041}}<syntaxhighlight lang="lua">if (pPlot:GetFeatureType() == FeatureTypes.FEATURE_FOREST) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|2043}}<syntaxhighlight lang="lua">elseif (pPlot:GetFeatureType() == FeatureTypes.FEATURE_MARSH) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|2045}}<syntaxhighlight lang="lua">elseif (pPlot:GetFeatureType() == FeatureTypes.FEATURE_JUNGLE) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|UnitPanel.lua}}
:<code>UI/InGame/WorldView/UnitPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0883}}<syntaxhighlight lang="lua">local iFeature = unit:GetPlot():GetFeatureType();</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetFeatureType]]
[[Category:Civ5 Features & Natural wonders API|GetFeatureType]]