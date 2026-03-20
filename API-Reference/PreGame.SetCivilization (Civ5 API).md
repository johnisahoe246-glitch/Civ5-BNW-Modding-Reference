{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|PreGame}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''void''' PreGame.SetCivilization<b>(</b>{{Type5|PlayerID}} player, {{Type5|CivilizationType}} civ = nil<b>)</b></code>


'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|player:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|civ:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|AdvancedSetup.lua}}
:<code>UI/FrontEnd/GameSetup/AdvancedSetup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0439}}<syntaxhighlight lang="lua">PreGame.SetCivilization( playerID, civID);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1158}}<syntaxhighlight lang="lua">PreGame.SetCivilization(i, -1);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|GameSetupScreen.lua}}
:<code>UI/FrontEnd/GameSetup/GameSetupScreen.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0051}}<syntaxhighlight lang="lua">PreGame.SetCivilization(0, -1);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0412}}<syntaxhighlight lang="lua">PreGame.SetCivilization(0, v.CivType);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|LoadTutorial.lua}}
:<code>UI/FrontEnd/LoadTutorial.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0071}}<syntaxhighlight lang="lua">PreGame.SetCivilization(playerID, civ.ID);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0075}}<syntaxhighlight lang="lua">PreGame.SetCivilization(playerID, -1);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0103}}<syntaxhighlight lang="lua">PreGame.SetCivilization(-1); -- random</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|MedievalScenarioLoadScreen.lua (G&K)}}
:<code>DLC/Expansion/Scenarios/MedievalScenario/MedievalScenarioLoadScreen.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0092}}<syntaxhighlight lang="lua">PreGame.SetCivilization(i, GameInfo.Civilizations[ScenarioCivilizations[i]].ID);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0102}}<syntaxhighlight lang="lua">PreGame.SetCivilization(0, GameInfo.Civilizations[ScenarioCivilizations[playerIndex]].ID);</syntaxhighlight>
{{CodeLine5|0103}}<syntaxhighlight lang="lua">PreGame.SetCivilization(playerIndex, GameInfo.Civilizations[ScenarioCivilizations[0]].ID);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0115}}<syntaxhighlight lang="lua">PreGame.SetCivilization(12, GameInfo.Civilizations["CIVILIZATION_MONGOL"].ID);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|MongolScenarioLoadScreen.lua - DLC_01 DLC}}
:<code>DLC/DLC_01/Scenarios/Mongol Scenario/MongolScenarioLoadScreen.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0026}}<syntaxhighlight lang="lua">PreGame.SetCivilization(-1);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|MPGameOptions.lua}}
:<code>UI/FrontEnd/Multiplayer/GameSetup/MPGameOptions.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0380}}<syntaxhighlight lang="lua">PreGame.SetCivilization(0, civList[1].CivType);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|SelectCivilization.lua}}
:<code>UI/FrontEnd/GameSetup/SelectCivilization.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0065}}<syntaxhighlight lang="lua">PreGame.SetCivilization( 0, civID );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|SetCivNames.lua}}
:<code>UI/FrontEnd/GameSetup/SetCivNames.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0188}}<syntaxhighlight lang="lua">PreGame.SetCivilization(g_EditSlot, -1);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|StagingRoom.lua}}
:<code>UI/FrontEnd/Multiplayer/StagingRoom.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0140}}<syntaxhighlight lang="lua">PreGame.SetCivilization( playerID, civID );</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|SetCivilization]]
[[Category:Civ5 Players API|SetCivilization]]