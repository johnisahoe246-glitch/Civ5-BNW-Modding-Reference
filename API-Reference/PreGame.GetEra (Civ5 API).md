{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|PreGame}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>{{Type5|EraType}} PreGame.GetEra<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|AdvancedSetup.lua}}
:<code>UI/FrontEnd/GameSetup/AdvancedSetup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0497}}<syntaxhighlight lang="lua">local info = GameInfo.Eras[ PreGame.GetEra() ];</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|GameMenu.lua}}
:<code>UI/InGame/Menus/GameMenu.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0338}}<syntaxhighlight lang="lua">if(PreGame.GetEra() ~= nil) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0341}}<syntaxhighlight lang="lua">controlTable.Text:LocalizeAndSetText("TXT_KEY_START_ERA", Locale.ConvertTextKey(GameInfo.Eras[PreGame.GetEra()].Description));</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|SaveMenu.lua}}
:<code>UI/InGame/Menus/SaveMenu.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0071}}<syntaxhighlight lang="lua">SetSaveInfoToCiv(PreGame.GetCivilization(), PreGame.GetGameSpeed(), PreGame.GetEra(), 0,</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0194}}<syntaxhighlight lang="lua">SetSaveInfoToCiv(PreGame.GetCivilization(), PreGame.GetGameSpeed(), PreGame.GetEra(), Game.GetElapsedGameTurns(),</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|StagingRoom.lua}}
:<code>UI/FrontEnd/Multiplayer/StagingRoom.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0908}}<syntaxhighlight lang="lua">Controls.StartEraLabel:SetText( Locale.ConvertTextKey( GameInfo.Eras[ PreGame.GetEra() ].Description ) );</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetEra]]