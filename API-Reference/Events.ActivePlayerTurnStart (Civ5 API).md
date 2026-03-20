{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Events}}.<br/>
This is a static method, invoke it with a dot.
}}


Fires on the turn start of the active player. The active player is the player playing on the local machine. In other words, this fires whenever your turn starts. Compare to {{Func5|Events|ActivePlayerTurnEnd}}
Note:'' This event does not fire when using Autoplay.


=Usage=
<code>'''void''' Events.ActivePlayerTurnStart<b>(</b><b>)</b></code>


'''Event Type'''
:Regular event: you can subscribe to it through <code>Events.ActivePlayerTurnStart.Add(''<function handler>'')</code> or invoke it directly through <code>Events.ActivePlayerTurnStart(''<arguments list>'')</code>.



=Examples=
<syntaxhighlight lang="lua" class="civ5-example">
function listener()
print("I'm listening!")
end
Events.ActivePlayerTurnStart.Add(listener)</syntaxhighlight>


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|DiploCorner.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/WorldView/DiploCorner.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0505}}<syntaxhighlight lang="lua">Events.ActivePlayerTurnStart.Add(OnActivePlayerTurnStart);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|InGame.lua}}
:<code>UI/InGame/InGame.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0733}}<syntaxhighlight lang="lua">Events.ActivePlayerTurnStart.Add( OnActivePlayerTurnStart );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|MPList.lua}}
:<code>UI/InGame/WorldView/MPList.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0337}}<syntaxhighlight lang="lua">Events.ActivePlayerTurnStart.Add( OnLocalTurnStart );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|NewTurn.lua}}
:<code>UI/InGame/NewTurn.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0062}}<syntaxhighlight lang="lua">Events.ActivePlayerTurnStart.Add( OnTurnStart );</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|ActivePlayerTurnStart]]
[[Category:Civ5 Players API|ActivePlayerTurnStart]]