{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|City}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''int''' City:GetYieldRate<b>(</b>{{Type5|YieldType}} index<b>)</b></code>


'''Returned Value'''
:No description available.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|index:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|CityBannerManager.lua}}
:<code>UI/InGame/CityBannerManager.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0302}}<syntaxhighlight lang="lua">local iProductionPerTurn = city:GetYieldRate(YieldTypes.YIELD_PRODUCTION);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0304}}<syntaxhighlight lang="lua">iProductionPerTurn = iProductionPerTurn + city:GetYieldRate(YieldTypes.YIELD_FOOD) - city:FoodConsumption(true);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|EconomicGeneralInfo.lua}}
:<code>UI/InGame/Popups/EconomicGeneralInfo.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0151}}<syntaxhighlight lang="lua">local productionYield = pCity:GetYieldRate( YieldTypes.YIELD_PRODUCTION );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0157}}<syntaxhighlight lang="lua">sortEntry.Science = pCity:GetYieldRate( YieldTypes.YIELD_SCIENCE );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0160}}<syntaxhighlight lang="lua">sortEntry.Gold = pCity:GetYieldRate( YieldTypes.YIELD_GOLD );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|InfoTooltipInclude.lua}}
:<code>UI/InGame/InfoTooltipInclude.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0700}}<syntaxhighlight lang="lua">local iFoodSurplus = pCity:GetYieldRate(YieldTypes.YIELD_FOOD) - iYieldEaten;</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ProductionPopup.lua}}
:<code>UI/InGame/Popups/ProductionPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0210}}<syntaxhighlight lang="lua">local productionYield = city:GetYieldRate(YieldTypes.YIELD_PRODUCTION);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0213}}<syntaxhighlight lang="lua">local scienceYield = city:GetYieldRate(YieldTypes.YIELD_SCIENCE);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0222}}<syntaxhighlight lang="lua">Controls.Gold:SetText( "[ICON_GOLD]" .. city:GetYieldRate( YieldTypes.YIELD_GOLD ) );</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetYieldRate]]
[[Category:Civ5 Yields API|GetYieldRate]]