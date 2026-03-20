{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Player}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''int''' Player:GetGreatPeopleRateModifier<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|CityView.lua}}
:<code>UI/InGame/CityView/CityView.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0999}}<syntaxhighlight lang="lua">iMod = iMod + pPlayer:GetGreatPeopleRateModifier();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CityView.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/CityView/CityView.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1010}}<syntaxhighlight lang="lua">local iPlayerMod = pPlayer:GetGreatPeopleRateModifier();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|GPList.lua}}
:<code>UI/InGame/GPList.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0238}}<syntaxhighlight lang="lua">iMod = iMod + player:GetGreatPeopleRateModifier();</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetGreatPeopleRateModifier]]
[[Category:Civ5 Great People API|GetGreatPeopleRateModifier]]