{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Unit}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>{{Type5|Plot}} Unit:GetPlot<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|ActionInfoPanel.lua}}
:<code>UI/InGame/WorldView/ActionInfoPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0107}}<syntaxhighlight lang="lua">local pPlot = v:GetPlot();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0120}}<syntaxhighlight lang="lua">local pPlot = pUnit:GetPlot();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|Bombardment.lua}}
:<code>UI/InGame/Bombardment.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0033}}<syntaxhighlight lang="lua">thisPlot = pHeadSelectedUnit:GetPlot();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|EnemyUnitPanel.lua}}
:<code>UI/InGame/WorldView/EnemyUnitPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0576}}<syntaxhighlight lang="lua">local pFromPlot = pMyUnit:GetPlot();</syntaxhighlight>
{{CodeLine5|0577}}<syntaxhighlight lang="lua">local pToPlot = pTheirUnit:GetPlot();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0744}}<syntaxhighlight lang="lua">if (pMyUnit:GetPlot():IsRiverCrossingToPlot(pToPlot)) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0757}}<syntaxhighlight lang="lua">if (not pToPlot:IsWater() and pMyUnit:GetPlot():IsWater()) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1463}}<syntaxhighlight lang="lua">local theirPlot = theirUnit:GetPlot();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|EnemyUnitPanel.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/WorldView/EnemyUnitPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0792}}<syntaxhighlight lang="lua">if (not pToPlot:IsWater() and pMyUnit:GetPlot():IsWater() and pMyUnit:GetDomainType() == DomainTypes.DOMAIN_LAND) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|InGame.lua}}
:<code>UI/InGame/InGame.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0445}}<syntaxhighlight lang="lua">return unit:CanEmbarkOnto(unit:GetPlot(), targetPlot);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0543}}<syntaxhighlight lang="lua">local thisPlot = pHeadSelectedUnit:GetPlot();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|MilitaryOverview.lua}}
:<code>UI/InGame/Popups/MilitaryOverview.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0215}}<syntaxhighlight lang="lua">local iTurnsLeft = unit:GetPlot():GetBuildTurnsLeft(buildType, 0, 0);</syntaxhighlight>
{{CodeLine5|0216}}<syntaxhighlight lang="lua">local iTurnsTotal = unit:GetPlot():GetBuildTurnsTotal(buildType);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TutorialChecks.lua}}
:<code>Tutorial/TutorialChecks.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0311}}<syntaxhighlight lang="lua">local plot = v:GetPlot();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1083}}<syntaxhighlight lang="lua">local pUnitPlot = v:GetPlot();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1554}}<syntaxhighlight lang="lua">local pFirstUnitPlot = v:GetPlot();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1559}}<syntaxhighlight lang="lua">local pSecondUnitPlot = w:GetPlot();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|3049}}<syntaxhighlight lang="lua">return v:GetPlot();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|UnitFlagManager.lua}}
:<code>UI/InGame/UnitFlagManager.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0580}}<syntaxhighlight lang="lua">local plot = pUnit:GetPlot();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0766}}<syntaxhighlight lang="lua">UpdateCityCargo( pUnit:GetPlot() );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0997}}<syntaxhighlight lang="lua">local pPlot = thisUnit:GetPlot();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|UnitPanel.lua}}
:<code>UI/InGame/WorldView/UnitPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0855}}<syntaxhighlight lang="lua">local pPlot = unit:GetPlot();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0883}}<syntaxhighlight lang="lua">local iFeature = unit:GetPlot():GetFeatureType();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|WorldView.lua}}
:<code>UI/InGame/WorldView/WorldView.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0517}}<syntaxhighlight lang="lua">if (pHeadSelectedUnit:CanEmbarkOnto(pHeadSelectedUnit:GetPlot(), plot)) then</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetPlot]]