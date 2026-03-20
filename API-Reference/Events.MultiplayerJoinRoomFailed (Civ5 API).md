{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Events}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''void''' Events.MultiplayerJoinRoomFailed<b>(</b>{{Type5|NetError}} extendedError, '''unknown''' aExtendedErrorText<b>)</b></code>


'''Event Type'''
:Regular event: you can subscribe to it through <code>Events.MultiplayerJoinRoomFailed.Add(''<function handler>'')</code> or invoke it directly through <code>Events.MultiplayerJoinRoomFailed(''<arguments list>'')</code>.

'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|extendedError:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|aExtendedErrorText:
|valign="top"| ''No description available.''
|}


=Source code samples=
{{PseudoH4|JoiningRoom.lua}}
:<code>UI/FrontEnd/Multiplayer/JoiningRoom.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0141}}<syntaxhighlight lang="lua">Events.MultiplayerJoinRoomFailed.Add( OnJoinRoomFailed );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0152}}<syntaxhighlight lang="lua">Events.MultiplayerJoinRoomFailed.Remove( OnJoinRoomFailed );</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|MultiplayerJoinRoomFailed]]