{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Deal}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''void''' Deal:ChangeGoldPerTurnTrade<b>(</b>{{Type5|PlayerID}} us, '''int''' goldPerTurn, {{Type5|ResourceType}} dealDuration<b>)</b></code>


'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|us:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|goldPerTurn:
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
{{CodeLine5|2037}}<syntaxhighlight lang="lua">g_Deal:ChangeGoldPerTurnTrade( g_iUs, iGoldPerTurn, g_iDealDuration );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|2050}}<syntaxhighlight lang="lua">g_Deal:ChangeGoldPerTurnTrade( g_iThem, iGoldPerTurn, g_iDealDuration );</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|ChangeGoldPerTurnTrade]]
[[Category:Civ5 Gold API|ChangeGoldPerTurnTrade]]
[[Category:Civ5 Trade API|ChangeGoldPerTurnTrade]]