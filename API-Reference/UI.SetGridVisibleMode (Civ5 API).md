{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|UI}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''void''' UI.SetGridVisibleMode<b>(</b>'''bool''' isChecked<b>)</b></code>


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
{{CodeLine5|0101}}<syntaxhighlight lang="lua">UI.SetGridVisibleMode( mapOptions.ShowGrid );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0313}}<syntaxhighlight lang="lua">UI.SetGridVisibleMode(bIsChecked);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|SetGridVisibleMode]]
[[Category:Civ5 Fog API|SetGridVisibleMode]]