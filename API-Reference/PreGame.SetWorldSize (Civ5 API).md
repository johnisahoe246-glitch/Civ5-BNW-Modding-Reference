{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|PreGame}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''void''' PreGame.SetWorldSize<b>(</b>{{Type5|HandicapType}} id<b>)</b></code>


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
{{CodeLine5|0610}}<syntaxhighlight lang="lua">PreGame.SetWorldSize( id );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0801}}<syntaxhighlight lang="lua">PreGame.SetWorldSize(wb.MapSize);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1209}}<syntaxhighlight lang="lua">PreGame.SetWorldSize( worldSize.ID );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|LoadMenu.lua}}
:<code>UI/FrontEnd/LoadMenu.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0061}}<syntaxhighlight lang="lua">PreGame.SetWorldSize( worldInfo.ID );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|LoadTutorial.lua}}
:<code>UI/FrontEnd/LoadTutorial.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0102}}<syntaxhighlight lang="lua">PreGame.SetWorldSize(0);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|MedievalScenarioLoadScreen.lua (G&K)}}
:<code>DLC/Expansion/Scenarios/MedievalScenario/MedievalScenarioLoadScreen.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0087}}<syntaxhighlight lang="lua">PreGame.SetWorldSize(GameInfo.Worlds.WORLDSIZE_HUGE.ID);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|MPGameOptions.lua}}
:<code>UI/FrontEnd/Multiplayer/GameSetup/MPGameOptions.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0090}}<syntaxhighlight lang="lua">PreGame.SetWorldSize(1);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0464}}<syntaxhighlight lang="lua">PreGame.SetWorldSize(id);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|SelectMapType.lua}}
:<code>UI/FrontEnd/GameSetup/SelectMapType.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0074}}<syntaxhighlight lang="lua">PreGame.SetWorldSize( mapInfo.MapSize );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|SteampunkScenarioLoadScreen.lua (G&K)}}
:<code>DLC/Expansion/Scenarios/SteampunkScenario/SteampunkScenarioLoadScreen.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0058}}<syntaxhighlight lang="lua">PreGame.SetWorldSize(GameInfo.Worlds.WORLDSIZE_SMALL.ID);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|SetWorldSize]]
[[Category:Civ5 Game Settings API|SetWorldSize]]