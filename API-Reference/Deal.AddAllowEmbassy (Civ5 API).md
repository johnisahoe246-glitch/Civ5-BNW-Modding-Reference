{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Deal}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''void''' Deal:AddAllowEmbassy<b>(</b>{{Type5|PlayerID}} us<b>)</b></code>


'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|us:
|valign="top"| ''No description available.''
|}


=Source code samples=
{{PseudoH4|TradeLogic.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/WorldView/TradeLogic.lua</code>
:{{CodeBegin5}}
{{CodeLine5|2257}}<syntaxhighlight lang="lua">g_Deal:AddAllowEmbassy(g_iUs);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|2259}}<syntaxhighlight lang="lua">g_Deal:AddAllowEmbassy(g_iThem);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|AddAllowEmbassy]]
[[Category:Civ5 Diplomacy API|AddAllowEmbassy]]