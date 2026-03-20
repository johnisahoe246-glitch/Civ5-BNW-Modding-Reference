{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|PreGame}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>{{Type5|CivilizationType}} PreGame.GetCivilization<b>(</b>{{Type5|PlayerID}} i = nil<b>)</b></code>


'''Returned Value'''
:No description available.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|i:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|AdvancedSetup.lua}}
:<code>UI/FrontEnd/GameSetup/AdvancedSetup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0294}}<syntaxhighlight lang="lua">local civIndex = PreGame.GetCivilization( i );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0333}}<syntaxhighlight lang="lua">local civIndex = PreGame.GetCivilization(0);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1131}}<syntaxhighlight lang="lua">local civIndex = PreGame.GetCivilization( 0 );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|GameSetupScreen.lua}}
:<code>UI/FrontEnd/GameSetup/GameSetupScreen.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0188}}<syntaxhighlight lang="lua">local civIndex = PreGame.GetCivilization(i);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|IconSupport.lua}}
:<code>UI/IconSupport.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0143}}<syntaxhighlight lang="lua">local thisCivType = PreGame.GetCivilization( playerID );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|LoadScreen.lua}}
:<code>UI/FrontEnd/LoadScreen.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0040}}<syntaxhighlight lang="lua">local civIndex = PreGame.GetCivilization( Game:GetActivePlayer() );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|MPGameOptions.lua}}
:<code>UI/FrontEnd/Multiplayer/GameSetup/MPGameOptions.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0367}}<syntaxhighlight lang="lua">local curCiv = PreGame.GetCivilization(0);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|SaveMenu.lua}}
:<code>UI/InGame/Menus/SaveMenu.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0071}}<syntaxhighlight lang="lua">SetSaveInfoToCiv(PreGame.GetCivilization(), PreGame.GetGameSpeed(), PreGame.GetEra(), 0,</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0194}}<syntaxhighlight lang="lua">SetSaveInfoToCiv(PreGame.GetCivilization(), PreGame.GetGameSpeed(), PreGame.GetEra(), Game.GetElapsedGameTurns(),</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0628}}<syntaxhighlight lang="lua">local civ = PreGame.GetCivilization();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|SetCivNames.lua}}
:<code>UI/FrontEnd/GameSetup/SetCivNames.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0021}}<syntaxhighlight lang="lua">local civIndex = PreGame.GetCivilization( g_EditSlot );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|StagingRoom.lua}}
:<code>UI/FrontEnd/Multiplayer/StagingRoom.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0075}}<syntaxhighlight lang="lua">local civIndex = PreGame.GetCivilization( Matchmaking.GetLocalID() );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0322}}<syntaxhighlight lang="lua">local civIndex = PreGame.GetCivilization( playerID );</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetCivilization]]
[[Category:Civ5 Players API|GetCivilization]]