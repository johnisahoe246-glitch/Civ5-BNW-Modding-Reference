{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Deal}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''void''' Deal:SetToPlayer<b>(</b>{{Type5|PlayerID}} them<b>)</b></code>


'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|them:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|TradeLogic.lua}}
:<code>UI/InGame/WorldView/TradeLogic.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0138}}<syntaxhighlight lang="lua">g_Deal:SetToPlayer(g_iThem);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0290}}<syntaxhighlight lang="lua">g_Deal:SetToPlayer( g_iThem );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0442}}<syntaxhighlight lang="lua">if( g_iThem ~= -1 ) then g_Deal:SetToPlayer( g_iThem ); end</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|SetToPlayer]]
[[Category:Civ5 Players API|SetToPlayer]]