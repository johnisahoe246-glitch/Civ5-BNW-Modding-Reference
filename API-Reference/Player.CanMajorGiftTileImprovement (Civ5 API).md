{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Player}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''bool''' Player:CanMajorGiftTileImprovement<b>(</b>{{Type5|PlayerID}} activePlayer<b>)</b></code>


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
{{CodeLine5|0854}}<syntaxhighlight lang="lua">if (not pPlayer:CanMajorGiftTileImprovement(iActivePlayer)) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0939}}<syntaxhighlight lang="lua">if (pMinor:CanMajorGiftTileImprovement(iActivePlayer)) then</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|CanMajorGiftTileImprovement]]
[[Category:Civ5 Improvements API|CanMajorGiftTileImprovement]]
[[Category:Civ5 Diplomacy API|CanMajorGiftTileImprovement]]
[[Category:Civ5 City States API|CanMajorGiftTileImprovement]]