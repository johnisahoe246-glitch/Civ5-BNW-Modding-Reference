{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This method is declared by {{Type5|ReplayMap}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''void''' UIElement:SetPlot<b>(</b>'''int''' x, '''int''' y, {{Type5|TerrainType}} terrain, '''int''' r, '''int''' g, '''int''' b, '''int''' a<b>)</b></code>


'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|x:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|y:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|terrain:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|r:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|g:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|b:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|a:
|valign="top"| ''No description available.''
|}


=Source code samples=
{{PseudoH4|ReplayViewer.lua}}
:<code>UI/InGame/Popups/ReplayViewer.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1017}}<syntaxhighlight lang="lua">replayMapControl:SetPlot(x, y, terrainType, plotColor.Red, plotColor.Green, plotColor.Blue, plotColor.Alpha);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|SetPlot]]