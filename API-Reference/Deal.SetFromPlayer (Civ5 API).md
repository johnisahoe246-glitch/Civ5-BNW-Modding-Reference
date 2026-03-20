{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Deal}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''void''' Deal:SetFromPlayer<b>(</b>{{Type5|PlayerID}} us<b>)</b></code>


'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|us:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|TradeLogic.lua}}
:<code>UI/InGame/WorldView/TradeLogic.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0137}}<syntaxhighlight lang="lua">g_Deal:SetFromPlayer(g_iUs);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0289}}<syntaxhighlight lang="lua">g_Deal:SetFromPlayer( g_iUs );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0441}}<syntaxhighlight lang="lua">if( g_iUs   ~= -1 ) then g_Deal:SetFromPlayer( g_iUs   ); end</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|SetFromPlayer]]
[[Category:Civ5 Players API|SetFromPlayer]]