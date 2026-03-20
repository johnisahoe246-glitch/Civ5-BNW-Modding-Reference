{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|OptionsManager}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''bool''' OptionsManager.GetResourceOn<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
{{PseudoH4|MiniMapPanel.lua}}
:<code>UI/InGame/WorldView/MiniMapPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0081}}<syntaxhighlight lang="lua">g_MapOptionDefaults.ShowResources = OptionsManager.GetResourceOn();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0118}}<syntaxhighlight lang="lua">if (OptionsManager.GetResourceOn() ~= mapOptions.ShowResources) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ResourceIconManager.lua}}
:<code>UI/InGame/ResourceIconManager.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0013}}<syntaxhighlight lang="lua">local g_bHideResourceIcons = not OptionsManager.GetResourceOn();</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetResourceOn]]
[[Category:Civ5 Resources API|GetResourceOn]]