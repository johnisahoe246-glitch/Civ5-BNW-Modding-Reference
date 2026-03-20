{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|City}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''int''' City:FoodDifference<b>(</b>'''bool''' bottom<b>)</b></code>


'''Returned Value'''
:No description available.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|bottom:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|CityBannerManager.lua}}
:<code>UI/InGame/CityBannerManager.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0283}}<syntaxhighlight lang="lua">local iFoodPerTurn = city:FoodDifference();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CityList.lua}}
:<code>UI/InGame/CityList.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0171}}<syntaxhighlight lang="lua">local iFoodPerTurn = pCity:FoodDifference();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CityView.lua}}
:<code>UI/InGame/CityView/CityView.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1389}}<syntaxhighlight lang="lua">elseif pCity:FoodDifference() < 0 then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1404}}<syntaxhighlight lang="lua">local iFoodDiff = pCity:FoodDifference();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|EconomicGeneralInfo.lua}}
:<code>UI/InGame/Popups/EconomicGeneralInfo.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0148}}<syntaxhighlight lang="lua">sortEntry.Food = pCity:FoodDifference();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ProductionPopup.lua}}
:<code>UI/InGame/Popups/ProductionPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0219}}<syntaxhighlight lang="lua">Controls.Food:SetText( "[ICON_FOOD]" .. city:FoodDifference() );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0229}}<syntaxhighlight lang="lua">elseif city:FoodDifference() < 0 then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|WhosWinningPopup.lua}}
:<code>UI/InGame/Popups/WhosWinningPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0193}}<syntaxhighlight lang="lua">iTotalFoodSurplus = iTotalFoodSurplus + pLoopCity:FoodDifference();</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|FoodDifference]]
[[Category:Civ5 Food & Population API|FoodDifference]]