{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Network}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''void''' Network.SendFaithPurchase<b>(</b>{{Type5|PlayerID}} arg0, {{Type5|FaithPurchaseType}} v1, '''int''' v2<b>)</b></code>


'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|arg0:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|v1:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|v2:
|valign="top"| ''No description available.''
|}


=Source code samples=
{{PseudoH4|ReligionOverview.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/Popups/ReligionOverview.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0471}}<syntaxhighlight lang="lua">Network.SendFaithPurchase(Game.GetActivePlayer(), v1, v2);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|SendFaithPurchase]]
[[Category:Civ5 City Production API|SendFaithPurchase]]
[[Category:Civ5 Religion API|SendFaithPurchase]]