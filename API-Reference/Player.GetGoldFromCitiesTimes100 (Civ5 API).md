{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Player}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''int''' Player:GetGoldFromCitiesTimes100<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|EconomicGeneralInfo.lua}}
:<code>UI/InGame/Popups/EconomicGeneralInfo.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0198}}<syntaxhighlight lang="lua">Controls.CityIncomeValue:SetText( Locale.ToNumber( pPlayer:GetGoldFromCitiesTimes100() / 100, "#.##" ) );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TopPanel.lua}}
:<code>UI/InGame/TopPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0430}}<syntaxhighlight lang="lua">local fGoldPerTurnFromCities = pPlayer:GetGoldFromCitiesTimes100() / 100;</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetGoldFromCitiesTimes100]]
[[Category:Civ5 Cities API|GetGoldFromCitiesTimes100]]
[[Category:Civ5 Gold API|GetGoldFromCitiesTimes100]]