{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a global function. Use: <code>include("MapGenerator.lua")</code>
}}


=Usage=
<code>'''void''' DoRiver<b>(</b>{{Type5|Plot}} startPlot, {{Type5|FlowDirectionType}} thisFlowDirection = nil, {{Type5|FlowDirectionType}} originalFlowDirection = nil, '''int''' riverID = nil<b>)</b></code>


'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|startPlot:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|thisFlowDirection:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|originalFlowDirection:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|riverID:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|Great_Plains.lua}}
:<code>Maps/Great_Plains.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0863}}<syntaxhighlight lang="lua">DoRiver(inlandCorner, nil, orig_direction, nil);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|MapGenerator.lua (G&K)}}
:<code>DLC/Expansion/Gameplay/Lua/MapGenerator.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0493}}<syntaxhighlight lang="lua">DoRiver(riverPlot, bestFlowDirection, originalFlowDirection, riverID);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0544}}<syntaxhighlight lang="lua">DoRiver(inlandCorner);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|DoRiver]]
[[Category:Civ5 Rivers API|DoRiver]]