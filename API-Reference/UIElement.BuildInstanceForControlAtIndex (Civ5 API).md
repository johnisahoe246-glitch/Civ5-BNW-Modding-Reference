{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This method is declared by {{Type5|Context}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''void''' UIElement:BuildInstanceForControlAtIndex<b>(</b>'''string''' arg0, '''table''' controlTable, {{Type5|Stack}} arg2, '''int''' arg3<b>)</b></code>


'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|arg0:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|controlTable:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|arg2:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|arg3:
|valign="top"| ''No description available.''
|}


=Source code samples=
{{PseudoH4|SelectGameSpeed.lua}}
:<code>UI/FrontEnd/GameSetup/SelectGameSpeed.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0067}}<syntaxhighlight lang="lua">ContextPtr:BuildInstanceForControlAtIndex( "ItemInstance", controlTable, Controls.Stack, i-1 );</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|BuildInstanceForControlAtIndex]]
[[Category:Civ5 Improvements API|BuildInstanceForControlAtIndex]]