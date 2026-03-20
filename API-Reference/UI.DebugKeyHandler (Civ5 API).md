{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|UI}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''void''' UI.DebugKeyHandler<b>(</b>{{Type5|KeyEventType}} uiMsg, {{Type5|KeyType}} wParam, '''unknown''' lParam<b>)</b></code>


'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|uiMsg:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|wParam:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|lParam:
|valign="top"| ''No description available.''
|}


=Source code samples=
{{PseudoH4|DebugMenu.lua}}
:<code>UI/InGame/DebugMenu.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0399}}<syntaxhighlight lang="lua">UI.DebugKeyHandler( uiMsg, wParam, lParam );</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|DebugKeyHandler]]