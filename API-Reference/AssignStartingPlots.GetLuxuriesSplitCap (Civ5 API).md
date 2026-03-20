{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|AssignStartingPlots}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''int''' AssignStartingPlots:GetLuxuriesSplitCap<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
{{PseudoH4|AssignStartingPlots.lua (G&K)}}
:<code>DLC/Expansion/Gameplay/Lua/AssignStartingPlots.lua</code>
:{{CodeBegin5}}
{{CodeLine5|7722}}<syntaxhighlight lang="lua">local split_cap = self:GetLuxuriesSplitCap() -- New for expansion. Cap no longer set to hardcoded value of 3.</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|7724}}<syntaxhighlight lang="lua">for index, resource_options in ipairs(luxury_candidates) do</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetLuxuriesSplitCap]]