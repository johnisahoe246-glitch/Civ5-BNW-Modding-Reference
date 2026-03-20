{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|OptionsManager}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''void''' OptionsManager.SetGridOn_Cached<b>(</b>'''bool''' isChecked<b>)</b></code>


'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|isChecked:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|MiniMapPanel.lua}}
:<code>UI/InGame/WorldView/MiniMapPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0111}}<syntaxhighlight lang="lua">OptionsManager.SetGridOn_Cached( mapOptions.ShowGrid );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0317}}<syntaxhighlight lang="lua">OptionsManager.SetGridOn_Cached( bIsChecked );</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|SetGridOn_Cached]]