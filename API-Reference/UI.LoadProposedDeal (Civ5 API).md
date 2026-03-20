{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|UI}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''void''' UI.LoadProposedDeal<b>(</b>{{Type5|PlayerID}} us, {{Type5|PlayerID}} them<b>)</b></code>


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
{{CodeLine5|0278}}<syntaxhighlight lang="lua">UI.LoadProposedDeal( g_iUs, g_iThem );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0283}}<syntaxhighlight lang="lua">UI.LoadProposedDeal( g_iThem, g_iUs );</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|LoadProposedDeal]]
[[Category:Civ5 Movement API|LoadProposedDeal]]
[[Category:Civ5 Diplomacy API|LoadProposedDeal]]
[[Category:Civ5 Trade API|LoadProposedDeal]]