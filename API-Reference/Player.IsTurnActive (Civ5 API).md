{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Player}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''int''' Player:IsTurnActive<b>(</b>'''unknown''' void<b>)</b></code>


'''Returned Value'''
:No description available.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|void:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|ActionInfoPanel.lua}}
:<code>UI/InGame/WorldView/ActionInfoPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0075}}<syntaxhighlight lang="lua">if not player:IsTurnActive() then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0154}}<syntaxhighlight lang="lua">if not player:IsTurnActive() or (PreGame.IsMultiplayerGame() and Network.HasSentNetTurnComplete()) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0242}}<syntaxhighlight lang="lua">if(otherPlayer:IsHuman() and otherPlayer:IsTurnActive()) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0272}}<syntaxhighlight lang="lua">if not player:IsTurnActive() or (PreGame.IsMultiplayerGame() and Network.HasSentNetTurnComplete()) or Game.IsProcessingMessages() then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0416}}<syntaxhighlight lang="lua">if pPlayer:IsTurnActive() then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|NewTurn.lua}}
:<code>UI/InGame/NewTurn.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0035}}<syntaxhighlight lang="lua">if (not player:IsTurnActive()) then</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|IsTurnActive]]