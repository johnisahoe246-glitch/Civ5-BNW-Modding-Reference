{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|UIManager}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''int''' UIManager.IsModal<b>(</b>{{Type5|Context}} ContextPtr<b>)</b></code>


'''Returned Value'''
:No description available.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|ContextPtr:
|valign="top"| ''No description available.''
|}


=Source code samples=
{{PseudoH4|SaveMenu.lua}}
:<code>UI/InGame/Menus/SaveMenu.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0140}}<syntaxhighlight lang="lua">if (UIManager:IsModal( ContextPtr )) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0620}}<syntaxhighlight lang="lua">UIManager:IsModal( ContextPtr ) ) then</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|IsModal]]