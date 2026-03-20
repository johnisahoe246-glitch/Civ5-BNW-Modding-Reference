{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Game}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>{{Type5|PlayerID}} Game.GetGameTurn<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|CityStateDiploPopup.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/Popups/CityStateDiploPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0507}}<syntaxhighlight lang="lua">local iTurnsCommitted = (pPlayer:GetTurnLastPledgedProtectionByMajor(iActivePlayer) + 10) - Game.GetGameTurn(); --antonjs: todo: xml</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0521}}<syntaxhighlight lang="lua">local iTurnsUntilRecovered = (iLastTurnPledgeBroken + 20) - Game.GetGameTurn(); --antonjs: todo: xml</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CityStateStatusHelper.lua (G&K)}}
:<code>DLC/Expansion/UI/CityStateStatusHelper.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0477}}<syntaxhighlight lang="lua">local iTurnsRemaining = pMinor:GetQuestTurnsRemaining(iMajor, eType, Game.GetGameTurn() - 1); -- add 1 since began on CS's turn (1 before), and avoids "0 turns remaining"</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CivsAlive.lua - DLC_01 DLC}}
:<code>DLC/DLC_01/Scenarios/Mongol Scenario/CivsAlive.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0007}}<syntaxhighlight lang="lua">local iTurnsRemaining = 100 - Game.GetGameTurn();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ReplayViewer.lua}}
:<code>UI/InGame/Popups/ReplayViewer.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1250}}<syntaxhighlight lang="lua">local finalTurn = Game.GetGameTurn();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TopPanel.lua}}
:<code>UI/InGame/TopPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0205}}<syntaxhighlight lang="lua">local turn = Locale.ConvertTextKey("TXT_KEY_TP_TURN_COUNTER", Game.GetGameTurn());</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TurnsRemaining.lua - DLC_02 DLC}}
:<code>DLC/DLC_02/Scenarios/NewWorldScenario/TurnsRemaining.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0311}}<syntaxhighlight lang="lua">local iGameTurn = Game.GetGameTurn();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TurnsRemaining.lua - DLC_04 DLC}}
:<code>DLC/DLC_04/Scenarios/1066Scenario/TurnsRemaining.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0006}}<syntaxhighlight lang="lua">local iTurnsRemaining = 70 - Game.GetGameTurn();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0235}}<syntaxhighlight lang="lua">local iTemp = math.floor(Game.GetGameTurn() / iValue);</syntaxhighlight>
{{CodeLine5|0236}}<syntaxhighlight lang="lua">if (Game.GetGameTurn() > 0 and Game.GetGameTurn()< 51 and iTemp * iValue == Game.GetGameTurn()) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TurnsRemaining.lua (G&K)}}
:<code>DLC/Expansion/Scenarios/FallOfRomeScenario/TurnsRemaining.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0014}}<syntaxhighlight lang="lua">local iTurnsRemaining = g_iGameTurnLength - Game.GetGameTurn();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TurnsRemaining.lua (G&K)}}
:<code>DLC/Expansion/Scenarios/MedievalScenario/TurnsRemaining.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0081}}<syntaxhighlight lang="lua">local iTurnsRemaining = 200 - Game.GetGameTurn();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0146}}<syntaxhighlight lang="lua">local iTurn = Game.GetGameTurn();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TurnsRemaining.lua (G&K)}}
:<code>DLC/Expansion/Scenarios/SteampunkScenario/TurnsRemaining.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0089}}<syntaxhighlight lang="lua">local strStatus = Locale.Lookup("TXT_KEY_STEAMPUNK_SCENARIO_TURNS_REMAINING", GetNumTokensOwned(iActivePlayer), GetNumTokensUnlocked(Game.GetGameTurn() - 1)); --antonjs: consider: keep var for last turn updated</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0419}}<syntaxhighlight lang="lua">LuaEvents.ScenarioPlayerStatusChanged(tCopy, Game.GetGameTurn(), Game.GetGameTurnYear(), giPlayerAboutToWin, giTurnsControlHeld);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0454}}<syntaxhighlight lang="lua">LuaEvents.ScenarioPlayerStatusChanged(tCopy, Game.GetGameTurn(), Game.GetGameTurnYear(), -1, 0);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0485}}<syntaxhighlight lang="lua">if (IsTokenUnlocked(sToken, Game.GetGameTurn() - 1)) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0795}}<syntaxhighlight lang="lua">LuaEvents.ScenarioPlayerStatusChanged(tPlayerStatusCopy, Game.GetGameTurn() - 1, Game.GetGameTurnYear() - 1, giPlayerAboutToWin, giTurnsControlHeld); --antonjs: todo: save and load the turn and year</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TutorialChecks.lua}}
:<code>Tutorial/TutorialChecks.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0082}}<syntaxhighlight lang="lua">if (Game.GetGameTurn() > 0) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0236}}<syntaxhighlight lang="lua">if (Game.GetGameTurn() > 100) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0240}}<syntaxhighlight lang="lua">if (Game.GetGameTurn() < 25) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0496}}<syntaxhighlight lang="lua">if (Game.GetGameTurn() > 50 or player:GetNumMilitaryUnits() >= 2) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0629}}<syntaxhighlight lang="lua">if (Game.GetGameTurn() >= 100) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0719}}<syntaxhighlight lang="lua">if (Game.GetGameTurn() - mostRecentLastMoveTurn >= 3) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0966}}<syntaxhighlight lang="lua">if (Game.GetGameTurn() >= 150) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1980}}<syntaxhighlight lang="lua">if (Game.GetGameTurn() >= 20) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|2617}}<syntaxhighlight lang="lua">if (Game.GetGameTurn() - Game.GetStartTurn() > 10) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TutorialEngine.lua}}
:<code>Tutorial/TutorialEngine.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0291}}<syntaxhighlight lang="lua">local gameTurn = Game.GetGameTurn();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|WonderPopup.lua}}
:<code>UI/InGame/Popups/WonderPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0026}}<syntaxhighlight lang="lua">if(Game == nil or Game.GetGameTurn() <= Game.GetStartTurn()) then</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetGameTurn]]