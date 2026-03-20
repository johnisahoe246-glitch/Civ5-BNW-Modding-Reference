{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|OptionsManager}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''bool''' OptionsManager.IsNoTileRecommendations<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|InGame.lua}}
:<code>UI/InGame/InGame.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0277}}<syntaxhighlight lang="lua">local value = not OptionsManager.IsNoTileRecommendations();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0345}}<syntaxhighlight lang="lua">if (not OptionsManager.IsNoTileRecommendations()) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|MiniMapPanel.lua}}
:<code>UI/InGame/WorldView/MiniMapPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0082}}<syntaxhighlight lang="lua">g_MapOptionDefaults.HideTileRecommendations = OptionsManager.IsNoTileRecommendations();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0122}}<syntaxhighlight lang="lua">if (OptionsManager.IsNoTileRecommendations() ~= mapOptions.HideTileRecommendations) then</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|IsNoTileRecommendations]]