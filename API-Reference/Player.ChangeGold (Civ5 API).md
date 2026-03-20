{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Player}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''void''' Player:ChangeGold<b>(</b>'''int''' change<b>)</b></code>


'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|change:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|CivsAlive.lua - DLC_01 DLC}}
:<code>DLC/DLC_01/Scenarios/Mongol Scenario/CivsAlive.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0117}}<syntaxhighlight lang="lua">Players[0]:ChangeGold(500);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0123}}<syntaxhighlight lang="lua">Players[0]:ChangeGold(1000);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TurnsRemaining.lua - DLC_02 DLC}}
:<code>DLC/DLC_02/Scenarios/NewWorldScenario/TurnsRemaining.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0173}}<syntaxhighlight lang="lua">player:ChangeGold(iGoldReceived);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TurnsRemaining.lua - DLC_04 DLC}}
:<code>DLC/DLC_04/Scenarios/1066Scenario/TurnsRemaining.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0262}}<syntaxhighlight lang="lua">pPlayer:ChangeGold (iGold);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0538}}<syntaxhighlight lang="lua">player:ChangeGold (500);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0588}}<syntaxhighlight lang="lua">player:ChangeGold (1000);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0638}}<syntaxhighlight lang="lua">player:ChangeGold (1500);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0681}}<syntaxhighlight lang="lua">player:ChangeGold (2000);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0725}}<syntaxhighlight lang="lua">player:ChangeGold (2500);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TurnsRemaining.lua (G&K)}}
:<code>DLC/Expansion/Scenarios/FallOfRomeScenario/TurnsRemaining.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0261}}<syntaxhighlight lang="lua">Players[iPlayer]:ChangeGold(iDiv);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|ChangeGold]]
[[Category:Civ5 Gold API|ChangeGold]]