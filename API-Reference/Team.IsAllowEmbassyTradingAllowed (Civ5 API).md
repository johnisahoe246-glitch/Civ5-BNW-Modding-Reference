{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Team}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''bool''' Team:IsAllowEmbassyTradingAllowed<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
{{PseudoH4|TradeLogic.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/WorldView/TradeLogic.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1093}}<syntaxhighlight lang="lua">if (not g_pThemTeam:IsAllowEmbassyTradingAllowed()) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1116}}<syntaxhighlight lang="lua">if (not g_pUsTeam:IsAllowEmbassyTradingAllowed()) then</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|IsAllowEmbassyTradingAllowed]]
[[Category:Civ5 Diplomacy API|IsAllowEmbassyTradingAllowed]]
[[Category:Civ5 Trade API|IsAllowEmbassyTradingAllowed]]