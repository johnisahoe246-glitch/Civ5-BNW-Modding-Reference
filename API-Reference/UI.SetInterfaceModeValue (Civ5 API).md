{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|UI}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''void''' UI.SetInterfaceModeValue<b>(</b>{{Type5|PlayerID}} minorCiv<b>)</b></code>


'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|minorCiv:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|CityStateDiploPopup.lua}}
:<code>UI/InGame/Popups/CityStateDiploPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0575}}<syntaxhighlight lang="lua">UI.SetInterfaceModeValue(g_iMinorCivID);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|SetInterfaceModeValue]]