{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|UI}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''void''' UI.DoFinalizePlayerDeal<b>(</b>{{Type5|PlayerID}} them, {{Type5|PlayerID}} us, '''bool''' arg2<b>)</b></code>


'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|them:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|us:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|arg2:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|TradeLogic.lua}}
:<code>UI/InGame/WorldView/TradeLogic.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0348}}<syntaxhighlight lang="lua">UI.DoFinalizePlayerDeal( g_iThem, g_iUs, false );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0807}}<syntaxhighlight lang="lua">UI.DoFinalizePlayerDeal( g_iUs, g_iThem, false );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0810}}<syntaxhighlight lang="lua">UI.DoFinalizePlayerDeal( g_iThem, g_iUs, true );</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|DoFinalizePlayerDeal]]
[[Category:Civ5 Players API|DoFinalizePlayerDeal]]
[[Category:Civ5 Diplomacy API|DoFinalizePlayerDeal]]
[[Category:Civ5 Trade API|DoFinalizePlayerDeal]]