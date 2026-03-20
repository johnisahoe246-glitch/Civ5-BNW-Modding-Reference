{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|PreGame}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''void''' PreGame.SetMaxTurns<b>(</b>'''string''' arg0<b>)</b></code>


'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|arg0:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|AdvancedSetup.lua}}
:<code>UI/FrontEnd/GameSetup/AdvancedSetup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0798}}<syntaxhighlight lang="lua">PreGame.SetMaxTurns(wb.MaxTurns);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0902}}<syntaxhighlight lang="lua">PreGame.SetMaxTurns(0);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0909}}<syntaxhighlight lang="lua">PreGame.SetMaxTurns(Controls.MaxTurnsEdit:GetText());</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|MedievalScenarioLoadScreen.lua (G&K)}}
:<code>DLC/Expansion/Scenarios/MedievalScenario/MedievalScenarioLoadScreen.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0111}}<syntaxhighlight lang="lua">PreGame.SetMaxTurns(200);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|MPGameOptions.lua}}
:<code>UI/FrontEnd/Multiplayer/GameSetup/MPGameOptions.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0743}}<syntaxhighlight lang="lua">PreGame.SetMaxTurns( Controls.MaxTurnsEdit:GetText() );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0754}}<syntaxhighlight lang="lua">PreGame.SetMaxTurns(100);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|SetMaxTurns]]