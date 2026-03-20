{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Deal}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''void''' Deal:AddDeclarationOfFriendship<b>(</b>{{Type5|PlayerID}} us<b>)</b></code>


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
{{CodeLine5|2294}}<syntaxhighlight lang="lua">g_Deal:AddDeclarationOfFriendship(g_iUs);</syntaxhighlight>
{{CodeLine5|2295}}<syntaxhighlight lang="lua">g_Deal:AddDeclarationOfFriendship(g_iThem);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|AddDeclarationOfFriendship]]