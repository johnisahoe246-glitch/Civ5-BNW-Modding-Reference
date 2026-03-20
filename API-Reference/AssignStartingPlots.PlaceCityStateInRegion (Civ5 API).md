{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|AssignStartingPlots}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''void''' AssignStartingPlots:PlaceCityStateInRegion<b>(</b>'''int''' city_state_number, {{Type5|PlayerID}} region_number<b>)</b></code>


'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|city_state_number:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|region_number:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|AssignStartingPlots.lua (G&K)}}
:<code>DLC/Expansion/Gameplay/Lua/AssignStartingPlots.lua</code>
:{{CodeBegin5}}
{{CodeLine5|6703}}<syntaxhighlight lang="lua">self:PlaceCityStateInRegion(cs_number, iRandRegion)</syntaxhighlight>
{{CodeLine5|6704}}<syntaxhighlight lang="lua">else -- Assigned to a Region.</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|6706}}<syntaxhighlight lang="lua">self:PlaceCityStateInRegion(cs_number, region_number)</syntaxhighlight>
{{CodeLine5|6707}}<syntaxhighlight lang="lua">end</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|PlaceCityStateInRegion]]
[[Category:Civ5 Cities API|PlaceCityStateInRegion]]