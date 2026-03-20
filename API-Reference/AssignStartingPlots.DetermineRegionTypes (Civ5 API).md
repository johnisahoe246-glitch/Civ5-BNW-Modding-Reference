{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|AssignStartingPlots}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''void''' AssignStartingPlots:DetermineRegionTypes<b>(</b><b>)</b></code>




=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|AssignStartingPlots.lua (G&K)}}
:<code>DLC/Expansion/Gameplay/Lua/AssignStartingPlots.lua</code>
:{{CodeBegin5}}
{{CodeLine5|3393}}<syntaxhighlight lang="lua">self:DetermineRegionTypes()</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|3395}}<syntaxhighlight lang="lua">-- Set up list of regions (to be processed in this order).</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|3397}}<syntaxhighlight lang="lua">-- First, make a list of all average fertility values...</syntaxhighlight>
{{CodeLine5|3398}}<syntaxhighlight lang="lua">local regionAssignList = {};</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|DetermineRegionTypes]]