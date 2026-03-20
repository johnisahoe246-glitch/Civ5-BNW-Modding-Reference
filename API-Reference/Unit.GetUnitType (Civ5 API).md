{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Unit}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>{{Type5|UnitType}} Unit:GetUnitType<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|EnemyUnitPanel.lua}}
:<code>UI/InGame/WorldView/EnemyUnitPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0095}}<syntaxhighlight lang="lua">local thisUnitInfo = GameInfo.Units[pUnit:GetUnitType()];</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|EnemyUnitPanel.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/WorldView/EnemyUnitPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0907}}<syntaxhighlight lang="lua">if (iModifier ~= 0 and pTheirUnit:IsHigherTechThan(pMyUnit:GetUnitType())) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1456}}<syntaxhighlight lang="lua">if (iModifier ~= 0 and pMyUnit:IsHigherTechThan(pTheirUnit:GetUnitType())) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1798}}<syntaxhighlight lang="lua">if (iModifier ~= 0 and pMyUnit:IsHigherTechThan(theirUnit:GetUnitType())) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|InGame.lua}}
:<code>UI/InGame/InGame.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0989}}<syntaxhighlight lang="lua">if (GameInfo.Units[unit:GetUnitType()].DontShowYields) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TurnsRemaining.lua - DLC_02 DLC}}
:<code>DLC/DLC_02/Scenarios/NewWorldScenario/TurnsRemaining.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0140}}<syntaxhighlight lang="lua">if (unit:GetUnitType() == GameInfoTypes["UNIT_CARAVEL"]) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0205}}<syntaxhighlight lang="lua">if (unit:GetUnitType() == GameInfoTypes["UNIT_TREASURE"]) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TurnsRemaining.lua - DLC_04 DLC}}
:<code>DLC/DLC_04/Scenarios/1066Scenario/TurnsRemaining.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0202}}<syntaxhighlight lang="lua">iUnitType = unit:GetUnitType();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TurnsRemaining.lua (G&K)}}
:<code>DLC/Expansion/Scenarios/FallOfRomeScenario/TurnsRemaining.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1009}}<syntaxhighlight lang="lua">print(pUnit:GetUnitType());</syntaxhighlight>
{{CodeLine5|1010}}<syntaxhighlight lang="lua">if pUnit:GetUnitType() == GameInfoTypes["UNIT_ROMAN_LEGION"] then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TurnsRemaining.lua (G&K)}}
:<code>DLC/Expansion/Scenarios/MedievalScenario/TurnsRemaining.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0605}}<syntaxhighlight lang="lua">if (unit:GetUnitType() == GameInfoTypes["UNIT_CARAVEL"] and iNumCaravels < 5) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0643}}<syntaxhighlight lang="lua">if (unit:GetUnitType() == GameInfoTypes["UNIT_SPANISH_CONQUISTADOR"]) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TutorialChecks.lua}}
:<code>Tutorial/TutorialChecks.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0976}}<syntaxhighlight lang="lua">local UnitType = v:GetUnitType();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|UnitPanel.lua}}
:<code>UI/InGame/WorldView/UnitPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0438}}<syntaxhighlight lang="lua">local thisUnitInfo = GameInfo.Units[unit:GetUnitType()];</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|UnitPanel.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/WorldView/UnitPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0667}}<syntaxhighlight lang="lua">elseif (GameInfo.Units[unit:GetUnitType()].RemoveHeresy) then</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetUnitType]]
[[Category:Civ5 Units API|GetUnitType]]