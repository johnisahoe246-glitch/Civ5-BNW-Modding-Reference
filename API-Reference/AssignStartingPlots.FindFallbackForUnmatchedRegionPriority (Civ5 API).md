{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|AssignStartingPlots}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''int''' AssignStartingPlots:FindFallbackForUnmatchedRegionPriority<b>(</b>'''int''' regionType, table('''int''' => {{Type5|PlayerID}}) regions_still_available<b>)</b></code>


'''Returned Value'''
:No description available.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|regionType:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|regions_still_available:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|AssignStartingPlots.lua (G&K)}}
:<code>DLC/Expansion/Gameplay/Lua/AssignStartingPlots.lua</code>
:{{CodeBegin5}}
{{CodeLine5|5044}}<syntaxhighlight lang="lua">local choose_this_region = self:FindFallbackForUnmatchedRegionPriority(iPriorityType, regions_still_available)</syntaxhighlight>
{{CodeLine5|5045}}<syntaxhighlight lang="lua">if choose_this_region == -1 then</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|FindFallbackForUnmatchedRegionPriority]]