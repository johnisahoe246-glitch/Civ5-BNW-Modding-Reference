{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|PreGame}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''int''' PreGame.IsReady<b>(</b>{{Type5|PlayerID}} player<b>)</b></code>


'''Returned Value'''
:No description available.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|player:
|valign="top"| ''No description available.''
|}


=Source code samples=
{{PseudoH4|StagingRoom.lua}}
:<code>UI/FrontEnd/Multiplayer/StagingRoom.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0383}}<syntaxhighlight lang="lua">bIsReady = PreGame.IsReady( playerID );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0390}}<syntaxhighlight lang="lua">bIsReady =   (PreGame.IsReady( m_HostID )) or</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0540}}<syntaxhighlight lang="lua">local bIsReady = PreGame.IsReady( Matchmaking.GetLocalID() );</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|IsReady]]