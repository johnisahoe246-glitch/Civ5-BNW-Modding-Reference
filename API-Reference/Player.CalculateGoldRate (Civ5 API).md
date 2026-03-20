{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Player}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''int''' Player:CalculateGoldRate<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|DiploRelationships.lua}}
:<code>UI/InGame/Popups/DiploRelationships.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0289}}<syntaxhighlight lang="lua">local iGoldPerTurn = Players[iPlayer]:CalculateGoldRate();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TopPanel.lua}}
:<code>UI/InGame/TopPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0042}}<syntaxhighlight lang="lua">local iGoldPerTurn = pPlayer:CalculateGoldRate();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TradeLogic.lua}}
:<code>UI/InGame/WorldView/TradeLogic.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1034}}<syntaxhighlight lang="lua">local iGoldPerTurn = g_pUs:CalculateGoldRate();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1049}}<syntaxhighlight lang="lua">iGoldPerTurn = g_pThem:CalculateGoldRate();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1686}}<syntaxhighlight lang="lua">strTooltip = Locale.ConvertTextKey( "TXT_KEY_DIPLO_CURRENT_GPT", g_pUs:CalculateGoldRate() - data1 );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1695}}<syntaxhighlight lang="lua">strTooltip = Locale.ConvertTextKey( "TXT_KEY_DIPLO_CURRENT_GPT", g_pThem:CalculateGoldRate() - data1 );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1976}}<syntaxhighlight lang="lua">if (iGoldPerTurn > g_pUs:CalculateGoldRate()) then</syntaxhighlight>
{{CodeLine5|1977}}<syntaxhighlight lang="lua">iGoldPerTurn = g_pUs:CalculateGoldRate();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1983}}<syntaxhighlight lang="lua">if (iGoldPerTurn > g_pThem:CalculateGoldRate()) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|2039}}<syntaxhighlight lang="lua">local strTooltip = Locale.ConvertTextKey( "TXT_KEY_DIPLO_CURRENT_GPT", g_pUs:CalculateGoldRate() - iGoldPerTurn );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|2052}}<syntaxhighlight lang="lua">local strTooltip = Locale.ConvertTextKey( "TXT_KEY_DIPLO_CURRENT_GPT", g_pThem:CalculateGoldRate() - iGoldPerTurn );</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|CalculateGoldRate]]
[[Category:Civ5 Gold API|CalculateGoldRate]]