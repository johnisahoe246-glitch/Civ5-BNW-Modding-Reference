{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Plot}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''int''' Plot:IsAdjacentToShallowWater<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|MapGenerator.lua (G&K)}}
:<code>DLC/Expansion/Gameplay/Lua/MapGenerator.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0207}}<syntaxhighlight lang="lua">if(plot:IsAdjacentToShallowWater() and Map.Rand(iExpansionDiceroll, "add shallows") == 0) then</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|IsAdjacentToShallowWater]]
[[Category:Civ5 Terrain API|IsAdjacentToShallowWater]]