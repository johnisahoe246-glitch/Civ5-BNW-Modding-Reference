{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Game}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''int''' Game.CountHumanPlayersAlive<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
{{PseudoH4|EndGameMenu.lua}}
:<code>UI/InGame/Popups/EndGameMenu.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0012}}<syntaxhighlight lang="lua">if (Game.IsHotSeat() and Game.CountHumanPlayersAlive() > 0) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0291}}<syntaxhighlight lang="lua">if (Game.IsHotSeat() and Game.CountHumanPlayersAlive() > 0 and not pPlayer:IsAlive()) then</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|CountHumanPlayersAlive]]
[[Category:Civ5 Players API|CountHumanPlayersAlive]]