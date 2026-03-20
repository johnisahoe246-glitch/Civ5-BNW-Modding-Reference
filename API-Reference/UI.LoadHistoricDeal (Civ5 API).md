{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|UI}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''void''' UI.LoadHistoricDeal<b>(</b>{{Type5|PlayerID}} player, {{Type5|SpecialistType}} i<b>)</b></code>


'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|player:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|i:
|valign="top"| ''No description available.''
|}


=Source code samples=
{{PseudoH4|DiploCurrentDeals.lua}}
:<code>UI/InGame/Popups/DiploCurrentDeals.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0060}}<syntaxhighlight lang="lua">UI.LoadHistoricDeal( iPlayer, i );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0143}}<syntaxhighlight lang="lua">UI.LoadHistoricDeal( iPlayer, index );</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|LoadHistoricDeal]]
[[Category:Civ5 Movement API|LoadHistoricDeal]]
[[Category:Civ5 Diplomacy API|LoadHistoricDeal]]
[[Category:Civ5 Trade API|LoadHistoricDeal]]