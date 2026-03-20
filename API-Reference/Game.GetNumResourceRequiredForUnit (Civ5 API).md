{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Game}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''int''' Game.GetNumResourceRequiredForUnit<b>(</b>{{Type5|UnitType}} unit, {{Type5|ResourceType}} resource<b>)</b></code>


'''Returned Value'''
:No description available.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|unit:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|resource:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|InfoTooltipInclude.lua}}
:<code>UI/InGame/InfoTooltipInclude.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0051}}<syntaxhighlight lang="lua">iNumResourceNeeded = Game.GetNumResourceRequiredForUnit(iUnitID, iResourceID);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetNumResourceRequiredForUnit]]
[[Category:Civ5 Resources API|GetNumResourceRequiredForUnit]]
[[Category:Civ5 Units API|GetNumResourceRequiredForUnit]]