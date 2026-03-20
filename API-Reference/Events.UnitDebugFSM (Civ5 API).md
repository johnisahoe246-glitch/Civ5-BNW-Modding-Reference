{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Events}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''void''' Events.UnitDebugFSM<b>(</b>'''int''' arg0<b>)</b></code>


'''Event Type'''
:Regular event: you can subscribe to it through <code>Events.UnitDebugFSM.Add(''<function handler>'')</code> or invoke it directly through <code>Events.UnitDebugFSM(''<arguments list>'')</code>.

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
{{CodeLine5|0682}}<syntaxhighlight lang="lua">Events.UnitDebugFSM( g_iUnitMemberIndex-1 );</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|UnitDebugFSM]]
[[Category:Civ5 Units API|UnitDebugFSM]]