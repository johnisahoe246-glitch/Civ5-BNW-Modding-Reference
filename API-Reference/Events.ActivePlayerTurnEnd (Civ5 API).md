{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Events}}.<br/>
This is a static method, invoke it with a dot.
}}


Fires on the turn end of the active player. The active player is the player playing on the local machine. In other words, this fires whenever your turn end. Compare to {{Func5|Events|ActivePlayerTurnStart}}
Note:'' This event does not fire when using Autoplay.


=Usage=
<code>'''void''' Events.ActivePlayerTurnEnd<b>(</b><b>)</b></code>


'''Event Type'''
:Regular event: you can subscribe to it through <code>Events.ActivePlayerTurnEnd.Add(''<function handler>'')</code> or invoke it directly through <code>Events.ActivePlayerTurnEnd(''<arguments list>'')</code>.



=Examples=
<syntaxhighlight lang="lua" class="civ5-example">
function listener()
print("I'm listening!")
end
Events.ActivePlayerTurnEnd.Add(listener)</syntaxhighlight>


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|ActionInfoPanel.lua}}
:<code>UI/InGame/WorldView/ActionInfoPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0265}}<syntaxhighlight lang="lua">Events.ActivePlayerTurnEnd.Add( OnActivePlayerTurnEnd );</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|ActivePlayerTurnEnd]]
[[Category:Civ5 Players API|ActivePlayerTurnEnd]]