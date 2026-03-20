{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|ID.png|The <code>TradeableItemType</code> pseudo-type is actually a regular '''integer'''. Pseudo-types do not exist in Lua, they only serve a documentation purpose on the wiki!
* {{Lua}} Integers labeled as <code>TradeableItemType</code> corresponds to the constants defined in the '''TradeableItems''' Lua enumeration.
}}


= Lua: the TradeableItems enumeration =
Firaxis provides a Lua enumeration named <code>TradeableItems</code>. This is just a regular global table. Its keys are the constants' names and the pairs the corresponding values.

<br/>Below are the values found in this enumeration.
<code>
{|
|-
!align="left" |Key
!
!align="left" |Value 
|-
|align="left" |"TRADE_ITEM_NONE"
|
|align="right" |-1
|-
|align="left" |"TRADE_ITEM_GOLD"
|
|align="right" |0
|-
|align="left" |"TRADE_ITEM_GOLD_PER_TURN"
|
|align="right" |1
|-
|align="left" |"TRADE_ITEM_MAPS"
|
|align="right" |2
|-
|align="left" |"TRADE_ITEM_RESOURCES"
|
|align="right" |3
|-
|align="left" |"TRADE_ITEM_CITIES"
|
|align="right" |4
|-
|align="left" |"TRADE_ITEM_UNITS"
|
|align="right" |5
|-
|align="left" |"TRADE_ITEM_OPEN_BORDERS"
|
|align="right" |6
|-
|align="left" |"TRADE_ITEM_DEFENSIVE_PACT"
|
|align="right" |7
|-
|align="left" |"TRADE_ITEM_RESEARCH_AGREEMENT"
|
|align="right" |8
|-
|align="left" |"TRADE_ITEM_TRADE_AGREEMENT"
|
|align="right" |9
|-
|align="left" |"TRADE_ITEM_PERMANENT_ALLIANCE"
|
|align="right" |10
|-
|align="left" |"TRADE_ITEM_SURRENDER"
|
|align="right" |11
|-
|align="left" |"TRADE_ITEM_TRUCE"
|
|align="right" |12
|-
|align="left" |"TRADE_ITEM_PEACE_TREATY"
|
|align="right" |13
|-
|align="left" |"TRADE_ITEM_THIRD_PARTY_PEACE"
|
|align="right" |14
|-
|align="left" |"TRADE_ITEM_THIRD_PARTY_WAR"
|
|align="right" |15
|-
|align="left" |"TRADE_ITEM_THIRD_PARTY_EMBARGO"
|
|align="right" |16
|-
|align="left" |"TRADE_ITEM_ALLOW_EMBASSY"
|
|align="right" |17
|-
|align="left" |"TRADE_ITEM_DECLARATION_OF_FRIENDSHIP"
|
|align="right" |18
|-
|align="left" |"NUM_TRADEABLE_ITEMS"
|
|align="right" |19
|}</code>


= Examples =
Here is how to use the LUA enumeration to retrieve the ''ID'' from the ''type''. Those examples will return and assign the integer value 0.
<syntaxhighlight lang="lua" class="civ5-example">
local id = TradeableItems.TRADE_ITEM_GOLD
local id = TradeableItems["TRADE_ITEM_GOLD"]
</syntaxhighlight>


=Used by=
{|cellspacing="4" cellpadding="0" width="100%" style="background-color:#F0F0F0"
<!-- 
GETGOLDAVAILABLE
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Deal}}:{{Func5|Deal|GetGoldAvailable}}<b>(</b>{{Type5|PlayerID}} us, {{Type5|TradeableItemType}} itemToBeChanged<b>)</b></code>
<!-- 
GETNEXTITEM
-->
|-
|align="right" width="200" |<code>{{Type5|TradeableItemType}}, '''unknown''', '''unknown''', {{Type5|ResourceType}}, '''int''', {{Type5|PlayerID}}</code>
|style="padding-left:6px" |<code>{{Type5|Deal}}:{{Func5|Deal|GetNextItem}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ISPOSSIBLETOTRADEITEM
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Deal}}:{{Func5|Deal|IsPossibleToTradeItem}}<b>(</b>{{Type5|PlayerID}} us, {{Type5|PlayerID}} them, {{Type5|TradeableItemType}} tradeType, {{Type5|TeamID}} dealDuration, {{Type5|ResourceType}} dealDuration = nil<b>)</b></code>
<!-- 
REMOVEBYTYPE
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Deal}}:{{Func5|Deal|RemoveByType}}<b>(</b>{{Type5|TradeableItemType}} arg0, {{Type5|PlayerID}} us<b>)</b></code>
|}




{{Civ5 API Footer}}
[[Category:Civ5 Types|TradeableItemType]]