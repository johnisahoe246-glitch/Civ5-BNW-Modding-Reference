{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|PreGame}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>{{Type5|SlotClaim}} PreGame.GetSlotClaim<b>(</b>{{Type5|PlayerID}} player<b>)</b></code>


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

{{PseudoH4|StagingRoom.lua}}
:<code>UI/FrontEnd/Multiplayer/StagingRoom.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0374}}<syntaxhighlight lang="lua">local bIsLocked = (PreGame.GetSlotClaim( playerID ) == SlotClaim.SLOTCLAIM_RESERVED ) or</syntaxhighlight>
{{CodeLine5|0375}}<syntaxhighlight lang="lua">(PreGame.GetSlotClaim( playerID ) == SlotClaim.SLOTCLAIM_ASSIGNED );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0673}}<syntaxhighlight lang="lua">if( PreGame.GetSlotClaim( i ) == SlotClaim.SLOTCLAIM_ASSIGNED ) then</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetSlotClaim]]
[[Category:Civ5 Game Settings API|GetSlotClaim]]