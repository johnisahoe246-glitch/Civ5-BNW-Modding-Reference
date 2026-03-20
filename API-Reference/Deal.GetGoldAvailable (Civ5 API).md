{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Deal}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''int''' Deal:GetGoldAvailable<b>(</b>{{Type5|PlayerID}} us, {{Type5|TradeableItemType}} itemToBeChanged<b>)</b></code>


'''Returned Value'''
:No description available.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|us:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|itemToBeChanged:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|DiploRelationships.lua}}
:<code>UI/InGame/Popups/DiploRelationships.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0278}}<syntaxhighlight lang="lua">local iGold = g_Deal:GetGoldAvailable(iPlayer, iItemToBeChanged);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TradeLogic.lua}}
:<code>UI/InGame/WorldView/TradeLogic.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1000}}<syntaxhighlight lang="lua">local iGold = g_Deal:GetGoldAvailable(g_iUs, iItemToBeChanged);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1015}}<syntaxhighlight lang="lua">iGold = g_Deal:GetGoldAvailable(g_iThem, iItemToBeChanged);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1663}}<syntaxhighlight lang="lua">strTooltip = Locale.ConvertTextKey( "TXT_KEY_DIPLO_CURRENT_GOLD", g_Deal:GetGoldAvailable(g_iUs, iItemToBeChanged) );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1670}}<syntaxhighlight lang="lua">strTooltip = Locale.ConvertTextKey( "TXT_KEY_DIPLO_CURRENT_GOLD", g_Deal:GetGoldAvailable(g_iThem, iItemToBeChanged) );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1876}}<syntaxhighlight lang="lua">iAmountAvailable = g_Deal:GetGoldAvailable(g_iUs, iItemToBeChanged);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1883}}<syntaxhighlight lang="lua">iAmountAvailable = g_Deal:GetGoldAvailable(g_iThem, iItemToBeChanged);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1926}}<syntaxhighlight lang="lua">iAmountAvailable = g_Deal:GetGoldAvailable(g_iUs, TradeableItems.TRADE_ITEM_GOLD);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1935}}<syntaxhighlight lang="lua">local strTooltip = Locale.ConvertTextKey( "TXT_KEY_DIPLO_CURRENT_GOLD", g_Deal:GetGoldAvailable(g_iUs, iItemToBeChanged) );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1941}}<syntaxhighlight lang="lua">iAmountAvailable = g_Deal:GetGoldAvailable(g_iThem, TradeableItems.TRADE_ITEM_GOLD);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1950}}<syntaxhighlight lang="lua">local strTooltip = Locale.ConvertTextKey( "TXT_KEY_DIPLO_CURRENT_GOLD", g_Deal:GetGoldAvailable(g_iThem, iItemToBeChanged) );</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetGoldAvailable]]
[[Category:Civ5 Gold API|GetGoldAvailable]]