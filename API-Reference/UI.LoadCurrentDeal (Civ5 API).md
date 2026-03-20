{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|UI}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''void''' UI.LoadCurrentDeal<b>(</b>{{Type5|PlayerID}} player, {{Type5|SpecialistType}} i<b>)</b></code>


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
{{CodeLine5|0036}}<syntaxhighlight lang="lua">UI.LoadCurrentDeal( iPlayer, i );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0141}}<syntaxhighlight lang="lua">UI.LoadCurrentDeal( iPlayer, index );</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|LoadCurrentDeal]]
[[Category:Civ5 Movement API|LoadCurrentDeal]]
[[Category:Civ5 Diplomacy API|LoadCurrentDeal]]
[[Category:Civ5 Trade API|LoadCurrentDeal]]