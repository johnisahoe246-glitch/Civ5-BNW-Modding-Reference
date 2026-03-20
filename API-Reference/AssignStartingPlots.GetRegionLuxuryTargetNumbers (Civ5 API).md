{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|AssignStartingPlots}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''unknown''' AssignStartingPlots:GetRegionLuxuryTargetNumbers<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|AssignStartingPlots.lua (G&K)}}
:<code>DLC/Expansion/Gameplay/Lua/AssignStartingPlots.lua</code>
:{{CodeBegin5}}
{{CodeLine5|8711}}<syntaxhighlight lang="lua">local target_list = self:GetRegionLuxuryTargetNumbers()</syntaxhighlight>
{{CodeLine5|8712}}<syntaxhighlight lang="lua">local targetNum = math.floor((target_list[self.iNumCivs] + (0.5 * self.luxury_low_fert_compensation[res_ID])) / assignment_split);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetRegionLuxuryTargetNumbers]]
[[Category:Civ5 Combat API|GetRegionLuxuryTargetNumbers]]