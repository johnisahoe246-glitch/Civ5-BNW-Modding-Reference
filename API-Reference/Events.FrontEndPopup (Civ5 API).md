{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Events}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''void''' Events.FrontEndPopup<b>(</b>'''string''' string<b>)</b></code>


'''Event Type'''
:Regular event: you can subscribe to it through <code>Events.FrontEndPopup.Add(''<function handler>'')</code> or invoke it directly through <code>Events.FrontEndPopup(''<arguments list>'')</code>.

'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|string:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|FrontEndPopup.lua}}
:<code>UI/FrontEnd/FrontEndPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0009}}<syntaxhighlight lang="lua">Events.FrontEndPopup.Add( OnFrontEndPopup )</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0014}}<syntaxhighlight lang="lua">function OnBack()</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|JoiningRoom.lua}}
:<code>UI/FrontEnd/Multiplayer/JoiningRoom.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0057}}<syntaxhighlight lang="lua">Events.FrontEndPopup.CallImmediate( szText );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0059}}<syntaxhighlight lang="lua">Events.FrontEndPopup.CallImmediate( "TXT_KEY_MP_ROOM_FULL" );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0061}}<syntaxhighlight lang="lua">Events.FrontEndPopup.CallImmediate( "TXT_KEY_MP_JOIN_FAILED" );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0086}}<syntaxhighlight lang="lua">Events.FrontEndPopup.CallImmediate( "TXT_KEY_MP_KICKED" );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|StagingRoom.lua}}
:<code>UI/FrontEnd/Multiplayer/StagingRoom.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1327}}<syntaxhighlight lang="lua">Events.FrontEndPopup.CallImmediate( Locale.ConvertTextKey( "TXT_KEY_MP_VERSION_MISMATCH_FOR_HOST", playerName ) );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1330}}<syntaxhighlight lang="lua">Events.FrontEndPopup.CallImmediate( Locale.ConvertTextKey( "TXT_KEY_MP_VERSION_MISMATCH_FOR_PLAYER" ) );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1375}}<syntaxhighlight lang="lua">Events.FrontEndPopup.CallImmediate( "TXT_KEY_MP_NETWORK_CONNECTION_LOST" );</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|FrontEndPopup]]