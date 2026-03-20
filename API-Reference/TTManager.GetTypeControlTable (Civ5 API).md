{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|TTManager}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''void''' TTManager.GetTypeControlTable<b>(</b>'''string''' arg0, table('''unknown''' => '''unknown''') tipControlTable<b>)</b></code>


'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|arg0:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|tipControlTable:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|CivilopediaScreen.lua}}
:<code>UI/Civilopedia/CivilopediaScreen.lua</code>
:{{CodeBegin5}}
{{CodeLine5|6459}}<syntaxhighlight lang="lua">TTManager:GetTypeControlTable( "TypeRoundImage", tipControlTable );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|PlotHelpManager.lua}}
:<code>UI/InGame/PlotHelpManager.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0015}}<syntaxhighlight lang="lua">TTManager:GetTypeControlTable( "HexDetails", tipControls );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TopPanel.lua}}
:<code>UI/InGame/TopPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0305}}<syntaxhighlight lang="lua">TTManager:GetTypeControlTable( "TooltipTypeTopPanel", tipControlTable );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|UnitPanel.lua}}
:<code>UI/InGame/WorldView/UnitPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0839}}<syntaxhighlight lang="lua">TTManager:GetTypeControlTable( "TypeUnitAction", tipControlTable );</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetTypeControlTable]]