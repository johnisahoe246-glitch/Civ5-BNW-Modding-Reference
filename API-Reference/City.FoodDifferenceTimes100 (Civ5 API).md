{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|City}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''int''' City:FoodDifferenceTimes100<b>(</b>'''bool''' bottom<b>)</b></code>


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
{{CodeLine5|0254}}<syntaxhighlight lang="lua">elseif city:FoodDifferenceTimes100() < 0 then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CityList.lua}}
:<code>UI/InGame/CityList.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0188}}<syntaxhighlight lang="lua">if (pCity:IsFoodProduction() or pCity:FoodDifferenceTimes100() == 0) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0191}}<syntaxhighlight lang="lua">elseif pCity:FoodDifferenceTimes100() < 0 then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CityView.lua}}
:<code>UI/InGame/CityView/CityView.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1394}}<syntaxhighlight lang="lua">local iFoodPerTurn = pCity:FoodDifferenceTimes100() / 100;</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|InfoTooltipInclude.lua}}
:<code>UI/InGame/InfoTooltipInclude.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0623}}<syntaxhighlight lang="lua">iTotalYield = pCity:FoodDifferenceTimes100() / 100;</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ProductionPopup.lua}}
:<code>UI/InGame/Popups/ProductionPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0227}}<syntaxhighlight lang="lua">if (city:IsFoodProduction() or city:FoodDifferenceTimes100() == 0) then</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|FoodDifferenceTimes100]]
[[Category:Civ5 Food & Population API|FoodDifferenceTimes100]]