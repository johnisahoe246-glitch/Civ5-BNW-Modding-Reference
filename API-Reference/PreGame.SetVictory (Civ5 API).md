{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|PreGame}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''void''' PreGame.SetVictory<b>(</b>{{Type5|VictoryType}} arg0, '''bool''' check<b>)</b></code>


'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|arg0:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|check:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|AdvancedSetup.lua}}
:<code>UI/FrontEnd/GameSetup/AdvancedSetup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0811}}<syntaxhighlight lang="lua">PreGame.SetVictory(row.ID, victories[row.Type]);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1063}}<syntaxhighlight lang="lua">PreGame.SetVictory(row.ID, bCheck);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1247}}<syntaxhighlight lang="lua">PreGame.SetVictory(row.ID, true);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|MedievalScenarioLoadScreen.lua (G&K)}}
:<code>DLC/Expansion/Scenarios/MedievalScenario/MedievalScenarioLoadScreen.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0070}}<syntaxhighlight lang="lua">PreGame.SetVictory(row.ID, false);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|MongolScenarioLoadScreen.lua - DLC_01 DLC}}
:<code>DLC/DLC_01/Scenarios/Mongol Scenario/MongolScenarioLoadScreen.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0045}}<syntaxhighlight lang="lua">PreGame.SetVictory(victory.ID, true);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|SetVictory]]
[[Category:Civ5 Victory API|SetVictory]]