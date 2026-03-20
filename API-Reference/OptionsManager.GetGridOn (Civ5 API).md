{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|OptionsManager}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''bool''' OptionsManager.GetGridOn<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|InGame.lua}}
:<code>UI/InGame/InGame.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0320}}<syntaxhighlight lang="lua">if (not OptionsManager.GetGridOn()) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|MiniMapPanel.lua}}
:<code>UI/InGame/WorldView/MiniMapPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0041}}<syntaxhighlight lang="lua">Controls.ShowGrid:SetCheck(OptionsManager.GetGridOn());</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0079}}<syntaxhighlight lang="lua">g_MapOptionDefaults.ShowGrid = OptionsManager.GetGridOn();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0110}}<syntaxhighlight lang="lua">if (OptionsManager.GetGridOn() ~= mapOptions.ShowGrid) then</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetGridOn]]