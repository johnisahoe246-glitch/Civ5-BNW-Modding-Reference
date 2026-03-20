{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Events}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''void''' Events.ConnectedToNetworkHost<b>(</b>{{Type5|PlayerID}} player<b>)</b></code>


'''Event Type'''
:Regular event: you can subscribe to it through <code>Events.ConnectedToNetworkHost.Add(''<function handler>'')</code> or invoke it directly through <code>Events.ConnectedToNetworkHost(''<arguments list>'')</code>.

'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|player:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|JoiningRoom.lua}}
:<code>UI/FrontEnd/Multiplayer/JoiningRoom.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0144}}<syntaxhighlight lang="lua">Events.ConnectedToNetworkHost.Add( OnConnect );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0155}}<syntaxhighlight lang="lua">Events.ConnectedToNetworkHost.Remove( OnConnect );</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|ConnectedToNetworkHost]]