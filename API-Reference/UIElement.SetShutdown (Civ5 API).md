{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This method is declared by {{Type5|Context}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''void''' UIElement:SetShutdown<b>(</b>('''void''' func<b>(</b><b>)</b>) OnShutdown<b>)</b></code>


'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|OnShutdown:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|UnitFlagManager.lua}}
:<code>UI/InGame/UnitFlagManager.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1553}}<syntaxhighlight lang="lua">ContextPtr:SetShutdown( OnShutdown );</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|SetShutdown]]