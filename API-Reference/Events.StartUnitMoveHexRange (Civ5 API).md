{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Events}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''void''' Events.StartUnitMoveHexRange<b>(</b><b>)</b></code>


'''Event Type'''
:Regular event: you can subscribe to it through <code>Events.StartUnitMoveHexRange.Add(''<function handler>'')</code> or invoke it directly through <code>Events.StartUnitMoveHexRange(''<arguments list>'')</code>.



=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|WorldView.lua}}
:<code>UI/InGame/WorldView/WorldView.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0761}}<syntaxhighlight lang="lua">Events.StartUnitMoveHexRange.Add( OnStartUnitMoveHexRange );</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|StartUnitMoveHexRange]]
[[Category:Civ5 Units API|StartUnitMoveHexRange]]
[[Category:Civ5 Movement API|StartUnitMoveHexRange]]
[[Category:Civ5 Combat API|StartUnitMoveHexRange]]