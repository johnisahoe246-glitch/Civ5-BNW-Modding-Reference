{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|City}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''int''' City:GetDamage<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|CityBannerManager.lua}}
:<code>UI/InGame/CityBannerManager.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0453}}<syntaxhighlight lang="lua">RefreshCityDamage( cityBanner, city:GetDamage() );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CityBannerManager.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/CityBannerManager.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0519}}<syntaxhighlight lang="lua">RefreshCityDamage( cityBanner, city:GetDamage(), city:GetMaxHitPoints() );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CityList.lua}}
:<code>UI/InGame/CityList.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0132}}<syntaxhighlight lang="lua">local iHealthPercent = 1 - (pCity:GetDamage() / GameDefines.MAX_CITY_HIT_POINTS);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CityList.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/CityList.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0132}}<syntaxhighlight lang="lua">local iHealthPercent = 1 - (pCity:GetDamage() / pCity:GetMaxHitPoints());</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CityView.lua}}
:<code>UI/InGame/CityView/CityView.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0717}}<syntaxhighlight lang="lua">OnCitySetDamage(pCity:GetDamage());</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CityView.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/CityView/CityView.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0726}}<syntaxhighlight lang="lua">OnCitySetDamage(pCity:GetDamage(), pCity:GetMaxHitPoints());</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|EconomicGeneralInfo.lua}}
:<code>UI/InGame/Popups/EconomicGeneralInfo.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0093}}<syntaxhighlight lang="lua">local pct = 1 - (pCity:GetDamage() / GameDefines.MAX_CITY_HIT_POINTS);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|EconomicGeneralInfo.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/Popups/EconomicGeneralInfo.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0093}}<syntaxhighlight lang="lua">local pct = 1 - (pCity:GetDamage() / pCity:GetMaxHitPoints());</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|EnemyUnitPanel.lua}}
:<code>UI/InGame/WorldView/EnemyUnitPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1414}}<syntaxhighlight lang="lua">local myCityCurHP = myCity:GetDamage();</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetDamage]]
[[Category:Civ5 Combat API|GetDamage]]