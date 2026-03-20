{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Deal}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''void''' Deal:RemoveByType<b>(</b>{{Type5|TradeableItemType}} arg0, {{Type5|PlayerID}} us<b>)</b></code>


'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|arg0:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|us:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|TradeLogic.lua}}
:<code>UI/InGame/WorldView/TradeLogic.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1899}}<syntaxhighlight lang="lua">g_Deal:RemoveByType( TradeableItems.TRADE_ITEM_GOLD, g_iUs );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1901}}<syntaxhighlight lang="lua">g_Deal:RemoveByType( TradeableItems.TRADE_ITEM_GOLD, g_iThem );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|2000}}<syntaxhighlight lang="lua">g_Deal:RemoveByType( TradeableItems.TRADE_ITEM_GOLD_PER_TURN, g_iUs );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|2002}}<syntaxhighlight lang="lua">g_Deal:RemoveByType( TradeableItems.TRADE_ITEM_GOLD_PER_TURN, g_iThem );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|2086}}<syntaxhighlight lang="lua">g_Deal:RemoveByType( TradeableItems.TRADE_ITEM_OPEN_BORDERS, g_iUs );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|2089}}<syntaxhighlight lang="lua">g_Deal:RemoveByType( TradeableItems.TRADE_ITEM_OPEN_BORDERS, g_iThem );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|2129}}<syntaxhighlight lang="lua">g_Deal:RemoveByType( TradeableItems.TRADE_ITEM_DEFENSIVE_PACT, g_iUs );</syntaxhighlight>
{{CodeLine5|2130}}<syntaxhighlight lang="lua">g_Deal:RemoveByType( TradeableItems.TRADE_ITEM_DEFENSIVE_PACT, g_iThem );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|2165}}<syntaxhighlight lang="lua">g_Deal:RemoveByType( TradeableItems.TRADE_ITEM_RESEARCH_AGREEMENT, g_iUs );</syntaxhighlight>
{{CodeLine5|2166}}<syntaxhighlight lang="lua">g_Deal:RemoveByType( TradeableItems.TRADE_ITEM_RESEARCH_AGREEMENT, g_iThem );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|2201}}<syntaxhighlight lang="lua">g_Deal:RemoveByType( TradeableItems.TRADE_ITEM_TRADE_AGREEMENT, g_iUs );</syntaxhighlight>
{{CodeLine5|2202}}<syntaxhighlight lang="lua">g_Deal:RemoveByType( TradeableItems.TRADE_ITEM_TRADE_AGREEMENT, g_iThem );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TradeLogic.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/WorldView/TradeLogic.lua</code>
:{{CodeBegin5}}
{{CodeLine5|2273}}<syntaxhighlight lang="lua">g_Deal:RemoveByType( TradeableItems.TRADE_ITEM_ALLOW_EMBASSY, g_iUs );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|2276}}<syntaxhighlight lang="lua">g_Deal:RemoveByType( TradeableItems.TRADE_ITEM_ALLOW_EMBASSY, g_iThem );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|2305}}<syntaxhighlight lang="lua">g_Deal:RemoveByType( TradeableItems.TRADE_ITEM_DECLARATION_OF_FRIENDSHIP, g_iUs );</syntaxhighlight>
{{CodeLine5|2306}}<syntaxhighlight lang="lua">g_Deal:RemoveByType( TradeableItems.TRADE_ITEM_DECLARATION_OF_FRIENDSHIP, g_iThem );</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|RemoveByType]]