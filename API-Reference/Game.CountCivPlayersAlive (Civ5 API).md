{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Game}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''int''' Game.CountCivPlayersAlive<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|WorldBuilderRandomItems.lua}}
:<code>Gameplay/Lua/WorldBuilderRandomItems.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0041}}<syntaxhighlight lang="lua">local players = math.floor((Game.CountCivPlayersAlive() * resource.Player) / 100);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|CountCivPlayersAlive]]
[[Category:Civ5 Players API|CountCivPlayersAlive]]