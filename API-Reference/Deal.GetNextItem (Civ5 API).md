{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Deal}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>{{Type5|TradeableItemType}}, '''unknown''', '''unknown''', {{Type5|ResourceType}}, '''int''', {{Type5|PlayerID}} Deal:GetNextItem<b>(</b><b>)</b></code>


'''Returned Values'''
:No description available.


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|TradeLogic.lua}}
:<code>UI/InGame/WorldView/TradeLogic.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0642}}<syntaxhighlight lang="lua">itemType, duration, finalTurn, data1, data2, fromPlayer = g_Deal:GetNextItem();</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetNextItem]]