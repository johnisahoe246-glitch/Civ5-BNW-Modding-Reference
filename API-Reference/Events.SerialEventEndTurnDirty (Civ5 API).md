{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Events}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''void''' Events.SerialEventEndTurnDirty<b>(</b><b>)</b></code>


'''Event Type'''
:Regular event: you can subscribe to it through <code>Events.SerialEventEndTurnDirty.Add(''<function handler>'')</code> or invoke it directly through <code>Events.SerialEventEndTurnDirty(''<arguments list>'')</code>.



=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|ActionInfoPanel.lua}}
:<code>UI/InGame/WorldView/ActionInfoPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0407}}<syntaxhighlight lang="lua">Events.SerialEventEndTurnDirty.Add( OnEndTurnDirty );</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|SerialEventEndTurnDirty]]
[[Category:Civ5 Game Settings API|SerialEventEndTurnDirty]]
[[Category:Civ5 Turns API|SerialEventEndTurnDirty]]
[[Category:Civ5 Victory API|SerialEventEndTurnDirty]]