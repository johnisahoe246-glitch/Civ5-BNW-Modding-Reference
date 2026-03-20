{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Player}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''bool''' Player:IsPlayerDenouncedEnemy<b>(</b>{{Type5|PlayerID}} otherPlayer<b>)</b></code>


'''Returned Value'''
:No description available.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|otherPlayer:
|valign="top"| ''No description available.''
|}


=Source code samples=
{{PseudoH4|InfoTooltipInclude.lua}}
:<code>UI/InGame/InfoTooltipInclude.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0785}}<syntaxhighlight lang="lua">if (pActivePlayer:IsPlayerDenouncedEnemy(iOtherPlayer)) then      -- Human has denounced an enemy of the AI</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|IsPlayerDenouncedEnemy]]
[[Category:Civ5 Players API|IsPlayerDenouncedEnemy]]
[[Category:Civ5 Diplomacy API|IsPlayerDenouncedEnemy]]