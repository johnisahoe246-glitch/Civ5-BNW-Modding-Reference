{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Game}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''void''' Game.SetActivePlayer<b>(</b>{{Type5|PlayerID}} newValue, '''bool''' forceHotSeat<b>)</b></code>


'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|newValue:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|forceHotSeat:
|valign="top"| ''No description available.''
|}


=Source code samples=
{{PseudoH4|EndGameMenu.lua}}
:<code>UI/InGame/Popups/EndGameMenu.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0028}}<syntaxhighlight lang="lua">Game.SetActivePlayer( iNextPlayer );</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|SetActivePlayer]]
[[Category:Civ5 Players API|SetActivePlayer]]