{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Plot}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''int''' Plot:IsWater<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|Amazon_XP.lua (G&K)}}
:<code>DLC/Expansion/Maps/Amazon_XP.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0261}}<syntaxhighlight lang="lua">if plot:IsWater() then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0390}}<syntaxhighlight lang="lua">if not plot:IsWater() and (plot:GetFeatureType() == FeatureTypes.NO_FEATURE) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0479}}<syntaxhighlight lang="lua">if (adjacentPlot == nil or riverPlot:IsNEOfRiver() or riverPlot:IsWater() or adjacentPlot:IsWater()) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0491}}<syntaxhighlight lang="lua">if (adjacentPlot == nil or riverPlot:IsWOfRiver() or riverPlot:IsWater() or adjacentPlot:IsWater()) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0580}}<syntaxhighlight lang="lua">if ( adjacentPlot == nil or riverPlot:IsWOfRiver() or riverPlot:IsWater() or adjacentPlot:IsWater() ) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0592}}<syntaxhighlight lang="lua">if ( adjacentPlot == nil or riverPlot:IsNWOfRiver() or riverPlot:IsWater() or adjacentPlot:IsWater() ) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0636}}<syntaxhighlight lang="lua">if (adjacentPlot == nil or riverPlot:IsNWOfRiver() or riverPlot:IsWater() or adjacentPlot:IsWater()) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0649}}<syntaxhighlight lang="lua">if ( adjacentPlot == nil or riverPlot:IsNEOfRiver() or riverPlot:IsWater() or adjacentPlot:IsWater()) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0662}}<syntaxhighlight lang="lua">if (riverPlot == nil or riverPlot:IsWater()) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0849}}<syntaxhighlight lang="lua">elseif(not plot:IsWater()) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|AssignStartingPlots.lua}}
:<code>Gameplay/Lua/AssignStartingPlots.lua</code>
:{{CodeBegin5}}
{{CodeLine5|5083}}<syntaxhighlight lang="lua">if self.plotDataIsCoastal[plotIndex] == false and plot:IsWater() == false then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|AssignStartingPlots.lua (G&K)}}
:<code>DLC/Expansion/Gameplay/Lua/AssignStartingPlots.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1552}}<syntaxhighlight lang="lua">if not plot:IsWater() then -- Land plot, process it.</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|5247}}<syntaxhighlight lang="lua">if plot:IsWater() == true then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|Bombardment.lua}}
:<code>UI/InGame/Bombardment.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0057}}<syntaxhighlight lang="lua">if thingThatCanActuallyFire:GetDomainType() == DomainTypes.DOMAIN_LAND and pTargetPlot:IsWater() then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0059}}<syntaxhighlight lang="lua">elseif thingThatCanActuallyFire:GetDomainType() == DomainTypes.DOMAIN_SEA and not pTargetPlot:IsWater() then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|Boreal.lua (G&K)}}
:<code>DLC/Expansion/Maps/Boreal.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0568}}<syntaxhighlight lang="lua">elseif iY >= iH - 5 and plot:IsWater() then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CityView.lua}}
:<code>UI/InGame/CityView/CityView.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1781}}<syntaxhighlight lang="lua">elseif ( plot:IsWater() and pCity:IsPlotBlockaded( plot ) ) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|EnemyUnitPanel.lua}}
:<code>UI/InGame/WorldView/EnemyUnitPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0757}}<syntaxhighlight lang="lua">if (not pToPlot:IsWater() and pMyUnit:GetPlot():IsWater()) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1796}}<syntaxhighlight lang="lua">if (pHeadUnit:IsCombatUnit() and (pHeadUnit:IsRanged() and pHeadUnit:IsEmbarked()) == false) and ((pHeadUnit:IsRanged() and pHeadUnit:IsRangeAttackOnlyInDomain() and not pPlot:IsWater()) == false) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|EnemyUnitPanel.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/WorldView/EnemyUnitPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0792}}<syntaxhighlight lang="lua">if (not pToPlot:IsWater() and pMyUnit:GetPlot():IsWater() and pMyUnit:GetDomainType() == DomainTypes.DOMAIN_LAND) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|Great_Plains.lua}}
:<code>Maps/Great_Plains.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1508}}<syntaxhighlight lang="lua">if plot:IsWater() or plot:IsMountain() or plot:GetFeatureType() == FeatureTypes.FEATURE_OASIS then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|MapGenerator.lua (G&K)}}
:<code>DLC/Expansion/Gameplay/Lua/MapGenerator.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0187}}<syntaxhighlight lang="lua">if(plot:IsWater()) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0538}}<syntaxhighlight lang="lua">if(not plot:IsWater()) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0695}}<syntaxhighlight lang="lua">if ( not plot:IsWater() ) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|MapmakerUtilities.lua}}
:<code>Gameplay/Lua/MapmakerUtilities.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0370}}<syntaxhighlight lang="lua">if plotDataIsCoastal[i] == false and not plot:IsWater() then -- plot is not itself on the coast or in the water.</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|NaturalWondersCustomMethods.lua (G&K)}}
:<code>DLC/Expansion/Gameplay/Lua/NaturalWondersCustomMethods.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0046}}<syntaxhighlight lang="lua">if adjPlot:IsWater() == false or adjPlot:IsLake() == true then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0067}}<syntaxhighlight lang="lua">if adjPlot:IsWater() == false then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0087}}<syntaxhighlight lang="lua">if plot:IsWater() == false and AdjacentToSaltWater(x, y) == false then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0143}}<syntaxhighlight lang="lua">if not plot:IsWater() then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0155}}<syntaxhighlight lang="lua">if not SEPlot:IsWater() then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|Skirmish.lua}}
:<code>Maps/Skirmish.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0663}}<syntaxhighlight lang="lua">elseif (not plot:IsWater()) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TerrainGenerator.lua}}
:<code>Gameplay/Lua/TerrainGenerator.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0164}}<syntaxhighlight lang="lua">if (plot:IsWater()) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TurnsRemaining.lua (G&K)}}
:<code>DLC/Expansion/Scenarios/MedievalScenario/TurnsRemaining.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1392}}<syntaxhighlight lang="lua">elseif (plot:IsWater()) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1404}}<syntaxhighlight lang="lua">elseif (adjPlot:IsWater()) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TutorialChecks.lua}}
:<code>Tutorial/TutorialChecks.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1438}}<syntaxhighlight lang="lua">if (not pTargetPlot:IsWater() and pTargetPlot:IsVisibleEnemyUnit(player:GetID())) then</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|IsWater]]
[[Category:Civ5 Terrain API|IsWater]]