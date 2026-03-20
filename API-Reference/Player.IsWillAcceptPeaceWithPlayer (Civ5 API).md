{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Player}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''bool''' Player:IsWillAcceptPeaceWithPlayer<b>(</b>{{Type5|PlayerID}} player<b>)</b></code>


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

{{PseudoH4|TradeLogic.lua}}
:<code>UI/InGame/WorldView/TradeLogic.lua</code>
:{{CodeBegin5}}
{{CodeLine5|2595}}<syntaxhighlight lang="lua">if (not Players[iFromPlayer]:IsWillAcceptPeaceWithPlayer(iLoopPlayer)) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|2598}}<syntaxhighlight lang="lua">elseif (not pLoopPlayer:IsWillAcceptPeaceWithPlayer(iFromPlayer)) then</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|IsWillAcceptPeaceWithPlayer]]
[[Category:Civ5 Players API|IsWillAcceptPeaceWithPlayer]]
[[Category:Civ5 Diplomacy API|IsWillAcceptPeaceWithPlayer]]