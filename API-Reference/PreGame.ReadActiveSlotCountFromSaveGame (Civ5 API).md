{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|PreGame}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''int''' PreGame.ReadActiveSlotCountFromSaveGame<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
{{PseudoH4|LoadMenu.lua}}
:<code>UI/FrontEnd/LoadMenu.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0066}}<syntaxhighlight lang="lua">local bResult, bPending = Matchmaking.HostInternetGame( strGameName, PreGame.ReadActiveSlotCountFromSaveGame() );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0069}}<syntaxhighlight lang="lua">local bResult, bPending = Matchmaking.HostHotSeatGame( strGameName, PreGame.ReadActiveSlotCountFromSaveGame() );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0071}}<syntaxhighlight lang="lua">local bResult, bPending = Matchmaking.HostLANGame( strGameName, PreGame.ReadActiveSlotCountFromSaveGame() );</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|ReadActiveSlotCountFromSaveGame]]
[[Category:Civ5 Game Settings API|ReadActiveSlotCountFromSaveGame]]