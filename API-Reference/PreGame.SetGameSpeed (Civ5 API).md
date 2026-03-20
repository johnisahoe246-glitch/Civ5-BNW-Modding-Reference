{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|PreGame}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''void''' PreGame.SetGameSpeed<b>(</b>{{Type5|GameSpeedType}} id<b>)</b></code>


'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|id:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|AdvancedSetup.lua}}
:<code>UI/FrontEnd/GameSetup/AdvancedSetup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0528}}<syntaxhighlight lang="lua">PreGame.SetGameSpeed( id );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0797}}<syntaxhighlight lang="lua">PreGame.SetGameSpeed(wb.DefaultSpeed);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1229}}<syntaxhighlight lang="lua">PreGame.SetGameSpeed(gameSpeed.ID);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|GameSetupScreen.lua}}
:<code>UI/FrontEnd/GameSetup/GameSetupScreen.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0400}}<syntaxhighlight lang="lua">PreGame.SetGameSpeed(preview.DefaultSpeed);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|LoadTutorial.lua}}
:<code>UI/FrontEnd/LoadTutorial.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0104}}<syntaxhighlight lang="lua">PreGame.SetGameSpeed(2); -- standard</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|MedievalScenarioLoadScreen.lua (G&K)}}
:<code>DLC/Expansion/Scenarios/MedievalScenario/MedievalScenarioLoadScreen.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0056}}<syntaxhighlight lang="lua">PreGame.SetGameSpeed(3);  -- Quick speed</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|MPGameOptions.lua}}
:<code>UI/FrontEnd/Multiplayer/GameSetup/MPGameOptions.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0112}}<syntaxhighlight lang="lua">PreGame.SetGameSpeed(2);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|SteampunkScenarioLoadScreen.lua (G&K)}}
:<code>DLC/Expansion/Scenarios/SteampunkScenario/SteampunkScenarioLoadScreen.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0054}}<syntaxhighlight lang="lua">PreGame.SetGameSpeed(GameInfo.GameSpeeds["GAMESPEED_STANDARD"].ID);  -- Quick speed</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|SetGameSpeed]]