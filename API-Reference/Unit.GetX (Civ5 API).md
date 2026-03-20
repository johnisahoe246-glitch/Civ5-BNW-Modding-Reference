{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Unit}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''int''' Unit:GetX<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.

=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|Bombardment.lua}}
:<code>UI/InGame/Bombardment.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0034}}<syntaxhighlight lang="lua">thisX = pHeadSelectedUnit:GetX();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0193}}<syntaxhighlight lang="lua">Events.SpawnArrowEvent( attacker:GetX(), attacker:GetY(), hexX, hexY );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|EnemyUnitPanel.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/WorldView/EnemyUnitPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0931}}<syntaxhighlight lang="lua">local plotDistance = Map.PlotDistance(pCapital:GetX(), pCapital:GetY(), pMyUnit:GetX(), pMyUnit:GetY());</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1480}}<syntaxhighlight lang="lua">local plotDistance = Map.PlotDistance(pCapital:GetX(), pCapital:GetY(), pTheirUnit:GetX(), pTheirUnit:GetY());</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1821}}<syntaxhighlight lang="lua">local plotDistance = Map.PlotDistance(pCapital:GetX(), pCapital:GetY(), theirUnit:GetX(), theirUnit:GetY());</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|InGame.lua}}
:<code>UI/InGame/InGame.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0422}}<syntaxhighlight lang="lua">local hexID = ToHexFromGrid( Vector2( unit:GetX(), unit:GetY() ) );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0450}}<syntaxhighlight lang="lua">local unitX = unit:GetX();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0544}}<syntaxhighlight lang="lua">local thisX = pHeadSelectedUnit:GetX();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0999}}<syntaxhighlight lang="lua">Events.RequestYieldDisplay( YieldDisplayTypes.AREA, 2, unit:GetX(), unit:GetY() );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TurnsRemaining.lua - DLC_02 DLC}}
:<code>DLC/DLC_02/Scenarios/NewWorldScenario/TurnsRemaining.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0538}}<syntaxhighlight lang="lua">if (pUnit:GetX() > 9) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0556}}<syntaxhighlight lang="lua">iDistance = Map.PlotDistance(1, iY, pUnit:GetX(), pUnit:GetY());</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TurnsRemaining.lua - DLC_04 DLC}}
:<code>DLC/DLC_04/Scenarios/1066Scenario/TurnsRemaining.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0200}}<syntaxhighlight lang="lua">iX = unit:GetX();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|UnitFlagManager.lua}}
:<code>UI/InGame/UnitFlagManager.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0242}}<syntaxhighlight lang="lua">local worldPosX, worldPosY, worldPosZ = GridToWorld( pUnit:GetX(), pUnit:GetY() );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1409}}<syntaxhighlight lang="lua">local plot = Map.GetPlot( unit:GetX(), unit:GetY() );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|UnitPanel.lua}}
:<code>UI/InGame/WorldView/UnitPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0744}}<syntaxhighlight lang="lua">x = unit and unit:GetX() or 0,</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetX]]