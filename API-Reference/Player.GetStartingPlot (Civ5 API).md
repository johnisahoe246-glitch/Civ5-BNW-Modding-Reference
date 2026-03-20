{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Player}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>{{Type5|Plot}} Player:GetStartingPlot<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|CivsAlive.lua - DLC_01 DLC}}
:<code>DLC/DLC_01/Scenarios/Mongol Scenario/CivsAlive.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0144}}<syntaxhighlight lang="lua">local playerStartPlot = Players[playerID]:GetStartingPlot();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TurnsRemaining.lua - DLC_02 DLC}}
:<code>DLC/DLC_02/Scenarios/NewWorldScenario/TurnsRemaining.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0089}}<syntaxhighlight lang="lua">if (pPlayer1:GetStartingPlot():GetX() < 50 and pPlayer2:GetStartingPlot():GetX() > 50) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0091}}<syntaxhighlight lang="lua">elseif (pPlayer2:GetStartingPlot():GetX() < 50 and pPlayer1:GetStartingPlot():GetX() > 50) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0275}}<syntaxhighlight lang="lua">local myStartingPlot = (Players[myPlayer]) and Players[myPlayer]:GetStartingPlot() or nil;</syntaxhighlight>
{{CodeLine5|0276}}<syntaxhighlight lang="lua">local theirStartingPlot = (Players[theirPlayer]) and Players[theirPlayer]:GetStartingPlot() or nil;</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0335}}<syntaxhighlight lang="lua">if (pLoopPlayer:IsAlive() and pLoopPlayer:GetStartingPlot():GetX() > 50) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0338}}<syntaxhighlight lang="lua">unit = pLoopPlayer:InitUnit (iUnitID, pLoopPlayer:GetStartingPlot():GetX(), pLoopPlayer:GetStartingPlot():GetY());</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0346}}<syntaxhighlight lang="lua">unit = pLoopPlayer:InitUnit (iUnitID, pLoopPlayer:GetStartingPlot():GetX(), pLoopPlayer:GetStartingPlot():GetY(), GameInfoTypes.UNITAI_EXPLORE_SEA, DirectionTypes.DIRECTION_WEST);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0356}}<syntaxhighlight lang="lua">if (pLoopPlayer:IsAlive()and pLoopPlayer:GetStartingPlot():GetX() > 50) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0446}}<syntaxhighlight lang="lua">if (newPlayer:GetStartingPlot():GetX() < 50) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0448}}<syntaxhighlight lang="lua">elseif (oldPlayer:GetStartingPlot():GetX() < 50 and newPlayer:GetStartingPlot():GetX() > 50) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TurnsRemaining.lua - DLC_04 DLC}}
:<code>DLC/DLC_04/Scenarios/1066Scenario/TurnsRemaining.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0089}}<syntaxhighlight lang="lua">local playerStartPlot = pPlayer:GetStartingPlot();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0508}}<syntaxhighlight lang="lua">local playerStartPlot = player:GetStartingPlot();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TurnsRemaining.lua (G&K)}}
:<code>DLC/Expansion/Scenarios/MedievalScenario/TurnsRemaining.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1069}}<syntaxhighlight lang="lua">local startPlot = pPlayer:GetStartingPlot();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TurnsRemaining.lua (G&K)}}
:<code>DLC/Expansion/Scenarios/SteampunkScenario/TurnsRemaining.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0847}}<syntaxhighlight lang="lua">local pPlot = pPlayer:GetStartingPlot();</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetStartingPlot]]
[[Category:Civ5 Players API|GetStartingPlot]]