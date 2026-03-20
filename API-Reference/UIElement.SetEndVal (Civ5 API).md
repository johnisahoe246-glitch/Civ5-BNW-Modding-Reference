{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This method is declared by {{Type5|Line}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''void''' UIElement:SetEndVal<b>(</b>'''int''' newX, '''int''' newY<b>)</b></code>


'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|newX:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|newY:
|valign="top"| ''No description available.''
|}


=Source code samples=
{{PseudoH4|ReplayViewer.lua}}
:<code>UI/InGame/Popups/ReplayViewer.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0352}}<syntaxhighlight lang="lua">horizontalMouseCrosshair:SetEndVal(graphDisplayWidth, y);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0355}}<syntaxhighlight lang="lua">verticalMouseCrosshair:SetEndVal(x, graphDisplayHeight);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0358}}<syntaxhighlight lang="lua">horizontalMouseGuide:SetEndVal(horizontalMouseGuideEnd, y);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0361}}<syntaxhighlight lang="lua">verticalMouseGuide:SetEndVal(x, verticalMouseGuideEnd);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0528}}<syntaxhighlight lang="lua">lineSegment.LineSegment:SetEndVal(newX, newY);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0542}}<syntaxhighlight lang="lua">lineSegment.LineSegment:SetEndVal(endX, endY);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|SetEndVal]]