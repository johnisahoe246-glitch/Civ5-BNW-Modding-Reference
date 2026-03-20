{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Matchmaking}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''unknown''', '''unknown''' Matchmaking.HostHotSeatGame<b>(</b>'''string''' gameName, '''int''' arg1<b>)</b></code>


'''Returned Values'''
:No description available.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|gameName:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|arg1:
|valign="top"| ''No description available.''
|}


=Source code samples=
{{PseudoH4|LoadMenu.lua}}
:<code>UI/FrontEnd/LoadMenu.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0069}}<syntaxhighlight lang="lua">local bResult, bPending = Matchmaking.HostHotSeatGame( strGameName, PreGame.ReadActiveSlotCountFromSaveGame() );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|MPGameSetupScreen.lua}}
:<code>UI/FrontEnd/Multiplayer/GameSetup/MPGameSetupScreen.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0052}}<syntaxhighlight lang="lua">local bResult, bPending = Matchmaking.HostHotSeatGame( strGameName, worldInfo.DefaultPlayers );</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|HostHotSeatGame]]