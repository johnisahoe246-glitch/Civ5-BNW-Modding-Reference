{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Game}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''void''' Game.SetPausePlayer<b>(</b>{{Type5|PlayerID}} arg0<b>)</b></code>


'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|arg0:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|LoadScreen.lua}}
:<code>UI/FrontEnd/LoadScreen.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0093}}<syntaxhighlight lang="lua">Game.SetPausePlayer(-1);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0131}}<syntaxhighlight lang="lua">Game.SetPausePlayer(Game.GetActivePlayer());</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|PlayerChange.lua}}
:<code>UI/InGame/PlayerChange.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0130}}<syntaxhighlight lang="lua">Game.SetPausePlayer( Game.GetActivePlayer() );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0135}}<syntaxhighlight lang="lua">Game.SetPausePlayer( -1 );</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|SetPausePlayer]]
[[Category:Civ5 Players API|SetPausePlayer]]