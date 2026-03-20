{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|UI}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''bool''' UI.ProposedDealExists<b>(</b>{{Type5|PlayerID}} them, {{Type5|PlayerID}} us<b>)</b></code>


'''Returned Value'''
:No description available.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|them:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|us:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|TradeLogic.lua}}
:<code>UI/InGame/WorldView/TradeLogic.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0276}}<syntaxhighlight lang="lua">if( UI.ProposedDealExists( g_iUs, g_iThem ) ) then -- this is our proposal</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0281}}<syntaxhighlight lang="lua">elseif( UI.ProposedDealExists( g_iThem, g_iUs ) ) then -- this is their proposal</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|ProposedDealExists]]
[[Category:Civ5 Diplomacy API|ProposedDealExists]]
[[Category:Civ5 Trade API|ProposedDealExists]]