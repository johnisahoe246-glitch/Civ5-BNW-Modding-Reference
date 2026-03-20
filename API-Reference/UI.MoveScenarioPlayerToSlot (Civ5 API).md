{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|UI}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''void''' UI.MoveScenarioPlayerToSlot<b>(</b>{{Type5|UnitType}} playerIndex, '''int''' arg1<b>)</b></code>


'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|playerIndex:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|arg1:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|FoRScenarioLoadScreen.lua (G&K)}}
:<code>DLC/Expansion/Scenarios/FallOfRomeScenario/FoRScenarioLoadScreen.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0067}}<syntaxhighlight lang="lua">UI.MoveScenarioPlayerToSlot( playerIndex, 0 );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|GameSetupScreen.lua}}
:<code>UI/FrontEnd/GameSetup/GameSetupScreen.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0408}}<syntaxhighlight lang="lua">UI.MoveScenarioPlayerToSlot(i - 1, 0);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|MongolScenarioLoadScreen.lua - DLC_01 DLC}}
:<code>DLC/DLC_01/Scenarios/Mongol Scenario/MongolScenarioLoadScreen.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0054}}<syntaxhighlight lang="lua">UI.MoveScenarioPlayerToSlot(0, 0);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|SelectCivilization.lua}}
:<code>UI/FrontEnd/GameSetup/SelectCivilization.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0067}}<syntaxhighlight lang="lua">UI.MoveScenarioPlayerToSlot( scenarioPlayerID, 0 );</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|MoveScenarioPlayerToSlot]]
[[Category:Civ5 Movement API|MoveScenarioPlayerToSlot]]
[[Category:Civ5 Players API|MoveScenarioPlayerToSlot]]
[[Category:Civ5 Game Settings API|MoveScenarioPlayerToSlot]]