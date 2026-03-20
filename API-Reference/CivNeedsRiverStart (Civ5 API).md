{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a global function. Use: <code>include("MapmakerUtilities.lua")</code>
}}


=Usage=
<code>'''bool''' CivNeedsRiverStart<b>(</b>'''string''' civType<b>)</b></code>


'''Returned Value'''
:No description available.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|civType:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|AssignStartingPlots.lua (G&K)}}
:<code>DLC/Expansion/Gameplay/Lua/AssignStartingPlots.lua</code>
:{{CodeBegin5}}
{{CodeLine5|4648}}<syntaxhighlight lang="lua">local bNeedsRiverStart = CivNeedsRiverStart(civType)</syntaxhighlight>
{{CodeLine5|4649}}<syntaxhighlight lang="lua">if bNeedsRiverStart == true then</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|CivNeedsRiverStart]]
[[Category:Civ5 Rivers API|CivNeedsRiverStart]]