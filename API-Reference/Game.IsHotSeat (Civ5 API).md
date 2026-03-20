{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Game}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''int''' Game.IsHotSeat<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|DiploCorner.lua}}
:<code>UI/InGame/WorldView/DiploCorner.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0391}}<syntaxhighlight lang="lua">if ( not Game.IsHotSeat() ) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|EndGameMenu.lua}}
:<code>UI/InGame/Popups/EndGameMenu.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0012}}<syntaxhighlight lang="lua">if (Game.IsHotSeat() and Game.CountHumanPlayersAlive() > 0) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0291}}<syntaxhighlight lang="lua">if (Game.IsHotSeat() and Game.CountHumanPlayersAlive() > 0 and not pPlayer:IsAlive()) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TutorialEngine.lua}}
:<code>Tutorial/TutorialEngine.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0542}}<syntaxhighlight lang="lua">if (Game.IsGameMultiPlayer() or Game.IsHotSeat()) then</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|IsHotSeat]]