{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Game}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>{{Type5|HandicapType}} Game.GetHandicapType<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|EnemyUnitPanel.lua}}
:<code>UI/InGame/WorldView/EnemyUnitPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1053}}<syntaxhighlight lang="lua">iModifier = GameInfo.HandicapInfos[Game:GetHandicapType()].BarbarianBonus;</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TurnsRemaining.lua - DLC_02 DLC}}
:<code>DLC/DLC_02/Scenarios/NewWorldScenario/TurnsRemaining.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0061}}<syntaxhighlight lang="lua">if (GenerateTreasureFromRazedCity(Game:GetHandicapType(), city:GetOwner(), city:GetPreviousOwner())) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0330}}<syntaxhighlight lang="lua">local iHandicap = Game:GetHandicapType();</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetHandicapType]]
[[Category:Civ5 Game Settings API|GetHandicapType]]