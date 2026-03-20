{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Events}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''void''' Events.UnitDataEdited<b>(</b>'''int''' floatVarList, '''int''' memberCount, '''int''' memberIndex, '''bool''' isDebugFSM, {{Type5|SpecialistType}} specRender, '''bool''' isFromLua = nil<b>)</b></code>


'''Event Type'''
:Regular event: you can subscribe to it through <code>Events.UnitDataEdited.Add(''<function handler>'')</code> or invoke it directly through <code>Events.UnitDataEdited(''<arguments list>'')</code>.

'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|floatVarList:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|memberCount:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|memberIndex:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|isDebugFSM:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|specRender:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|isFromLua:
|valign="top"| ''No description available.''
|}


=Source code samples=
{{PseudoH4|DebugMode.lua}}
:<code>UI/InGame/DebugMode.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0690}}<syntaxhighlight lang="lua">Events.UnitDataEdited( g_tFloatVarList, g_iUnitMemberCount, g_iUnitMemberIndex-1, false, g_iUnitSpecularRender );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0713}}<syntaxhighlight lang="lua">Events.UnitDataEdited.Add( OnFloatVarListTransfer );</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|UnitDataEdited]]
[[Category:Civ5 Units API|UnitDataEdited]]