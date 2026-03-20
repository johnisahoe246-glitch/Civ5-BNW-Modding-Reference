{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a global function. Use: <code>include("MapmakerUtilities.lua")</code>
}}


=Usage=
<code>'''int''' AdjacentToSaltWater<b>(</b>'''int''' x, '''int''' y<b>)</b></code>


'''Returned Value'''
:No description available.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|x:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|y:
|valign="top"| ''No description available.''
|}


=Source code samples=
{{PseudoH4|MapmakerUtilities.lua}}
:<code>Gameplay/Lua/MapmakerUtilities.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0343}}<syntaxhighlight lang="lua">local plotIsAdjacent = AdjacentToSaltWater(x, y)</syntaxhighlight>
{{CodeLine5|0344}}<syntaxhighlight lang="lua">if plotIsAdjacent then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|NaturalWondersCustomMethods.lua (G&K)}}
:<code>DLC/Expansion/Gameplay/Lua/NaturalWondersCustomMethods.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0087}}<syntaxhighlight lang="lua">if plot:IsWater() == false and AdjacentToSaltWater(x, y) == false then</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|AdjacentToSaltWater]]
[[Category:Civ5 Terrain API|AdjacentToSaltWater]]