{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|PreGame}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>{{Type5|HandicapType}} PreGame.GetWorldSize<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|AdvancedSetup.lua}}
:<code>UI/FrontEnd/GameSetup/AdvancedSetup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0632}}<syntaxhighlight lang="lua">local info = GameInfo.Worlds[ PreGame.GetWorldSize() ];</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0946}}<syntaxhighlight lang="lua">PreGame.SetNumMinorCivs(GameInfo.Worlds[ PreGame.GetWorldSize() ].DefaultMinorCivs);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|MPGameOptions.lua}}
:<code>UI/FrontEnd/Multiplayer/GameSetup/MPGameOptions.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0071}}<syntaxhighlight lang="lua">if (PreGame.GetWorldSize() >= 0) then</syntaxhighlight>
{{CodeLine5|0072}}<syntaxhighlight lang="lua">return GameInfo.Worlds[ PreGame.GetWorldSize() ].DefaultPlayers;</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|MPGameSetupScreen.lua}}
:<code>UI/FrontEnd/Multiplayer/GameSetup/MPGameSetupScreen.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0047}}<syntaxhighlight lang="lua">local worldInfo = GameInfo.Worlds[ PreGame.GetWorldSize() ];</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|SaveMapMenu.lua}}
:<code>UI/InGame/Menus/SaveMapMenu.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0042}}<syntaxhighlight lang="lua">SetSaveInfo(PreGame.GetWorldSize() );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0124}}<syntaxhighlight lang="lua">SetSaveInfo(PreGame.GetWorldSize());</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|SaveMenu.lua}}
:<code>UI/InGame/Menus/SaveMenu.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0072}}<syntaxhighlight lang="lua">PreGame.GetHandicap(), PreGame.GetWorldSize(), PreGame.GetMapScript(), nil,</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|SinglePlayer.lua}}
:<code>UI/FrontEnd/SinglePlayer.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0073}}<syntaxhighlight lang="lua">info = GameInfo.Worlds[ PreGame.GetWorldSize() ];</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetWorldSize]]
[[Category:Civ5 Game Settings API|GetWorldSize]]