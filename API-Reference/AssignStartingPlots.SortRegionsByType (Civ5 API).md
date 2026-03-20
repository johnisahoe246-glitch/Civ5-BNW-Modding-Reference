{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|AssignStartingPlots}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''void''' AssignStartingPlots:SortRegionsByType<b>(</b><b>)</b></code>




=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|Amazon_XP.lua (G&K)}}
:<code>DLC/Expansion/Maps/Amazon_XP.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1148}}<syntaxhighlight lang="lua">self:SortRegionsByType()</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1150}}<syntaxhighlight lang="lua">-- Assign a luxury to each region.</syntaxhighlight>
{{CodeLine5|1151}}<syntaxhighlight lang="lua">for index, region_info in ipairs(self.regions_sorted_by_type) do</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|AssignStartingPlots.lua (G&K)}}
:<code>DLC/Expansion/Gameplay/Lua/AssignStartingPlots.lua</code>
:{{CodeBegin5}}
{{CodeLine5|7885}}<syntaxhighlight lang="lua">self:SortRegionsByType() -- creates self.regions_sorted_by_type, which will be expanded to store all data regarding regional luxuries.</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|7887}}<syntaxhighlight lang="lua">-- Assign a luxury to each region.</syntaxhighlight>
{{CodeLine5|7888}}<syntaxhighlight lang="lua">for index, region_info in ipairs(self.regions_sorted_by_type) do</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|SortRegionsByType]]