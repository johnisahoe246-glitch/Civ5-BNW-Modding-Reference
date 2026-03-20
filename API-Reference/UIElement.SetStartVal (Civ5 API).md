{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This method is declared by {{Type5|Line}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''void''' UIElement:SetStartVal<b>(</b>'''int''' startX, '''int''' startY<b>)</b></code>


'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|startX:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|startY:
|valign="top"| ''No description available.''
|}


=Source code samples=
{{PseudoH4|ReplayViewer.lua}}
:<code>UI/InGame/Popups/ReplayViewer.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0351}}<syntaxhighlight lang="lua">horizontalMouseCrosshair:SetStartVal(0, y);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0354}}<syntaxhighlight lang="lua">verticalMouseCrosshair:SetStartVal(x, 0);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0357}}<syntaxhighlight lang="lua">horizontalMouseGuide:SetStartVal(graphDisplayWidth, y);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0360}}<syntaxhighlight lang="lua">verticalMouseGuide:SetStartVal(x, graphDisplayHeight);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0439}}<syntaxhighlight lang="lua">lineSegment.LineSegment:SetStartVal(startX, startY);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|SetStartVal]]