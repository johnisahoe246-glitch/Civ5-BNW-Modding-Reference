{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Events}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''void''' Events.MultiplayerGamePlayerUpdated<b>(</b><b>)</b></code>


'''Event Type'''
:Regular event: you can subscribe to it through <code>Events.MultiplayerGamePlayerUpdated.Add(''<function handler>'')</code> or invoke it directly through <code>Events.MultiplayerGamePlayerUpdated(''<arguments list>'')</code>.



=Source code samples=
{{PseudoH4|StagingRoom.lua}}
:<code>UI/FrontEnd/Multiplayer/StagingRoom.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0641}}<syntaxhighlight lang="lua">Events.MultiplayerGamePlayerUpdated.Add( OnDisconnectOrPossiblyUpdate );</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|MultiplayerGamePlayerUpdated]]
[[Category:Civ5 Players API|MultiplayerGamePlayerUpdated]]