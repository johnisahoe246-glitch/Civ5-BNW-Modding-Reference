{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a global function. Use: <code>include("MapGenerator.lua")</code>
}}


=Usage=
<code>'''...''' GetCoreMapOptions<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|Arborea.lua (G&K)}}
:<code>DLC/Expansion/Maps/Arborea.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0017}}<syntaxhighlight lang="lua">local world_age, temperature, rainfall, sea_level, resources = GetCoreMapOptions()</syntaxhighlight>
{{CodeLine5|0018}}<syntaxhighlight lang="lua">rainfall = {</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|Archipelago.lua}}
:<code>Maps/Archipelago.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0016}}<syntaxhighlight lang="lua">local world_age, temperature, rainfall, sea_level, resources = GetCoreMapOptions()</syntaxhighlight>
{{CodeLine5|0017}}<syntaxhighlight lang="lua">return {</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|Tilted_Axis.lua (G&K)}}
:<code>DLC/Expansion/Maps/Tilted_Axis.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0031}}<syntaxhighlight lang="lua">local world_age, temperature, rainfall, sea_level, resources = GetCoreMapOptions()</syntaxhighlight>
{{CodeLine5|0032}}<syntaxhighlight lang="lua">local sea_level = {</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetCoreMapOptions]]
[[Category:Civ5 Game Settings API|GetCoreMapOptions]]