{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|AssignStartingPlots}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''void''' AssignStartingPlots:AddExtraBonusesToHillsRegions<b>(</b><b>)</b></code>




=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|Amazon_XP.lua (G&K)}}
:<code>DLC/Expansion/Maps/Amazon_XP.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1509}}<syntaxhighlight lang="lua">self:AddExtraBonusesToHillsRegions()</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1511}}<syntaxhighlight lang="lua">local resources_to_place = {</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|Great_Plains.lua}}
:<code>Maps/Great_Plains.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1486}}<syntaxhighlight lang="lua">self:AddExtraBonusesToHillsRegions()</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1488}}<syntaxhighlight lang="lua">-- Great Plains, Buffalo Herds</syntaxhighlight>
{{CodeLine5|1489}}<syntaxhighlight lang="lua">print("Placing Buffalo Herds (Cows - Lua Great Plains) ...")</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|AddExtraBonusesToHillsRegions]]
[[Category:Civ5 Terrain API|AddExtraBonusesToHillsRegions]]