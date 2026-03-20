{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|PreGame}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>{{Type5|SlotStatus}} PreGame.GetSlotStatus<b>(</b>{{Type5|PlayerID}} player<b>)</b></code>


'''Returned Value'''
:No description available.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|player:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|AdvancedSetup.lua}}
:<code>UI/FrontEnd/GameSetup/AdvancedSetup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0272}}<syntaxhighlight lang="lua">if( PreGame.GetSlotStatus( i ) ~= SlotStatus.SS_COMPUTER ) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0284}}<syntaxhighlight lang="lua">if( PreGame.GetSlotStatus(i) == SlotStatus.SS_COMPUTER) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0982}}<syntaxhighlight lang="lua">if( PreGame.GetSlotStatus( i ) == SlotStatus.SS_COMPUTER ) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1036}}<syntaxhighlight lang="lua">if( PreGame.GetSlotStatus(i) == SlotStatus.SS_COMPUTER ) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1156}}<syntaxhighlight lang="lua">if( PreGame.GetSlotStatus(i) ~= SlotStatus.SS_COMPUTER) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|NetworkDebug.lua}}
:<code>UI/InGame/NetworkDebug.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0011}}<syntaxhighlight lang="lua">if (PreGame.GetSlotStatus( i-1 ) == SlotStatus.SS_TAKEN) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|StagingRoom.lua}}
:<code>UI/FrontEnd/Multiplayer/StagingRoom.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0226}}<syntaxhighlight lang="lua">if( PreGame.GetSlotStatus( i ) == SlotStatus.SS_COMPUTER or PreGame.GetSlotStatus( i ) == SlotStatus.SS_TAKEN ) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0372}}<syntaxhighlight lang="lua">local bIsHuman  = (PreGame.GetSlotStatus( playerID ) == SlotStatus.SS_TAKEN ) or</syntaxhighlight>
{{CodeLine5|0373}}<syntaxhighlight lang="lua">(PreGame.GetSlotStatus( playerID ) == SlotStatus.SS_OPEN );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0377}}<syntaxhighlight lang="lua">local bIsDisabled = (PreGame.GetSlotStatus( playerID ) == SlotStatus.SS_CLOSED );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0391}}<syntaxhighlight lang="lua">(PreGame.GetLoadFileName() ~= "" and PreGame.GetSlotStatus( playerID ) == SlotStatus.SS_CLOSED); -- prevent closed player slots from blocking game startup when loading save games -tsmith</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetSlotStatus]]
[[Category:Civ5 Game Settings API|GetSlotStatus]]