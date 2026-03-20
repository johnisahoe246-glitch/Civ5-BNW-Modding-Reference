{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Events}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''void''' Events.PlayerVersionMismatchEvent<b>(</b>{{Type5|PlayerID}} player, '''unknown''' playerName, '''bool''' isHost<b>)</b></code>


'''Event Type'''
:Regular event: you can subscribe to it through <code>Events.PlayerVersionMismatchEvent.Add(''<function handler>'')</code> or invoke it directly through <code>Events.PlayerVersionMismatchEvent(''<arguments list>'')</code>.

'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|player:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|playerName:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|isHost:
|valign="top"| ''No description available.''
|}


=Source code samples=
{{PseudoH4|StagingRoom.lua}}
:<code>UI/FrontEnd/Multiplayer/StagingRoom.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1334}}<syntaxhighlight lang="lua">Events.PlayerVersionMismatchEvent.Add( OnVersionMismatch );</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|PlayerVersionMismatchEvent]]
[[Category:Civ5 Players API|PlayerVersionMismatchEvent]]