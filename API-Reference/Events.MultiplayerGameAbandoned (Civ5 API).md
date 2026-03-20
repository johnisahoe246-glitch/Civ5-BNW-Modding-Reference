{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Events}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''void''' Events.MultiplayerGameAbandoned<b>(</b>{{Type5|NetKicked}} reason<b>)</b></code>


'''Event Type'''
:Regular event: you can subscribe to it through <code>Events.MultiplayerGameAbandoned.Add(''<function handler>'')</code> or invoke it directly through <code>Events.MultiplayerGameAbandoned(''<arguments list>'')</code>.

'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|reason:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|JoiningRoom.lua}}
:<code>UI/FrontEnd/Multiplayer/JoiningRoom.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0143}}<syntaxhighlight lang="lua">Events.MultiplayerGameAbandoned.Add( OnMultiplayerGameAbandoned );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0154}}<syntaxhighlight lang="lua">Events.MultiplayerGameAbandoned.Remove( OnMultiplayerGameAbandoned );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|StagingRoom.lua}}
:<code>UI/FrontEnd/Multiplayer/StagingRoom.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1379}}<syntaxhighlight lang="lua">Events.MultiplayerGameAbandoned.Add( OnAbandoned );</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|MultiplayerGameAbandoned]]