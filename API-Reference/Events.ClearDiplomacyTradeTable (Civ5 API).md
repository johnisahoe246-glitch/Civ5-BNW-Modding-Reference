{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Events}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''void''' Events.ClearDiplomacyTradeTable<b>(</b><b>)</b></code>


'''Event Type'''
:Regular event: you can subscribe to it through <code>Events.ClearDiplomacyTradeTable.Add(''<function handler>'')</code> or invoke it directly through <code>Events.ClearDiplomacyTradeTable(''<arguments list>'')</code>.



=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|TradeLogic.lua}}
:<code>UI/InGame/WorldView/TradeLogic.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0722}}<syntaxhighlight lang="lua">Events.ClearDiplomacyTradeTable.Add(DoClearDeal);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|ClearDiplomacyTradeTable]]
[[Category:Civ5 Diplomacy API|ClearDiplomacyTradeTable]]
[[Category:Civ5 Trade API|ClearDiplomacyTradeTable]]