{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Path}}.<br/>
This is a static method, invoke it with a dot.
}}


Obtains the filename without the extension for a given path
This method returns the name of the file, minus extension, in a given path.


=Usage=
<code>'''string''' Path.GetFileNameWithoutExtension<b>(</b>'''string''' path<b>)</b></code>


'''Returned Value'''
:The name of the file in the path, minus the extension or an empty string on error.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|path:
|valign="top"| ''An absolute or relative path to a file.''
|}


=Examples=
<syntaxhighlight lang="lua" class="civ5-example">
local path = "C:\\temp\\foo.bar";
print(Path.GetFileNameWithoutExtension(path)); -- prints "foo"</syntaxhighlight>


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|AdvancedSetup.lua}}
:<code>UI/FrontEnd/GameSetup/AdvancedSetup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0714}}<syntaxhighlight lang="lua">name = Path.GetFileNameWithoutExtension(map.File);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|GameSetupScreen.lua}}
:<code>UI/FrontEnd/GameSetup/GameSetupScreen.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0339}}<syntaxhighlight lang="lua">local mapName = Path.GetFileNameWithoutExtension(mapScriptFileName);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0343}}<syntaxhighlight lang="lua">mapName = Path.GetFileNameWithoutExtension(mapScriptFileName);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|LoadMenu.lua}}
:<code>UI/FrontEnd/LoadMenu.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0353}}<syntaxhighlight lang="lua">name = Path.GetFileNameWithoutExtension(header.MapScript);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0507}}<syntaxhighlight lang="lua">return Path.GetFileNameWithoutExtension(file);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|LoadReplayMenu.lua}}
:<code>UI/FrontEnd/LoadReplayMenu.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0148}}<syntaxhighlight lang="lua">local name = Path.GetFileNameWithoutExtension(g_FileList[g_iSelected]);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0414}}<syntaxhighlight lang="lua">local displayName = Path.GetFileNameWithoutExtension(v);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|Lobby.lua}}
:<code>UI/FrontEnd/Multiplayer/Lobby.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0252}}<syntaxhighlight lang="lua">local serverMapFileName = Path.GetFileNameWithoutExtension(serverMapFile);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0258}}<syntaxhighlight lang="lua">local mapFileName = Path.GetFileNameWithoutExtension(row.FileName);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0282}}<syntaxhighlight lang="lua">name = Path.GetFileNameWithoutExtension(serverMapFile);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|MPGameOptions.lua}}
:<code>UI/FrontEnd/Multiplayer/GameSetup/MPGameOptions.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0251}}<syntaxhighlight lang="lua">local fileTitle = Path.GetFileNameWithoutExtension(PreGame.GetMapScript());</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0616}}<syntaxhighlight lang="lua">mapName = Path.GetFileNameWithoutExtension(v[1]);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|SaveMenu.lua}}
:<code>UI/InGame/Menus/SaveMenu.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0309}}<syntaxhighlight lang="lua">name = Path.GetFileNameWithoutExtension(mapScript);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetFileNameWithoutExtension]]