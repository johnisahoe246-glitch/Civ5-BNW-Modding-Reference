{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Player}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''int''' Player:GetCurrentCapitalFoodBonus<b>(</b>{{Type5|PlayerID}} major<b>)</b></code>


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

{{PseudoH4|CityStateStatusHelper.lua (G&K)}}
:<code>DLC/Expansion/UI/CityStateStatusHelper.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0326}}<syntaxhighlight lang="lua">local iCapitalFoodBonus = pMinor:GetCurrentCapitalFoodBonus(iMajor) / 100;</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DiploRelationships.lua}}
:<code>UI/InGame/Popups/DiploRelationships.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0432}}<syntaxhighlight lang="lua">local iCapitalFoodBonus = pPlayer:GetCurrentCapitalFoodBonus(iActivePlayer) / 100;</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetCurrentCapitalFoodBonus]]
[[Category:Civ5 Cities API|GetCurrentCapitalFoodBonus]]
[[Category:Civ5 Food & Population API|GetCurrentCapitalFoodBonus]]