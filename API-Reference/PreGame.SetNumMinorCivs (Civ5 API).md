{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|PreGame}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''void''' PreGame.SetNumMinorCivs<b>(</b>'''int''' numMinorCivsWanted<b>)</b></code>


'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|numMinorCivsWanted:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|AdvancedSetup.lua}}
:<code>UI/FrontEnd/GameSetup/AdvancedSetup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0611}}<syntaxhighlight lang="lua">PreGame.SetNumMinorCivs( mapSize.DefaultMinorCivs );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0789}}<syntaxhighlight lang="lua">PreGame.SetNumMinorCivs(mapScript.DefaultCityStates);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0799}}<syntaxhighlight lang="lua">PreGame.SetNumMinorCivs(wb.CityStateCount);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0803}}<syntaxhighlight lang="lua">PreGame.SetNumMinorCivs(-1);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0932}}<syntaxhighlight lang="lua">PreGame.SetNumMinorCivs( math.floor( fValue * maxMinorCivs ) );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0946}}<syntaxhighlight lang="lua">PreGame.SetNumMinorCivs(GameInfo.Worlds[ PreGame.GetWorldSize() ].DefaultMinorCivs);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1210}}<syntaxhighlight lang="lua">PreGame.SetNumMinorCivs( worldSize.DefaultMinorCivs );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|MedievalScenarioLoadScreen.lua (G&K)}}
:<code>DLC/Expansion/Scenarios/MedievalScenario/MedievalScenarioLoadScreen.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0089}}<syntaxhighlight lang="lua">PreGame.SetNumMinorCivs(25);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|MPGameOptions.lua}}
:<code>UI/FrontEnd/Multiplayer/GameSetup/MPGameOptions.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0465}}<syntaxhighlight lang="lua">PreGame.SetNumMinorCivs(GameInfo.Worlds[id].DefaultMinorCivs);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0734}}<syntaxhighlight lang="lua">PreGame.SetNumMinorCivs(numMinorCivsWanted);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|SelectMapSize.lua}}
:<code>UI/FrontEnd/GameSetup/SelectMapSize.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0039}}<syntaxhighlight lang="lua">PreGame.SetNumMinorCivs( GameInfo.Worlds[ id ].DefaultMinorCivs );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|SelectMapType.lua}}
:<code>UI/FrontEnd/GameSetup/SelectMapType.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0075}}<syntaxhighlight lang="lua">PreGame.SetNumMinorCivs( world.DefaultMinorCivs );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|SteampunkScenarioLoadScreen.lua (G&K)}}
:<code>DLC/Expansion/Scenarios/SteampunkScenario/SteampunkScenarioLoadScreen.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0053}}<syntaxhighlight lang="lua">PreGame.SetNumMinorCivs(10);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|SetNumMinorCivs]]
[[Category:Civ5 Players API|SetNumMinorCivs]]
[[Category:Civ5 City States API|SetNumMinorCivs]]