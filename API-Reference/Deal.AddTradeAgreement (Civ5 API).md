{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Deal}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''void''' Deal:AddTradeAgreement<b>(</b>{{Type5|PlayerID}} us, {{Type5|ResourceType}} dealDuration<b>)</b></code>


'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|us:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|dealDuration:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|TradeLogic.lua}}
:<code>UI/InGame/WorldView/TradeLogic.lua</code>
:{{CodeBegin5}}
{{CodeLine5|2185}}<syntaxhighlight lang="lua">g_Deal:AddTradeAgreement( g_iUs, g_iDealDuration );</syntaxhighlight>
{{CodeLine5|2186}}<syntaxhighlight lang="lua">g_Deal:AddTradeAgreement( g_iThem, g_iDealDuration );</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|AddTradeAgreement]]
[[Category:Civ5 Trade API|AddTradeAgreement]]