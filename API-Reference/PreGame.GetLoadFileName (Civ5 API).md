{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|PreGame}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''string''' PreGame.GetLoadFileName<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
{{PseudoH4|MPGameOptions.lua}}
:<code>UI/FrontEnd/Multiplayer/GameSetup/MPGameOptions.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0038}}<syntaxhighlight lang="lua">return (Matchmaking.IsHost() and PreGame.GetLoadFileName() == "") or PreGame.IsHotSeatGame() or Matchmaking.GetLocalID() == -1;</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0045}}<syntaxhighlight lang="lua">return (PreGame.GetLoadFileName() == "" and Matchmaking.GetLocalID() == -1) or PreGame.IsHotSeatGame();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|MPGameSetupScreen.lua}}
:<code>UI/FrontEnd/Multiplayer/GameSetup/MPGameSetupScreen.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0123}}<syntaxhighlight lang="lua">if PreGame.GetLoadFileName() == "" then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|StagingRoom.lua}}
:<code>UI/FrontEnd/Multiplayer/StagingRoom.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0391}}<syntaxhighlight lang="lua">(PreGame.GetLoadFileName() ~= "" and PreGame.GetSlotStatus( playerID ) == SlotStatus.SS_CLOSED); -- prevent closed player slots from blocking game startup when loading save games -tsmith</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0541}}<syntaxhighlight lang="lua">if(PreGame.GetLoadFileName() ~= "" or bIsHotSeat) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0595}}<syntaxhighlight lang="lua">if PreGame.GetLoadFileName() ~= "" then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0891}}<syntaxhighlight lang="lua">if( PreGame.GetLoadFileName() ~= "" ) then</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetLoadFileName]]
[[Category:Civ5 Movement API|GetLoadFileName]]