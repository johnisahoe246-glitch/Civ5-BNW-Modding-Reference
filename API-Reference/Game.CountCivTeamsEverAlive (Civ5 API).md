{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Game}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''int''' Game.CountCivTeamsEverAlive<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
{{PseudoH4|MapmakerUtilities.lua}}
:<code>Gameplay/Lua/MapmakerUtilities.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0059}}<syntaxhighlight lang="lua">local iNumTeams = Game.CountCivTeamsEverAlive()</syntaxhighlight>
{{CodeLine5|0060}}<syntaxhighlight lang="lua">local iNumTeamsOfCivs = iNumTeams - iNumCityStates;</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|CountCivTeamsEverAlive]]
[[Category:Civ5 Players API|CountCivTeamsEverAlive]]