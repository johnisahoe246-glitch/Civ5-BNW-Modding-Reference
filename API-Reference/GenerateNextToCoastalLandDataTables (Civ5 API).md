{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a global function. Use: <code>include("MapmakerUtilities.lua")</code>
}}


=Usage=
<code>table('''int''' => '''bool'''), table('''int''' => '''int''') GenerateNextToCoastalLandDataTables<b>(</b><b>)</b></code>


'''Returned Values'''
:No description available.


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|AssignStartingPlots.lua (G&K)}}
:<code>DLC/Expansion/Gameplay/Lua/AssignStartingPlots.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0514}}<syntaxhighlight lang="lua">self.plotDataIsCoastal, self.plotDataIsNextToCoast = GenerateNextToCoastalLandDataTables()</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0516}}<syntaxhighlight lang="lua">-- Set up data for resource ID shortcuts.</syntaxhighlight>
{{CodeLine5|0517}}<syntaxhighlight lang="lua">for resource_data in GameInfo.Resources() do</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GenerateNextToCoastalLandDataTables]]
[[Category:Civ5 Terrain API|GenerateNextToCoastalLandDataTables]]