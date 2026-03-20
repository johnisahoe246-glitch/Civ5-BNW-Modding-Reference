{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Player}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''void''' Player:DoTradeScreenClosed<b>(</b>'''bool''' aIMakingOffer<b>)</b></code>


'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|aIMakingOffer:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|TradeLogic.lua}}
:<code>UI/InGame/WorldView/TradeLogic.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0380}}<syntaxhighlight lang="lua">Players[g_iThem]:DoTradeScreenClosed(g_bAIMakingOffer);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|DoTradeScreenClosed]]
[[Category:Civ5 Trade API|DoTradeScreenClosed]]