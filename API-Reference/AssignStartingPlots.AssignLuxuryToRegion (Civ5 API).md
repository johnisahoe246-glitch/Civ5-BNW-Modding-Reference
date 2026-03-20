{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|AssignStartingPlots}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>{{Type5|ResourceType}} AssignStartingPlots:AssignLuxuryToRegion<b>(</b>{{Type5|PlayerID}} region_number<b>)</b></code>


'''Returned Value'''
:No description available.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|region_number:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|Amazon_XP.lua (G&K)}}
:<code>DLC/Expansion/Maps/Amazon_XP.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1153}}<syntaxhighlight lang="lua">local resource_ID = self:AssignLuxuryToRegion(region_number)</syntaxhighlight>
{{CodeLine5|1154}}<syntaxhighlight lang="lua">self.regions_sorted_by_type[index][2] = resource_ID; -- This line applies the assignment.</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|AssignLuxuryToRegion]]