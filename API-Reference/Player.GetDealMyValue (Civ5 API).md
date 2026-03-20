{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Player}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>{{Type5|SpecialistType}} Player:GetDealMyValue<b>(</b>{{Type5|Deal}} Deal<b>)</b></code>


'''Returned Value'''
:No description available.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|Deal:
|valign="top"| ''No description available.''
|}


=Source code samples=
{{PseudoH4|TradeLogic.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/WorldView/TradeLogic.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0372}}<syntaxhighlight lang="lua">iDealValue = g_pUs:GetDealMyValue(g_Deal);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetDealMyValue]]
[[Category:Civ5 Diplomacy API|GetDealMyValue]]
[[Category:Civ5 Trade API|GetDealMyValue]]