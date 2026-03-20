{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Deal}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''void''' Deal:ChangeGoldTrade<b>(</b>{{Type5|PlayerID}} us, '''int''' gold<b>)</b></code>


'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|us:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|gold:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|TradeLogic.lua}}
:<code>UI/InGame/WorldView/TradeLogic.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1932}}<syntaxhighlight lang="lua">g_Deal:ChangeGoldTrade( g_iUs, iGold );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1947}}<syntaxhighlight lang="lua">g_Deal:ChangeGoldTrade( g_iThem, iGold );</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|ChangeGoldTrade]]
[[Category:Civ5 Gold API|ChangeGoldTrade]]
[[Category:Civ5 Trade API|ChangeGoldTrade]]