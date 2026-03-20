{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|AssignStartingPlots}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''unknown''' AssignStartingPlots:ChopIntoThreeRegions<b>(</b>'''unknown''' fertility_table, '''table''' rectangle_data_table, '''bool''' taller, '''unknown''' chopPercent = nil<b>)</b></code>


'''Returned Value'''
:No description available.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|fertility_table:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|rectangle_data_table:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|taller:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|chopPercent:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|AssignStartingPlots.lua (G&K)}}
:<code>DLC/Expansion/Gameplay/Lua/AssignStartingPlots.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1198}}<syntaxhighlight lang="lua">local results = self:ChopIntoThreeRegions(fertility_table, rectangle_data_table, bTaller);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|ChopIntoThreeRegions]]