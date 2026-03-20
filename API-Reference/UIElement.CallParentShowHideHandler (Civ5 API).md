{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This method is declared by {{Type5|Context}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''void''' UIElement:CallParentShowHideHandler<b>(</b>'''bool''' arg0<b>)</b></code>


'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|arg0:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|ModsError.lua}}
:<code>UI/FrontEnd/Modding/ModsError.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0012}}<syntaxhighlight lang="lua">ContextPtr:CallParentShowHideHandler( true );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TradeLogic.lua}}
:<code>UI/InGame/WorldView/TradeLogic.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0352}}<syntaxhighlight lang="lua">ContextPtr:CallParentShowHideHandler( false );</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|CallParentShowHideHandler]]