{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a built-in global function. No <code>include</code> statement is needed.
}}


=Usage=
<code>'''void''' SetStrategicViewOverlay<b>(</b>'''int''' index<b>)</b></code>


'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|index:
|valign="top"| ''No description available.''
|}


=Source code samples=
{{PseudoH4|MiniMapPanel.lua}}
:<code>UI/InGame/WorldView/MiniMapPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0135}}<syntaxhighlight lang="lua">SetStrategicViewOverlay( mapOptions.SVOverlayMode );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0214}}<syntaxhighlight lang="lua">SetStrategicViewOverlay(index);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|SetStrategicViewOverlay]]