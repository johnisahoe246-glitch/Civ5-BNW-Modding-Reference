{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Game}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''int''' Game.GetGameTurnYear<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|ChooseReligionPopup.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/Popups/ChooseReligionPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0484}}<syntaxhighlight lang="lua">local year = Game.GetGameTurnYear();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TurnsRemaining.lua (G&K)}}
:<code>DLC/Expansion/Scenarios/MedievalScenario/TurnsRemaining.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0162}}<syntaxhighlight lang="lua">if (Game.GetGameTurnYear() > 1514) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TurnsRemaining.lua (G&K)}}
:<code>DLC/Expansion/Scenarios/SteampunkScenario/TurnsRemaining.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0419}}<syntaxhighlight lang="lua">LuaEvents.ScenarioPlayerStatusChanged(tCopy, Game.GetGameTurn(), Game.GetGameTurnYear(), giPlayerAboutToWin, giTurnsControlHeld);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0454}}<syntaxhighlight lang="lua">LuaEvents.ScenarioPlayerStatusChanged(tCopy, Game.GetGameTurn(), Game.GetGameTurnYear(), -1, 0);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0795}}<syntaxhighlight lang="lua">LuaEvents.ScenarioPlayerStatusChanged(tPlayerStatusCopy, Game.GetGameTurn() - 1, Game.GetGameTurnYear() - 1, giPlayerAboutToWin, giTurnsControlHeld); --antonjs: todo: save and load the turn and year</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetGameTurnYear]]