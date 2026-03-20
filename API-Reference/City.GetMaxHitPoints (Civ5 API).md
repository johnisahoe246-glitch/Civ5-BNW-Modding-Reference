{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|City}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''int''' City:GetMaxHitPoints<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
{{PseudoH4|CityBannerManager.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/CityBannerManager.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0519}}<syntaxhighlight lang="lua">RefreshCityDamage( cityBanner, city:GetDamage(), city:GetMaxHitPoints() );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0873}}<syntaxhighlight lang="lua">RefreshCityDamage(instance, iDamage, city:GetMaxHitPoints());</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CityList.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/CityList.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0132}}<syntaxhighlight lang="lua">local iHealthPercent = 1 - (pCity:GetDamage() / pCity:GetMaxHitPoints());</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CityView.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/CityView/CityView.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0726}}<syntaxhighlight lang="lua">OnCitySetDamage(pCity:GetDamage(), pCity:GetMaxHitPoints());</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|EconomicGeneralInfo.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/Popups/EconomicGeneralInfo.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0093}}<syntaxhighlight lang="lua">local pct = 1 - (pCity:GetDamage() / pCity:GetMaxHitPoints());</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|EnemyUnitPanel.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/WorldView/EnemyUnitPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1584}}<syntaxhighlight lang="lua">local myCityMaxHP = myCity:GetMaxHitPoints();</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetMaxHitPoints]]
[[Category:Civ5 Combat API|GetMaxHitPoints]]