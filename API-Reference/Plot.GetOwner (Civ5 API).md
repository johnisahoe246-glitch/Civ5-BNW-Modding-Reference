{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Plot}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>{{Type5|PlayerID}} Plot:GetOwner<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|CityBannerManager.lua}}
:<code>UI/InGame/CityBannerManager.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1091}}<syntaxhighlight lang="lua">local playerID = plot:GetOwner();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CityStateDiploPopup.lua}}
:<code>UI/InGame/Popups/CityStateDiploPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0302}}<syntaxhighlight lang="lua">local iOwner = pTargetPlot:GetOwner();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CityView.lua}}
:<code>UI/InGame/CityView/CityView.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1726}}<syntaxhighlight lang="lua">if ( plot:GetOwner() == pCity:GetOwner() ) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CivsAlive.lua - DLC_01 DLC}}
:<code>DLC/DLC_01/Scenarios/Mongol Scenario/CivsAlive.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0145}}<syntaxhighlight lang="lua">local eOwner = playerStartPlot:GetOwner();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DeclareWarMovePopup.lua}}
:<code>UI/InGame/PopupsGeneric/DeclareWarMovePopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0016}}<syntaxhighlight lang="lua">local owner = Players[plot:GetOwner()];</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|EnemyUnitPanel.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/WorldView/EnemyUnitPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0904}}<syntaxhighlight lang="lua">if (pToPlot:GetOwner() == iMyPlayer) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1453}}<syntaxhighlight lang="lua">if (pToPlot:GetOwner() == iTheirPlayer) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1795}}<syntaxhighlight lang="lua">if (theirPlot:GetOwner() == iTheirPlayer) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|MinorCivEnterTerritoryPopup.lua}}
:<code>UI/InGame/PopupsGeneric/MinorCivEnterTerritoryPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0014}}<syntaxhighlight lang="lua">popupText = Locale.ConvertTextKey("TXT_KEY_POPUP_ENTER_MINOR_CIV_LANDS", Players[plot:GetOwner()]:GetCivilizationAdjective());</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|PlotMouseoverInclude.lua}}
:<code>UI/InGame/PlotMouseoverInclude.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0414}}<syntaxhighlight lang="lua">if(plot:GetOwner() ~= activePlayer) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TurnsRemaining.lua - DLC_02 DLC}}
:<code>DLC/DLC_02/Scenarios/NewWorldScenario/TurnsRemaining.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0397}}<syntaxhighlight lang="lua">local iNWOwner = pPlot:GetOwner();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0404}}<syntaxhighlight lang="lua">local iPlayer = adjacentPlot:GetOwner();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TurnsRemaining.lua (G&K)}}
:<code>DLC/Expansion/Scenarios/MedievalScenario/TurnsRemaining.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0427}}<syntaxhighlight lang="lua">local iOwner = pVaticanPlot:GetOwner();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0486}}<syntaxhighlight lang="lua">if (pJerusalemPlot:GetOwner() == ePlayer) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0490}}<syntaxhighlight lang="lua">local eOwner = pJerusalemPlot:GetOwner();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1388}}<syntaxhighlight lang="lua">if (plot:GetOwner() ~= -1) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1400}}<syntaxhighlight lang="lua">if (adjPlot:GetOwner() ~= -1) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TutorialChecks.lua}}
:<code>Tutorial/TutorialChecks.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0251}}<syntaxhighlight lang="lua">if (v:IsCombatUnit() and pPlot:GetOwner() == v:GetOwner()) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0312}}<syntaxhighlight lang="lua">if (plot:GetOwner() ~= Game.GetActivePlayer() and player:GetPlotDanger(plot) > 0) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1371}}<syntaxhighlight lang="lua">if (pPlot and pPlot:GetOwner() ~= v:GetOwner() and pPlot:GetUnitPower() <= 0) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|2458}}<syntaxhighlight lang="lua">local iPlotOwner = pPlot:GetOwner();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|UnitPanel.lua}}
:<code>UI/InGame/WorldView/UnitPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0944}}<syntaxhighlight lang="lua">if (pPlot:GetOwner() ~= unit:GetOwner()) then</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetOwner]]
[[Category:Civ5 Terrain Ownership API|GetOwner]]