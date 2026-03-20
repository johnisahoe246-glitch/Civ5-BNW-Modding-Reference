{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|LuaEvents}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''void''' LuaEvents.ChatShow<b>(</b>'''int''' chatOpen<b>)</b></code>


'''Event Type'''
:Regular event: you can subscribe to it through <code>LuaEvents.ChatShow.Add(''<function handler>'')</code> or invoke it directly through <code>LuaEvents.ChatShow(''<arguments list>'')</code>.

'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|chatOpen:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|DiploCorner.lua}}
:<code>UI/InGame/WorldView/DiploCorner.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0125}}<syntaxhighlight lang="lua">LuaEvents.ChatShow( m_bChatOpen );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|MPList.lua}}
:<code>UI/InGame/WorldView/MPList.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0352}}<syntaxhighlight lang="lua">LuaEvents.ChatShow.Add( OnChatToggle );</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|ChatShow]]