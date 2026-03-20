{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Network}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''int''' Network.HasSentNetTurnComplete<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|ActionInfoPanel.lua}}
:<code>UI/InGame/WorldView/ActionInfoPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0084}}<syntaxhighlight lang="lua">if Network.HasSentNetTurnComplete() and PreGame.IsMultiplayerGame() then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0154}}<syntaxhighlight lang="lua">if not player:IsTurnActive() or (PreGame.IsMultiplayerGame() and Network.HasSentNetTurnComplete()) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0272}}<syntaxhighlight lang="lua">if not player:IsTurnActive() or (PreGame.IsMultiplayerGame() and Network.HasSentNetTurnComplete()) or Game.IsProcessingMessages() then</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|HasSentNetTurnComplete]]