{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|UI}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>{{Type5|WorldBuilderMapData}} UI.GetMapPreview<b>(</b>'''string''' mapFilePath<b>)</b></code>


'''Returned Value'''
:No description available.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|mapFilePath:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|AdvancedSetup.lua}}
:<code>UI/FrontEnd/GameSetup/AdvancedSetup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0700}}<syntaxhighlight lang="lua">local mapData = UI.GetMapPreview(map.File);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|GameMenu.lua}}
:<code>UI/InGame/Menus/GameMenu.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0257}}<syntaxhighlight lang="lua">local mapData = UI.GetMapPreview(mapScript);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|GameSetupScreen.lua}}
:<code>UI/FrontEnd/GameSetup/GameSetupScreen.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0336}}<syntaxhighlight lang="lua">local mapInfo = UI.GetMapPreview(mapScriptFileName);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0398}}<syntaxhighlight lang="lua">local preview = UI.GetMapPreview(mapFileName);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|LoadMenu.lua}}
:<code>UI/FrontEnd/LoadMenu.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0347}}<syntaxhighlight lang="lua">local mapData = UI.GetMapPreview(header.MapScript);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|Lobby.lua}}
:<code>UI/FrontEnd/Multiplayer/Lobby.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0274}}<syntaxhighlight lang="lua">local mapData = UI.GetMapPreview(serverMapFile);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|MPGameOptions.lua}}
:<code>UI/FrontEnd/Multiplayer/GameSetup/MPGameOptions.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0610}}<syntaxhighlight lang="lua">local mapInfo = UI.GetMapPreview(v[1]);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|SaveMapMenu.lua}}
:<code>UI/InGame/Menus/SaveMapMenu.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0118}}<syntaxhighlight lang="lua">SetSaveInfo(UI.GetMapPreview(entry.File).MapSize, date);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|SelectMapType.lua}}
:<code>UI/FrontEnd/GameSetup/SelectMapType.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0068}}<syntaxhighlight lang="lua">local mapInfo = UI.GetMapPreview(mapScript);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|SinglePlayer.lua}}
:<code>UI/FrontEnd/SinglePlayer.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0057}}<syntaxhighlight lang="lua">local mapData = UI.GetMapPreview(savedMapScript);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetMapPreview]]