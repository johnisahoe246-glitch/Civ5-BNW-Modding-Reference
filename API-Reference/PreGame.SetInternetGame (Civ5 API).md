{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|PreGame}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''void''' PreGame.SetInternetGame<b>(</b>'''int''' isInternet<b>)</b></code>


'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|isInternet:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|MultiplayerSelect.lua}}
:<code>UI/FrontEnd/Multiplayer/MultiplayerSelect.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0011}}<syntaxhighlight lang="lua">PreGame.SetInternetGame( true );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0026}}<syntaxhighlight lang="lua">PreGame.SetInternetGame( false );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|StagingRoom.lua}}
:<code>UI/FrontEnd/Multiplayer/StagingRoom.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0604}}<syntaxhighlight lang="lua">PreGame.SetInternetGame( bIsInternet );</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|SetInternetGame]]