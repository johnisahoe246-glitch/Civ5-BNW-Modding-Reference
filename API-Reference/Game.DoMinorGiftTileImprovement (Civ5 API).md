{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Game}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''void''' Game.DoMinorGiftTileImprovement<b>(</b>{{Type5|PlayerID}} fromPlayer, {{Type5|TaskType}} toPlayer, '''int''' plotX, '''int''' plotY<b>)</b></code>


'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|fromPlayer:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|toPlayer:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|plotX:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|plotY:
|valign="top"| ''No description available.''
|}


=Source code samples=
{{PseudoH4|InGame.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/InGame.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0274}}<syntaxhighlight lang="lua">Game.DoMinorGiftTileImprovement(iFromPlayer, iToPlayer, iPlotX, iPlotY);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|DoMinorGiftTileImprovement]]
[[Category:Civ5 Improvements API|DoMinorGiftTileImprovement]]
[[Category:Civ5 Diplomacy API|DoMinorGiftTileImprovement]]
[[Category:Civ5 City States API|DoMinorGiftTileImprovement]]