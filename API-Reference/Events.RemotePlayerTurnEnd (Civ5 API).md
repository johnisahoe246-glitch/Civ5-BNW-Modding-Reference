{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Events}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''void''' Events.RemotePlayerTurnEnd<b>(</b><b>)</b></code>


'''Event Type'''
:Regular event: you can subscribe to it through <code>Events.RemotePlayerTurnEnd.Add(''<function handler>'')</code> or invoke it directly through <code>Events.RemotePlayerTurnEnd(''<arguments list>'')</code>.



=Source code samples=
{{PseudoH4|MPList.lua}}
:<code>UI/InGame/WorldView/MPList.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0329}}<syntaxhighlight lang="lua">Events.RemotePlayerTurnEnd.Add( OnRemotePlayerTurnEnd );</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|RemotePlayerTurnEnd]]
[[Category:Civ5 Players API|RemotePlayerTurnEnd]]