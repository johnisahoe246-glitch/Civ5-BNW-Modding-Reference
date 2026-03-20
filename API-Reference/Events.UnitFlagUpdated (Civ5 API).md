{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Events}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''void''' Events.UnitFlagUpdated<b>(</b>'''int''' unitCulture, '''int''' unitType, '''float''' unitHealth, '''bool''' unitFortified<b>)</b></code>


'''Event Type'''
:Regular event: you can subscribe to it through <code>Events.UnitFlagUpdated.Add(''<function handler>'')</code> or invoke it directly through <code>Events.UnitFlagUpdated(''<arguments list>'')</code>.

'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|unitCulture:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|unitType:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|unitHealth:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|unitFortified:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|DebugMode.lua}}
:<code>UI/InGame/DebugMode.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0513}}<syntaxhighlight lang="lua">Events.UnitFlagUpdated( g_iUnitCulture, g_iUnitType, g_fUnitHealth, g_bUnitFortified );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|UnitList.lua}}
:<code>UI/InGame/UnitList.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0084}}<syntaxhighlight lang="lua">Events.UnitFlagUpdated.Add( OnChangeEvent );</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|UnitFlagUpdated]]
[[Category:Civ5 Units API|UnitFlagUpdated]]