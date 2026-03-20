{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Player}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''bool''' Player:IsPlayerDoFwithAnyFriend<b>(</b>{{Type5|PlayerID}} otherPlayer<b>)</b></code>


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
{{CodeLine5|0782}}<syntaxhighlight lang="lua">if (pActivePlayer:IsPlayerDoFwithAnyFriend(iOtherPlayer)) then      -- Human has a mutual friend with the AI</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|IsPlayerDoFwithAnyFriend]]
[[Category:Civ5 Players API|IsPlayerDoFwithAnyFriend]]
[[Category:Civ5 Diplomacy API|IsPlayerDoFwithAnyFriend]]