{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Game}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>{{Type5|GameplayStateType}} Game.GetGameState<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|CivsAlive.lua - DLC_01 DLC}}
:<code>DLC/DLC_01/Scenarios/Mongol Scenario/CivsAlive.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0032}}<syntaxhighlight lang="lua">if (Game.GetGameState() == GameplayGameStateTypes.GAMESTATE_ON) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DiploCorner.lua}}
:<code>UI/InGame/WorldView/DiploCorner.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0371}}<syntaxhighlight lang="lua">if (iUNCountdown ~= 0 and Game.GetGameState() == GameplayGameStateTypes.GAMESTATE_ON ) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TurnsRemaining.lua - DLC_04 DLC}}
:<code>DLC/DLC_04/Scenarios/1066Scenario/TurnsRemaining.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0032}}<syntaxhighlight lang="lua">if (iTurnsRemaining < 1 or Game.GetGameState() == GameplayGameStateTypes.GAMESTATE_EXTENDED) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0073}}<syntaxhighlight lang="lua">if (Game:GetGameState() ~= GameplayGameStateTypes.GAMESTATE_EXTENDED) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TurnsRemaining.lua (G&K)}}
:<code>DLC/Expansion/Scenarios/SteampunkScenario/TurnsRemaining.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0121}}<syntaxhighlight lang="lua">local gameState = Game.GetGameState();</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetGameState]]