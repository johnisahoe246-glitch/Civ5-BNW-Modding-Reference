{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Team}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''bool''' Team:IsResearchAgreementTradingAllowed<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|TradeLogic.lua}}
:<code>UI/InGame/WorldView/TradeLogic.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1179}}<syntaxhighlight lang="lua">elseif (not g_pUsTeam:IsResearchAgreementTradingAllowed() and not g_pThemTeam:IsResearchAgreementTradingAllowed()) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TradeLogic.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/WorldView/TradeLogic.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1264}}<syntaxhighlight lang="lua">if (not g_pUsTeam:IsResearchAgreementTradingAllowed() and not g_pThemTeam:IsResearchAgreementTradingAllowed()) then</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|IsResearchAgreementTradingAllowed]]
[[Category:Civ5 Science API|IsResearchAgreementTradingAllowed]]
[[Category:Civ5 Trade API|IsResearchAgreementTradingAllowed]]