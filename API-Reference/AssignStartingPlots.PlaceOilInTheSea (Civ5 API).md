{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|AssignStartingPlots}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''void''' AssignStartingPlots:PlaceOilInTheSea<b>(</b><b>)</b></code>




=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|Amazon_XP.lua (G&K)}}
:<code>DLC/Expansion/Maps/Amazon_XP.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1464}}<syntaxhighlight lang="lua">self:PlaceOilInTheSea()</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1467}}<syntaxhighlight lang="lua">-- Check for low or missing Strategic resources</syntaxhighlight>
{{CodeLine5|1468}}<syntaxhighlight lang="lua">if self.amounts_of_resources_placed[self.iron_ID + 1] < 8 then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|AssignStartingPlots.lua (G&K)}}
:<code>DLC/Expansion/Gameplay/Lua/AssignStartingPlots.lua</code>
:{{CodeBegin5}}
{{CodeLine5|9715}}<syntaxhighlight lang="lua">self:PlaceOilInTheSea();</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|PlaceOilInTheSea]]
[[Category:Civ5 Terrain API|PlaceOilInTheSea]]