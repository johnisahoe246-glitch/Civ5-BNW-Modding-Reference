{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Player}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''int''' Player:GetQuestTurnsRemaining<b>(</b>{{Type5|PlayerID}} major, {{Type5|MinorCivQuestType}} type, {{Type5|PlayerID}} arg2<b>)</b></code>


'''Returned Value'''
:No description available.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|major:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|type:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|arg2:
|valign="top"| ''No description available.''
|}


=Source code samples=
{{PseudoH4|CityStateStatusHelper.lua (G&K)}}
:<code>DLC/Expansion/UI/CityStateStatusHelper.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0477}}<syntaxhighlight lang="lua">local iTurnsRemaining = pMinor:GetQuestTurnsRemaining(iMajor, eType, Game.GetGameTurn() - 1); -- add 1 since began on CS's turn (1 before), and avoids "0 turns remaining"</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetQuestTurnsRemaining]]