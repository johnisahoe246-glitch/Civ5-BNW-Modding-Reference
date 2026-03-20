{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Events}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''void''' Events.MultiplayerJoinRoomComplete<b>(</b><b>)</b></code>


'''Event Type'''
:Regular event: you can subscribe to it through <code>Events.MultiplayerJoinRoomComplete.Add(''<function handler>'')</code> or invoke it directly through <code>Events.MultiplayerJoinRoomComplete(''<arguments list>'')</code>.



=Source code samples=
{{PseudoH4|JoiningRoom.lua}}
:<code>UI/FrontEnd/Multiplayer/JoiningRoom.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0140}}<syntaxhighlight lang="lua">Events.MultiplayerJoinRoomComplete.Add( OnJoinRoomComplete );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0151}}<syntaxhighlight lang="lua">Events.MultiplayerJoinRoomComplete.Remove( OnJoinRoomComplete );</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|MultiplayerJoinRoomComplete]]