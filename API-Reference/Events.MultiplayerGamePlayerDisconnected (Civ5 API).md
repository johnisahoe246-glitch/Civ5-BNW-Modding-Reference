{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Events}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''void''' Events.MultiplayerGamePlayerDisconnected<b>(</b>{{Type5|PlayerID}} player<b>)</b></code>


'''Event Type'''
:Regular event: you can subscribe to it through <code>Events.MultiplayerGamePlayerDisconnected.Add(''<function handler>'')</code> or invoke it directly through <code>Events.MultiplayerGamePlayerDisconnected(''<arguments list>'')</code>.

'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|player:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|DiploCorner.lua}}
:<code>UI/InGame/WorldView/DiploCorner.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0220}}<syntaxhighlight lang="lua">Events.MultiplayerGamePlayerDisconnected.Add( OnPlayerDisconnect );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|MPList.lua}}
:<code>UI/InGame/WorldView/MPList.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0303}}<syntaxhighlight lang="lua">Events.MultiplayerGamePlayerDisconnected.Add( UpdateAndSort )</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0308}}<syntaxhighlight lang="lua">function OnUpdate()</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|StagingRoom.lua}}
:<code>UI/FrontEnd/Multiplayer/StagingRoom.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0652}}<syntaxhighlight lang="lua">Events.MultiplayerGamePlayerDisconnected.Add( OnDisconnect );</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|MultiplayerGamePlayerDisconnected]]
[[Category:Civ5 Players API|MultiplayerGamePlayerDisconnected]]