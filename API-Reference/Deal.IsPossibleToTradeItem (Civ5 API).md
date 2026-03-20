{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Deal}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''int''' Deal:IsPossibleToTradeItem<b>(</b>{{Type5|PlayerID}} us, {{Type5|PlayerID}} them, {{Type5|TradeableItemType}} tradeType, {{Type5|TeamID}} dealDuration, {{Type5|ResourceType}} dealDuration = nil<b>)</b></code>


'''Returned Value'''
:No description available.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|us:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|them:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|tradeType:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|dealDuration:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|dealDuration:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|DiploRelationships.lua}}
:<code>UI/InGame/Popups/DiploRelationships.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0296}}<syntaxhighlight lang="lua">bOpenBordersAllowed = g_Deal:IsPossibleToTradeItem(iPlayer, g_iUs, TradeableItems.TRADE_ITEM_OPEN_BORDERS, g_iDealDuration);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0304}}<syntaxhighlight lang="lua">bDefensivePactAllowed = g_Deal:IsPossibleToTradeItem(iPlayer, g_iUs, TradeableItems.TRADE_ITEM_DEFENSIVE_PACT, g_iDealDuration);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0312}}<syntaxhighlight lang="lua">bResearchAgreementAllowed = g_Deal:IsPossibleToTradeItem(iPlayer, g_iUs, TradeableItems.TRADE_ITEM_RESEARCH_AGREEMENT, g_iDealDuration);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0320}}<syntaxhighlight lang="lua">bTradeAgreementAllowed = g_Deal:IsPossibleToTradeItem(iPlayer, g_iUs, TradeableItems.TRADE_ITEM_TRADE_AGREEMENT, g_iDealDuration);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0333}}<syntaxhighlight lang="lua">local bCanTradeResource = g_Deal:IsPossibleToTradeItem(iPlayer, g_iUs, TradeableItems.TRADE_ITEM_RESOURCES, i, 1);   -- 1 here is 1 quanity of the Resource, which is the minimum possible</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DiploRelationships.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/Popups/DiploRelationships.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0299}}<syntaxhighlight lang="lua">bEmbassyAllowed = g_Deal:IsPossibleToTradeItem(iPlayer, g_iUs, TradeableItems.TRADE_ITEM_ALLOW_EMBASSY, g_iDealDuration);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TradeLogic.lua}}
:<code>UI/InGame/WorldView/TradeLogic.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1004}}<syntaxhighlight lang="lua">local bGoldTradeAllowed = g_Deal:IsPossibleToTradeItem(g_iUs, g_iThem, TradeableItems.TRADE_ITEM_GOLD, 1);   -- 1 here is 1 Gold, which is the minimum possible</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1019}}<syntaxhighlight lang="lua">bGoldTradeAllowed = g_Deal:IsPossibleToTradeItem(g_iThem, g_iUs, TradeableItems.TRADE_ITEM_GOLD, 1);   -- 1 here is 1 Gold, which is the minimum possible</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1038}}<syntaxhighlight lang="lua">local bGPTAllowed = g_Deal:IsPossibleToTradeItem(g_iUs, g_iThem, TradeableItems.TRADE_ITEM_GOLD_PER_TURN, 1, g_iDealDuration);   -- 1 here is 1 GPT, which is the minimum possible</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1053}}<syntaxhighlight lang="lua">bGPTAllowed = g_Deal:IsPossibleToTradeItem(g_iThem, g_iUs, TradeableItems.TRADE_ITEM_GOLD_PER_TURN, 1, g_iDealDuration);   -- 1 here is 1 GPT, which is the minimum possible</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1067}}<syntaxhighlight lang="lua">local bOpenBordersAllowed = g_Deal:IsPossibleToTradeItem(g_iUs, g_iThem, TradeableItems.TRADE_ITEM_OPEN_BORDERS, g_iDealDuration);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1096}}<syntaxhighlight lang="lua">bOpenBordersAllowed = g_Deal:IsPossibleToTradeItem(g_iThem, g_iUs, TradeableItems.TRADE_ITEM_OPEN_BORDERS, g_iDealDuration);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1117}}<syntaxhighlight lang="lua">local bDefensivePactAllowed = g_Deal:IsPossibleToTradeItem(g_iUs, g_iThem, TradeableItems.TRADE_ITEM_DEFENSIVE_PACT, g_iDealDuration);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1149}}<syntaxhighlight lang="lua">bDefensivePactAllowed = g_Deal:IsPossibleToTradeItem(g_iThem, g_iUs, TradeableItems.TRADE_ITEM_DEFENSIVE_PACT, g_iDealDuration);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1164}}<syntaxhighlight lang="lua">local bResearchAgreementAllowed = g_Deal:IsPossibleToTradeItem(g_iUs, g_iThem, TradeableItems.TRADE_ITEM_RESEARCH_AGREEMENT, g_iDealDuration);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1204}}<syntaxhighlight lang="lua">bResearchAgreementAllowed = g_Deal:IsPossibleToTradeItem(g_iThem, g_iUs, TradeableItems.TRADE_ITEM_RESEARCH_AGREEMENT, g_iDealDuration);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1219}}<syntaxhighlight lang="lua">local bTradeAgreementAllowed = g_Deal:IsPossibleToTradeItem(g_iUs, g_iThem, TradeableItems.TRADE_ITEM_TRADE_AGREEMENT, g_iDealDuration);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1251}}<syntaxhighlight lang="lua">bTradeAgreementAllowed = g_Deal:IsPossibleToTradeItem(g_iThem, g_iUs, TradeableItems.TRADE_ITEM_TRADE_AGREEMENT, g_iDealDuration);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1268}}<syntaxhighlight lang="lua">if( g_Deal:IsPossibleToTradeItem( g_iUs, g_iThem, TradeableItems.TRADE_ITEM_CITIES, pCity:GetX(), pCity:GetY() ) ) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1286}}<syntaxhighlight lang="lua">if( g_Deal:IsPossibleToTradeItem( g_iThem, g_iUs, TradeableItems.TRADE_ITEM_CITIES, pCity:GetX(), pCity:GetY() ) ) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1357}}<syntaxhighlight lang="lua">bCanTradeResource = g_Deal:IsPossibleToTradeItem(g_iUs, g_iThem, TradeableItems.TRADE_ITEM_RESOURCES, resType, 1);   -- 1 here is 1 quanity of the Resource, which is the minimum possible</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1424}}<syntaxhighlight lang="lua">bCanTradeResource = g_Deal:IsPossibleToTradeItem(g_iThem, g_iUs, TradeableItems.TRADE_ITEM_RESOURCES, resType, 1);   -- 1 here is 1 quanity of the Resource, which is the minimum possible</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|2467}}<syntaxhighlight lang="lua">if ( g_Deal:IsPossibleToTradeItem( m_iFrom, m_iTo, TradeableItems.TRADE_ITEM_CITIES, pCity:GetX(), pCity:GetY() ) ) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|2561}}<syntaxhighlight lang="lua">g_Deal:IsPossibleToTradeItem( iFromPlayer, iToPlayer, tradeType, iLoopTeam ) ) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TradeLogic.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/WorldView/TradeLogic.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1084}}<syntaxhighlight lang="lua">local bAllowEmbassyAllowed = g_Deal:IsPossibleToTradeItem(g_iUs, g_iThem, TradeableItems.TRADE_ITEM_ALLOW_EMBASSY, g_iDealDuration);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1113}}<syntaxhighlight lang="lua">bEmbassyAllowed = g_Deal:IsPossibleToTradeItem(g_iThem, g_iUs, TradeableItems.TRADE_ITEM_ALLOW_EMBASSY, g_iDealDuration);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1363}}<syntaxhighlight lang="lua">local bDoFAllowed = g_Deal:IsPossibleToTradeItem(g_iUs, g_iThem, TradeableItems.TRADE_ITEM_DECLARATION_OF_FRIENDSHIP, g_iDealDuration);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|IsPossibleToTradeItem]]
[[Category:Civ5 Trade API|IsPossibleToTradeItem]]