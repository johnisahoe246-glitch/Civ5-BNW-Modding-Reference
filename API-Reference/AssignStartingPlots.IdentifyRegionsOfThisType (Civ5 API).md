{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|AssignStartingPlots}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''void''' AssignStartingPlots:IdentifyRegionsOfThisType<b>(</b>'''int''' region_type<b>)</b></code>


'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|region_type:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|AssignStartingPlots.lua (G&K)}}
:<code>DLC/Expansion/Gameplay/Lua/AssignStartingPlots.lua</code>
:{{CodeBegin5}}
{{CodeLine5|7704}}<syntaxhighlight lang="lua">self:IdentifyRegionsOfThisType(check_this_type)</syntaxhighlight>
{{CodeLine5|7705}}<syntaxhighlight lang="lua">end</syntaxhighlight>
{{CodeLine5|7706}}<syntaxhighlight lang="lua">self:IdentifyRegionsOfThisType(0) -- If any Undefined Regions, put them at the bottom of the list.</syntaxhighlight>
{{CodeLine5|7707}}<syntaxhighlight lang="lua">end</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|IdentifyRegionsOfThisType]]