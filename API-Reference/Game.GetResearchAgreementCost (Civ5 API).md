{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Game}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''int''' Game.GetResearchAgreementCost<b>(</b>{{Type5|PlayerID}} us, {{Type5|PlayerID}} them<b>)</b></code>


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
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|TradeLogic.lua}}
:<code>UI/InGame/WorldView/TradeLogic.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0915}}<syntaxhighlight lang="lua">local iRACost = Game.GetResearchAgreementCost(g_iUs, g_iThem);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1166}}<syntaxhighlight lang="lua">local iCost = Game.GetResearchAgreementCost(g_iThem, g_iUs);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetResearchAgreementCost]]
[[Category:Civ5 Science API|GetResearchAgreementCost]]