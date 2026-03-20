{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Game}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''void''' Game.DoMinorPledgeProtection<b>(</b>{{Type5|PlayerID}} activePlayer, {{Type5|PlayerID}} minorCiv, '''bool''' arg2<b>)</b></code>


'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|activePlayer:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|minorCiv:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|arg2:
|valign="top"| ''No description available.''
|}


=Source code samples=
{{PseudoH4|CityStateDiploPopup.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/Popups/CityStateDiploPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0637}}<syntaxhighlight lang="lua">Game.DoMinorPledgeProtection(Game.GetActivePlayer(), g_iMinorCivID, true);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0652}}<syntaxhighlight lang="lua">Game.DoMinorPledgeProtection(iActivePlayer, g_iMinorCivID, false);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|DoMinorPledgeProtection]]
[[Category:Civ5 City States API|DoMinorPledgeProtection]]