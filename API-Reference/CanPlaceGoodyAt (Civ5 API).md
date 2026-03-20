{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a global function. Use: <code>include("MapGenerator.lua")</code>
}}


=Usage=
<code>'''bool''' CanPlaceGoodyAt<b>(</b>{{Type5|ImprovementType}} improvement, {{Type5|Plot}} plot<b>)</b></code>


'''Returned Value'''
:No description available.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|improvement:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|plot:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|MapGenerator.lua (G&K)}}
:<code>DLC/Expansion/Gameplay/Lua/MapGenerator.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0703}}<syntaxhighlight lang="lua">if (CanPlaceGoodyAt(improvement, plot)) then</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|CanPlaceGoodyAt]]
[[Category:Civ5 Goodies API|CanPlaceGoodyAt]]