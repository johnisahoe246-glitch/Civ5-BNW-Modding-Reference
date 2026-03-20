{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Game}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''int''' Game.Rand<b>(</b>'''int''' max_num, '''string''' log<b>)</b></code>


'''Returned Value'''
:No description available.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|max_num:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|log:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|TurnsRemaining.lua - DLC_02 DLC}}
:<code>DLC/DLC_02/Scenarios/NewWorldScenario/TurnsRemaining.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0106}}<syntaxhighlight lang="lua">if (Game.Rand(100, "Rolling for treasure") < 80) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0110}}<syntaxhighlight lang="lua">if (Game.Rand(100, "Rolling for treasure") < 70) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0114}}<syntaxhighlight lang="lua">if (Game.Rand(100, "Rolling for treasure") < 60) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0118}}<syntaxhighlight lang="lua">if (Game.Rand(100, "Rolling for treasure") < 50) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0324}}<syntaxhighlight lang="lua">local iRandom = Game.Rand(20, "Delay between natural wonder treasures");</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TurnsRemaining.lua - DLC_04 DLC}}
:<code>DLC/DLC_04/Scenarios/1066Scenario/TurnsRemaining.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0577}}<syntaxhighlight lang="lua">local iRand = Game.Rand(5, "Norman attack target");</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0627}}<syntaxhighlight lang="lua">local iRand = Game.Rand(5, "Danish attack target");</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TurnsRemaining.lua (G&K)}}
:<code>DLC/Expansion/Scenarios/FallOfRomeScenario/TurnsRemaining.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0426}}<syntaxhighlight lang="lua">local iRandChoice = Game.Rand(iCounter, "Choosing which city to drop an army on");</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|2208}}<syntaxhighlight lang="lua">local iSwapIndex = Game.Rand(iNumMissions, "Scrambling mission order") + 1;</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|WhosWinningPopup.lua}}
:<code>UI/InGame/Popups/WhosWinningPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0068}}<syntaxhighlight lang="lua">local iRand = Game.Rand(#g_tListOfDudes, "Rolling to determine Progress Screen dude.");</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0088}}<syntaxhighlight lang="lua">iRand = Game.Rand(#g_tListModeText+1, "Rolling to determine Progress Screen list type.");</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|Rand]]