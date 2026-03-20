{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Events}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''void''' Events.GameMessageChat<b>(</b>{{Type5|PlayerID}} fromPlayer, {{Type5|PlayerID}} toPlayer, '''string''' text, {{Type5|ChatTargetType}} targetType<b>)</b></code>


'''Event Type'''
:Regular event: you can subscribe to it through <code>Events.GameMessageChat.Add(''<function handler>'')</code> or invoke it directly through <code>Events.GameMessageChat(''<arguments list>'')</code>.

'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|fromPlayer:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|toPlayer:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|text:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|targetType:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|DiploCorner.lua}}
:<code>UI/InGame/WorldView/DiploCorner.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0185}}<syntaxhighlight lang="lua">Events.GameMessageChat.Add( OnChat );</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GameMessageChat]]