{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Player}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''bool''' Player:IsPlayerIgnoredBorderPromise<b>(</b>{{Type5|PlayerID}} activePlayer<b>)</b></code>


'''Returned Value'''
:No description available.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|activePlayer:
|valign="top"| ''No description available.''
|}


=Source code samples=
{{PseudoH4|InfoTooltipInclude.lua}}
:<code>UI/InGame/InfoTooltipInclude.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0849}}<syntaxhighlight lang="lua">if (pOtherPlayer:IsPlayerIgnoredBorderPromise(iActivePlayer)) then</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|IsPlayerIgnoredBorderPromise]]
[[Category:Civ5 Players API|IsPlayerIgnoredBorderPromise]]
[[Category:Civ5 Diplomacy API|IsPlayerIgnoredBorderPromise]]