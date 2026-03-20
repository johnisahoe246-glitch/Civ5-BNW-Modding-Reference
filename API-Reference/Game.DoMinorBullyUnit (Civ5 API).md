{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Game}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''void''' Game.DoMinorBullyUnit<b>(</b>{{Type5|PlayerID}} activePlayer, {{Type5|PlayerID}} minorCiv<b>)</b></code>


'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|activePlayer:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|minorCiv:
|valign="top"| ''No description available.''
|}


=Source code samples=
{{PseudoH4|CityStateDiploPopup.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/Popups/CityStateDiploPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1101}}<syntaxhighlight lang="lua">Game.DoMinorBullyUnit(iActivePlayer, g_iMinorCivID);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|DoMinorBullyUnit]]
[[Category:Civ5 Units API|DoMinorBullyUnit]]
[[Category:Civ5 Diplomacy API|DoMinorBullyUnit]]
[[Category:Civ5 City States API|DoMinorBullyUnit]]