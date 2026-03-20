{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|PreGame}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''void''' PreGame.SetReady<b>(</b>{{Type5|PlayerID}} arg0, '''bool''' checked = nil<b>)</b></code>


'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|arg0:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|checked:
|valign="top"| ''No description available.''
|}


=Source code samples=
{{PseudoH4|StagingRoom.lua}}
:<code>UI/FrontEnd/Multiplayer/StagingRoom.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0192}}<syntaxhighlight lang="lua">PreGame.SetReady( Matchmaking.GetLocalID(), bChecked );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0543}}<syntaxhighlight lang="lua">PreGame.SetReady(Matchmaking.GetLocalID(), true);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0856}}<syntaxhighlight lang="lua">PreGame.SetReady( Matchmaking.GetLocalID() );</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|SetReady]]