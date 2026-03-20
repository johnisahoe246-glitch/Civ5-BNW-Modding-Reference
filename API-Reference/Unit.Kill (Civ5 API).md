{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Unit}}.<br/>
This is an instance method, invoke it with a colon.
}}

Removes a unit from the game.

=Usage=
<code>'''void''' Unit:Kill<b>(</b>'''bool''' delay = false, {{Type5|PlayerID}} player = NO_PLAYER<b>)</b></code>


'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|delay:
|valign="top"| ''If true, the unit will be partially cleaned up, but its final removal will happen at the end of the frame. But what use does this have?''
|-
|valign="top" style="padding-right:6px;"|player:
|valign="top"| ''Player ID of the player that has killed this unit or -1 for no player.''
|}

=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|TurnsRemaining.lua - DLC_02 DLC}}
:<code>DLC/DLC_02/Scenarios/NewWorldScenario/TurnsRemaining.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0156}}<syntaxhighlight lang="lua">unit:Kill(true, -1);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TurnsRemaining.lua - DLC_04 DLC}}
:<code>DLC/DLC_04/Scenarios/1066Scenario/TurnsRemaining.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0207}}<syntaxhighlight lang="lua">unit:Kill();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0470}}<syntaxhighlight lang="lua">pPlot:GetUnit(0):Kill(true, -1);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TurnsRemaining.lua (G&K)}}
:<code>DLC/Expansion/Scenarios/FallOfRomeScenario/TurnsRemaining.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1043}}<syntaxhighlight lang="lua">pPlot:GetUnit(0):Kill(false, -1);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TurnsRemaining.lua (G&K)}}
:<code>DLC/Expansion/Scenarios/MedievalScenario/TurnsRemaining.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1078}}<syntaxhighlight lang="lua">pUnit:Kill();</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|Kill]]