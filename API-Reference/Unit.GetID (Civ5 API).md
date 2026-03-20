{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Unit}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>{{Type5|UnitID}} Unit:GetID<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|InGame.lua}}
:<code>UI/InGame/InGame.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0204}}<syntaxhighlight lang="lua">Data3 = pUnit:GetID();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0517}}<syntaxhighlight lang="lua">Events.ShowMovementRange( iPlayerID, unit:GetID() );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0619}}<syntaxhighlight lang="lua">Events.ShowAttackTargets(iPlayerID, unit:GetID());</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0964}}<syntaxhighlight lang="lua">unit:GetID() == unitId and</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|MilitaryOverview.lua}}
:<code>UI/InGame/Popups/MilitaryOverview.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0070}}<syntaxhighlight lang="lua">pSelectedUnit:GetID() == unitID ) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0136}}<syntaxhighlight lang="lua">iSelectedUnit = pSelectedUnit:GetID();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0145}}<syntaxhighlight lang="lua">local iUnit = unit:GetID();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0159}}<syntaxhighlight lang="lua">instance.Button:SetVoid1( unit:GetID() );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|PlotMouseoverInclude.lua}}
:<code>UI/InGame/PlotMouseoverInclude.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0294}}<syntaxhighlight lang="lua">strUnitText = strUnitText .. " ("..tostring(unit:GetOwner()).." - " .. tostring(unit:GetID()) .. ")";</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|SetUnitName.lua}}
:<code>UI/InGame/Popups/SetUnitName.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0019}}<syntaxhighlight lang="lua">Network.SendRenameUnit(pUnit:GetID(), Controls.EditUnitName:GetText());</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TutorialChecks.lua}}
:<code>Tutorial/TutorialChecks.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0202}}<syntaxhighlight lang="lua">return v:GetID();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0460}}<syntaxhighlight lang="lua">iWorkerID = v:GetID();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0587}}<syntaxhighlight lang="lua">iUnitID = v:GetID();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|2487}}<syntaxhighlight lang="lua">return unit:GetID();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|UnitFlagManager.lua}}
:<code>UI/InGame/UnitFlagManager.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0596}}<syntaxhighlight lang="lua">if( test ~= nil and test:GetID() ~= self.m_UnitID and not test:IsGarrisoned() )</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0616}}<syntaxhighlight lang="lua">local escortFlag = playerTable[ escortUnit:GetID() ];</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0716}}<syntaxhighlight lang="lua">controlTable.Button:SetVoids( self.m_playerID, pPlotUnit:GetID() );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1069}}<syntaxhighlight lang="lua">controlTable.Button:SetVoids( pPlotUnit:GetOwner(), pPlotUnit:GetID() );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1264}}<syntaxhighlight lang="lua">local owner, unitID = unit:GetOwner(), unit:GetID();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1412}}<syntaxhighlight lang="lua">OnUnitCreated( player:GetID(), unit:GetID(), 0, 0, 0, 0, 0, 0, 0, WhiteFog, 0, 0, true );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1449}}<syntaxhighlight lang="lua">local pFlag = playerTable[ pUnit:GetID() ];</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|UnitFlagManager.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/UnitFlagManager.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0595}}<syntaxhighlight lang="lua">if( test ~= nil and test:GetID() ~= self.m_UnitID and not test:IsGarrisoned() and not test:IsDead() and not test:IsDelayedDeath() )</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|UnitList.lua}}
:<code>UI/InGame/UnitList.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0285}}<syntaxhighlight lang="lua">valueA = entryA.unit:GetID();</syntaxhighlight>
{{CodeLine5|0286}}<syntaxhighlight lang="lua">valueB = entryB.unit:GetID();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|UnitPanel.lua}}
:<code>UI/InGame/WorldView/UnitPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0739}}<syntaxhighlight lang="lua">local unitID = unit and unit:GetID() or -1;</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0825}}<syntaxhighlight lang="lua">Data1 = UI.GetHeadSelectedUnit():GetID(),</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetID]]