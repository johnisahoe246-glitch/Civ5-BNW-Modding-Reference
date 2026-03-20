{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|PreGame}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''string''' PreGame.GetMapScript<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|AdvancedSetup.lua}}
:<code>UI/FrontEnd/GameSetup/AdvancedSetup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0043}}<syntaxhighlight lang="lua">local currentMapScript = PreGame.GetMapScript();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0184}}<syntaxhighlight lang="lua">for option in DB.Query("select * from MapScriptOptions where not exists (select 1 from MapScriptOptionPossibleValues where FileName = MapScriptOptions.FileName and OptionID = MapScriptOptions.OptionID) and Hidden = 0 and FileName = ?", PreGame.GetMapScript()) do</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0624}}<syntaxhighlight lang="lua">local filename = PreGame.GetMapScript();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0842}}<syntaxhighlight lang="lua">local mapScriptFileName = PreGame.GetMapScript();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|GameMenu.lua}}
:<code>UI/InGame/Menus/GameMenu.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0222}}<syntaxhighlight lang="lua">local mapScript = PreGame.GetMapScript();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|GameSetupScreen.lua}}
:<code>UI/FrontEnd/GameSetup/GameSetupScreen.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0024}}<syntaxhighlight lang="lua">if( bIsModding and IsWBMap(PreGame.GetMapScript()) ) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|MPGameOptions.lua}}
:<code>UI/FrontEnd/Multiplayer/GameSetup/MPGameOptions.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0054}}<syntaxhighlight lang="lua">local mapScriptFileName = Locale.ToLower(PreGame.GetMapScript());</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0251}}<syntaxhighlight lang="lua">local fileTitle = Path.GetFileNameWithoutExtension(PreGame.GetMapScript());</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|SaveMenu.lua}}
:<code>UI/InGame/Menus/SaveMenu.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0072}}<syntaxhighlight lang="lua">PreGame.GetHandicap(), PreGame.GetWorldSize(), PreGame.GetMapScript(), nil,</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|SelectCivilization.lua}}
:<code>UI/FrontEnd/GameSetup/SelectCivilization.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0025}}<syntaxhighlight lang="lua">local isWBMap = IsWBMap(PreGame.GetMapScript());</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0069}}<syntaxhighlight lang="lua">local playerList = UI.GetMapPlayers(PreGame.GetMapScript());</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0159}}<syntaxhighlight lang="lua">local civList = UI.GetMapPlayers(PreGame.GetMapScript());</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|SinglePlayer.lua}}
:<code>UI/FrontEnd/SinglePlayer.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0046}}<syntaxhighlight lang="lua">local savedMapScript = PreGame.GetMapScript();</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetMapScript]]
[[Category:Civ5 Game Settings API|GetMapScript]]