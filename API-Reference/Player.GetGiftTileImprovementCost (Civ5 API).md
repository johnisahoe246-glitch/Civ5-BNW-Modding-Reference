{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Player}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''int''' Player:GetGiftTileImprovementCost<b>(</b>{{Type5|PlayerID}} activePlayer<b>)</b></code>


'''Returned Value'''
:No description available.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|activePlayer:
|valign="top"| ''No description available.''
|}


=Source code samples=
{{PseudoH4|CityStateDiploPopup.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/Popups/CityStateDiploPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0852}}<syntaxhighlight lang="lua">iGold = pPlayer:GetGiftTileImprovementCost(iActivePlayer);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetGiftTileImprovementCost]]
[[Category:Civ5 Improvements API|GetGiftTileImprovementCost]]
[[Category:Civ5 Diplomacy API|GetGiftTileImprovementCost]]
[[Category:Civ5 City States API|GetGiftTileImprovementCost]]