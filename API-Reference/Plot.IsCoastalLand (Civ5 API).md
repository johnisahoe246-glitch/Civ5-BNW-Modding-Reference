{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Plot}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''bool''' Plot:IsCoastalLand<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|Amazon_XP.lua (G&K)}}
:<code>DLC/Expansion/Maps/Amazon_XP.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0343}}<syntaxhighlight lang="lua">if plot:IsCoastalLand() then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0817}}<syntaxhighlight lang="lua">return (not plot:IsCoastalLand()) and (Map.Rand(8, "MapGenerator AddRivers") == 0);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|MapGenerator.lua (G&K)}}
:<code>DLC/Expansion/Gameplay/Lua/MapGenerator.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0562}}<syntaxhighlight lang="lua">if not plot:IsCoastalLand() then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|West_vs_East.lua}}
:<code>Maps/West_vs_East.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0202}}<syntaxhighlight lang="lua">return (not plot:IsCoastalLand()) and (Map.Rand(8, "AddRivers Lua") == 0);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|IsCoastalLand]]
[[Category:Civ5 Terrain API|IsCoastalLand]]