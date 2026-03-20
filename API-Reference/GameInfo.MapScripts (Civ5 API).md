{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|GameInfo}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>iterator({{Type5|MapScriptInfo}}) GameInfo.MapScripts<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|AdvancedSetup.lua}}
:<code>UI/FrontEnd/GameSetup/AdvancedSetup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0625}}<syntaxhighlight lang="lua">for row in GameInfo.MapScripts{FileName = filename} do</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0678}}<syntaxhighlight lang="lua">for row in GameInfo.MapScripts{SupportsSinglePlayer = 1} do</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0843}}<syntaxhighlight lang="lua">for row in GameInfo.MapScripts{FileName = mapScriptFileName} do</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1216}}<syntaxhighlight lang="lua">local mapScript = GameInfo.MapScripts{FileName = "Assets\\Maps\\Continents.lua"}();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|GameMenu.lua}}
:<code>UI/InGame/Menus/GameMenu.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0225}}<syntaxhighlight lang="lua">for row in GameInfo.MapScripts{FileName = mapScript, Hidden = 0} do</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0349}}<syntaxhighlight lang="lua">for row in GameInfo.MapScripts() do</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|LoadMenu.lua}}
:<code>UI/FrontEnd/LoadMenu.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0315}}<syntaxhighlight lang="lua">for row in GameInfo.MapScripts{FileName = header.MapScript, SupportsSinglePlayer = 1, Hidden = 0} do</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|MPGameOptions.lua}}
:<code>UI/FrontEnd/Multiplayer/GameSetup/MPGameOptions.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0105}}<syntaxhighlight lang="lua">for row in GameInfo.MapScripts{SupportsMultiplayer = 1} do</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|SaveMapMenu.lua}}
:<code>UI/InGame/Menus/SaveMapMenu.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0140}}<syntaxhighlight lang="lua">for row in GameInfo.MapScripts{FileName = mapScript} do</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|SaveMenu.lua}}
:<code>UI/InGame/Menus/SaveMenu.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0273}}<syntaxhighlight lang="lua">for row in GameInfo.MapScripts{FileName = mapScript, SupportsSinglePlayer = 1, Hidden = 0} do</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|SelectMapType.lua}}
:<code>UI/FrontEnd/GameSetup/SelectMapType.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0247}}<syntaxhighlight lang="lua">for row in GameInfo.MapScripts{FileName = fileName, SupportsSinglePlayer = 1, Hidden = 0} do</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|SinglePlayer.lua}}
:<code>UI/FrontEnd/SinglePlayer.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0049}}<syntaxhighlight lang="lua">for mapScript in GameInfo.MapScripts() do</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|MapScripts]]