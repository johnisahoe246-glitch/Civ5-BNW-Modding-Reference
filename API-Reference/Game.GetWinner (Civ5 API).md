{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Game}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>{{Type5|TeamID}} Game.GetWinner<b>(</b><b>)</b></code>

'''Returned Value'''
:No description available.

=Source code samples=
{{PseudoH4|Ranking.lua}}
:<code>UI/InGame/Popups/Ranking.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0019}}<syntaxhighlight lang="lua">if (pPlayer:GetTeam() == Game:GetWinner()) then</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetWinner]]
[[Category:Civ5 Victory API|GetWinner]]