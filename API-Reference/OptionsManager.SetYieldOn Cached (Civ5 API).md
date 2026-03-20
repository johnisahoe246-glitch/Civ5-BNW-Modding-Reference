{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|OptionsManager}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''void''' OptionsManager.SetYieldOn_Cached<b>(</b>'''bool''' isChecked<b>)</b></code>


'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|isChecked:
|valign="top"| ''No description available.''
|}


=Source code samples=
{{PseudoH4|MiniMapPanel.lua}}
:<code>UI/InGame/WorldView/MiniMapPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0115}}<syntaxhighlight lang="lua">OptionsManager.SetYieldOn_Cached( mapOptions.ShowYield );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0355}}<syntaxhighlight lang="lua">OptionsManager.SetYieldOn_Cached( bIsChecked );</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|SetYieldOn_Cached]]
[[Category:Civ5 Yields API|SetYieldOn_Cached]]