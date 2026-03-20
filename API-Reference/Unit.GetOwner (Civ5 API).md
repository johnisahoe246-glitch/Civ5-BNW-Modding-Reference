{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Unit}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>{{Type5|PlayerID}} Unit:GetOwner<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|EnemyUnitPanel.lua}}
:<code>UI/InGame/WorldView/EnemyUnitPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0103}}<syntaxhighlight lang="lua">local pPlayer = Players[pUnit:GetOwner()];</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0567}}<syntaxhighlight lang="lua">local iMyPlayer = pMyUnit:GetOwner();</syntaxhighlight>
{{CodeLine5|0568}}<syntaxhighlight lang="lua">local iTheirPlayer = pTheirUnit:GetOwner();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0611}}<syntaxhighlight lang="lua">local pFireSupportUnit = pMyUnit:GetFireSupportUnit(pTheirUnit:GetOwner(), pToPlot:GetX(), pToPlot:GetY());</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1055}}<syntaxhighlight lang="lua">iModifier = iModifier + Players[pMyUnit:GetOwner()]:GetBarbarianCombatBonus();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1422}}<syntaxhighlight lang="lua">local iTheirPlayer = theirUnit:GetOwner();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1460}}<syntaxhighlight lang="lua">local theirPlayerID = theirUnit:GetOwner();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1845}}<syntaxhighlight lang="lua">if (pTeam:IsAtWar(pUnit:GetTeam()) or (UIManager:GetAlt() and pUnit:GetOwner() ~= iTeam)) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1941}}<syntaxhighlight lang="lua">if (myTeam:IsAtWar(theirUnit:GetTeam()) or (UIManager:GetAlt() and theirUnit:GetOwner() ~= myTeamID)) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|InGame.lua}}
:<code>UI/InGame/InGame.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0184}}<syntaxhighlight lang="lua">if (pFoundUnit:GetOwner() == iPlayerID) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|PlotMouseoverInclude.lua}}
:<code>UI/InGame/PlotMouseoverInclude.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0268}}<syntaxhighlight lang="lua">local pPlayer = Players[unit:GetOwner()];</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0294}}<syntaxhighlight lang="lua">strUnitText = strUnitText .. " ("..tostring(unit:GetOwner()).." - " .. tostring(unit:GetID()) .. ")";</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TurnsRemaining.lua - DLC_04 DLC}}
:<code>DLC/DLC_04/Scenarios/1066Scenario/TurnsRemaining.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0204}}<syntaxhighlight lang="lua">iOldOwner = unit:GetOwner();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TutorialChecks.lua}}
:<code>Tutorial/TutorialChecks.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0251}}<syntaxhighlight lang="lua">if (v:IsCombatUnit() and pPlot:GetOwner() == v:GetOwner()) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1371}}<syntaxhighlight lang="lua">if (pPlot and pPlot:GetOwner() ~= v:GetOwner() and pPlot:GetUnitPower() <= 0) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|UnitFlagManager.lua}}
:<code>UI/InGame/UnitFlagManager.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0609}}<syntaxhighlight lang="lua">local playerTable = g_MasterList[ escortUnit:GetOwner() ];</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1069}}<syntaxhighlight lang="lua">controlTable.Button:SetVoids( pPlotUnit:GetOwner(), pPlotUnit:GetID() );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1264}}<syntaxhighlight lang="lua">local owner, unitID = unit:GetOwner(), unit:GetID();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1447}}<syntaxhighlight lang="lua">local playerTable = g_MasterList[ pUnit:GetOwner() ];</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|UnitPanel.lua}}
:<code>UI/InGame/WorldView/UnitPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0447}}<syntaxhighlight lang="lua">local pPlayer = Players[ unit:GetOwner() ];</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0944}}<syntaxhighlight lang="lua">if (pPlot:GetOwner() ~= unit:GetOwner()) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|WorldView.lua}}
:<code>UI/InGame/WorldView/WorldView.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0618}}<syntaxhighlight lang="lua">if (plot:IsVisibleEnemyUnit(pHeadSelectedUnit:GetOwner()) or plot:IsEnemyCity(pHeadSelectedUnit)) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0644}}<syntaxhighlight lang="lua">if (city and city:GetOwner() == pHeadSelectedUnit:GetOwner() and pHeadSelectedUnit:IsCanAttack()) then</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetOwner]]
[[Category:Civ5 Terrain Ownership API|GetOwner]]