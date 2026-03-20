{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a global function. Use: <code>include("MapmakerUtilities.lua")</code>
}}


=Usage=
<code>table('''int''' => '''bool''') GenerateCoastalLandDataTable<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
{{PseudoH4|MapmakerUtilities.lua}}
:<code>Gameplay/Lua/MapmakerUtilities.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0357}}<syntaxhighlight lang="lua">local plotDataIsCoastal = GenerateCoastalLandDataTable()</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0359}}<syntaxhighlight lang="lua">-- Set up data table for IsNextToCoast</syntaxhighlight>
{{CodeLine5|0360}}<syntaxhighlight lang="lua">local iW, iH = Map.GetGridSize();</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GenerateCoastalLandDataTable]]
[[Category:Civ5 Terrain API|GenerateCoastalLandDataTable]]