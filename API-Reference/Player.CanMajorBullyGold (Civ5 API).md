{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Player}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''bool''' Player:CanMajorBullyGold<b>(</b>{{Type5|PlayerID}} major<b>)</b></code>


'''Returned Value'''
:No description available.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|major:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|CityStateDiploPopup.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/Popups/CityStateDiploPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0979}}<syntaxhighlight lang="lua">if (not pPlayer:CanMajorBullyGold(iActivePlayer)) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1055}}<syntaxhighlight lang="lua">if (pPlayer:CanMajorBullyGold(iActivePlayer)) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CityStateStatusHelper.lua (G&K)}}
:<code>DLC/Expansion/UI/CityStateStatusHelper.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0061}}<syntaxhighlight lang="lua">local bCanBully = pMinor:CanMajorBullyGold(iMajor);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|CanMajorBullyGold]]
[[Category:Civ5 Gold API|CanMajorBullyGold]]
[[Category:Civ5 Diplomacy API|CanMajorBullyGold]]