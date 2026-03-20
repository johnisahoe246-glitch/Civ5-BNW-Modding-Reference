{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Plot}}.<br/>
This is an instance method, invoke it with a colon.<br/>
Places a river on the southwest side of this plot.
}}


=Usage=
<code>'''void''' Plot:SetNEOfRiver<b>(</b>'''bool''' newValue, '''{{Type5|FlowDirectionType}}''' flowDirection<b>)</b></code>

Note that this function is placing a river on the southwest side of the plot not the northeast side. The function name is a bit confusing, but just remember that it's saying the plot is relative to the river and not the other way around.


'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|newValue:
|valign="top"| ''Not sure what this does but it always seems to be set to true.''
|-
|valign="top" style="padding-right:6px;"|flowDirection:
|valign="top"| ''The direction the river is flowing. Will be either FLOWDIRECTION_NORTHWEST or FLOWDIRECTION_SOUTHEAST. If your river is flowing the wrong way, you can reverse it by using the opposite direction. See {{Func5|GetOppositeFlowDirection}}.''
|}

=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|Amazon_XP.lua (G&K)}}
:<code>DLC/Expansion/Maps/Amazon_XP.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0483}}<syntaxhighlight lang="lua">riverPlot:SetNEOfRiver(true, thisFlowDirection);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|SetNEOfRiver]]
[[Category:Civ5 Rivers API|SetNEOfRiver]]