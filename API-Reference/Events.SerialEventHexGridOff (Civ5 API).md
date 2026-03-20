{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Events}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''void''' Events.SerialEventHexGridOff<b>(</b><b>)</b></code>


'''Event Type'''
:Regular event: you can subscribe to it through <code>Events.SerialEventHexGridOff.Add(''<function handler>'')</code> or invoke it directly through <code>Events.SerialEventHexGridOff(''<arguments list>'')</code>.



=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|InGame.lua}}
:<code>UI/InGame/InGame.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0370}}<syntaxhighlight lang="lua">Events.SerialEventHexGridOff();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|MiniMapPanel.lua}}
:<code>UI/InGame/WorldView/MiniMapPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0345}}<syntaxhighlight lang="lua">Events.SerialEventHexGridOff.Add( OnGridOff )</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0350}}<syntaxhighlight lang="lua">function OnYieldChecked( bIsChecked )</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|SerialEventHexGridOff]]