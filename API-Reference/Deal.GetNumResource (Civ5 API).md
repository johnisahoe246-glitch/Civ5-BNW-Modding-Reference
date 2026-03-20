{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Deal}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''int''' Deal:GetNumResource<b>(</b>{{Type5|PlayerID}} us, {{Type5|ResourceType}} resType<b>)</b></code>


'''Returned Value'''
:No description available.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|us:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|resType:
|valign="top"| ''No description available.''
|}


=Source code samples=
{{PseudoH4|TradeLogic.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/WorldView/TradeLogic.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1500}}<syntaxhighlight lang="lua">iResourceCount = g_Deal:GetNumResource(g_iUs, resType);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1567}}<syntaxhighlight lang="lua">iResourceCount = g_Deal:GetNumResource(g_iThem, resType);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|2475}}<syntaxhighlight lang="lua">if (iAmount > g_Deal:GetNumResource(g_iUs, resourceId)) then</syntaxhighlight>
{{CodeLine5|2476}}<syntaxhighlight lang="lua">iAmount = g_Deal:GetNumResource(g_iUs, resourceId);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|2480}}<syntaxhighlight lang="lua">if (iAmount > g_Deal:GetNumResource(g_iThem, resourceId)) then</syntaxhighlight>
{{CodeLine5|2481}}<syntaxhighlight lang="lua">iAmount = g_Deal:GetNumResource(g_iThem, resourceId);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|2582}}<syntaxhighlight lang="lua">if (iNumResource > g_Deal:GetNumResource(iPlayer, iResourceID)) then</syntaxhighlight>
{{CodeLine5|2583}}<syntaxhighlight lang="lua">iNumResource = g_Deal:GetNumResource(iPlayer, iResourceID);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetNumResource]]
[[Category:Civ5 Resources API|GetNumResource]]