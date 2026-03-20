{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Plot}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''int''' Plot:GetNumFriendlyUnitsOfType<b>(</b>{{Type5|Unit}} unit<b>)</b></code>


'''Returned Value'''
:No description available.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|unit:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|UnitPanel.lua}}
:<code>UI/InGame/WorldView/UnitPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1018}}<syntaxhighlight lang="lua">if (pPlot:GetNumFriendlyUnitsOfType(unit) > 1) then</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetNumFriendlyUnitsOfType]]
[[Category:Civ5 Units API|GetNumFriendlyUnitsOfType]]