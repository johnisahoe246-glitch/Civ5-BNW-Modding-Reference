{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Events}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''void''' Events.UnitTypeChanged<b>(</b>'''string''' arg0<b>)</b></code>


'''Event Type'''
:Regular event: you can subscribe to it through <code>Events.UnitTypeChanged.Add(''<function handler>'')</code> or invoke it directly through <code>Events.UnitTypeChanged(''<arguments list>'')</code>.

'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|arg0:
|valign="top"| ''No description available.''
|}


=Source code samples=
{{PseudoH4|DebugMode.lua}}
:<code>UI/InGame/DebugMode.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0207}}<syntaxhighlight lang="lua">Events.UnitTypeChanged("ART_DEF_UNIT_" .. ArtInfo.Units[g_iCreateCommonGreatUnitType].Type);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0223}}<syntaxhighlight lang="lua">Events.UnitTypeChanged("ART_DEF_UNIT_U_" .. ArtInfo.UniqueUnits[g_iCreateUniqueUnitType].Type);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|UnitTypeChanged]]
[[Category:Civ5 Units API|UnitTypeChanged]]