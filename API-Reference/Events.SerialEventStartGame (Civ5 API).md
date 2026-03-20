{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Events}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''void''' Events.SerialEventStartGame<b>(</b>'''int''' arg0 = nil<b>)</b></code>


'''Event Type'''
:Regular event: you can subscribe to it through <code>Events.SerialEventStartGame.Add(''<function handler>'')</code> or invoke it directly through <code>Events.SerialEventStartGame(''<arguments list>'')</code>.

'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|arg0:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|AdvancedSetup.lua}}
:<code>UI/FrontEnd/GameSetup/AdvancedSetup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1180}}<syntaxhighlight lang="lua">Events.SerialEventStartGame();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|WorldPicker.lua}}
:<code>UI/FrontEnd/WorldPicker.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0009}}<syntaxhighlight lang="lua">Events.SerialEventStartGame( WorldSizeTypes.WORLDSIZE_DUEL );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0019}}<syntaxhighlight lang="lua">Events.SerialEventStartGame( WorldSizeTypes.WORLDSIZE_TINY );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0029}}<syntaxhighlight lang="lua">Events.SerialEventStartGame( WorldSizeTypes.WORLDSIZE_SMALL );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0039}}<syntaxhighlight lang="lua">Events.SerialEventStartGame( WorldSizeTypes.WORLDSIZE_STANDARD );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0049}}<syntaxhighlight lang="lua">Events.SerialEventStartGame( WorldSizeTypes.WORLDSIZE_LARGE );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0059}}<syntaxhighlight lang="lua">Events.SerialEventStartGame( WorldSizeTypes.WORLDSIZE_HUGE );</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|SerialEventStartGame]]