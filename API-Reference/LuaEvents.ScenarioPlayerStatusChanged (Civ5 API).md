{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|LuaEvents}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''void''' LuaEvents.ScenarioPlayerStatusChanged<b>(</b>table({{Type5|PlayerID}} => table('''string''' => '''table''')) tPlayerStatus, {{Type5|PlayerID}} turn, '''int''' year, {{Type5|PlayerID}} playerAboutToWin, '''int''' turnsControlHeld<b>)</b></code>


'''Event Type'''
:Regular event: you can subscribe to it through <code>LuaEvents.ScenarioPlayerStatusChanged.Add(''<function handler>'')</code> or invoke it directly through <code>LuaEvents.ScenarioPlayerStatusChanged(''<arguments list>'')</code>.

'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|tPlayerStatus:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|turn:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|year:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|playerAboutToWin:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|turnsControlHeld:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|TurnsRemaining.lua (G&K)}}
:<code>DLC/Expansion/Scenarios/SteampunkScenario/TurnsRemaining.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0419}}<syntaxhighlight lang="lua">LuaEvents.ScenarioPlayerStatusChanged(tCopy, Game.GetGameTurn(), Game.GetGameTurnYear(), giPlayerAboutToWin, giTurnsControlHeld);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0454}}<syntaxhighlight lang="lua">LuaEvents.ScenarioPlayerStatusChanged(tCopy, Game.GetGameTurn(), Game.GetGameTurnYear(), -1, 0);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0564}}<syntaxhighlight lang="lua">LuaEvents.ScenarioPlayerStatusChanged.Add( ReceivePlayerStatusChanged );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0795}}<syntaxhighlight lang="lua">LuaEvents.ScenarioPlayerStatusChanged(tPlayerStatusCopy, Game.GetGameTurn() - 1, Game.GetGameTurnYear() - 1, giPlayerAboutToWin, giTurnsControlHeld); --antonjs: todo: save and load the turn and year</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|ScenarioPlayerStatusChanged]]
[[Category:Civ5 Players API|ScenarioPlayerStatusChanged]]