{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|City}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''int''' City:GetYieldRateTimes100<b>(</b>{{Type5|YieldType}} index<b>)</b></code>


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

{{PseudoH4|CityView.lua}}
:<code>UI/InGame/CityView/CityView.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1354}}<syntaxhighlight lang="lua">local iGoldPerTurn = pCity:GetYieldRateTimes100(YieldTypes.YIELD_GOLD) / 100;</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1362}}<syntaxhighlight lang="lua">local iSciencePerTurn = pCity:GetYieldRateTimes100(YieldTypes.YIELD_SCIENCE) / 100;</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|EconomicGeneralInfo.lua}}
:<code>UI/InGame/Popups/EconomicGeneralInfo.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0204}}<syntaxhighlight lang="lua">local CityIncome = pCity:GetYieldRateTimes100(YieldTypes.YIELD_GOLD) / 100;</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|InfoTooltipInclude.lua}}
:<code>UI/InGame/InfoTooltipInclude.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0625}}<syntaxhighlight lang="lua">iTotalYield = pCity:GetYieldRateTimes100(iYieldType) / 100;</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetYieldRateTimes100]]
[[Category:Civ5 Yields API|GetYieldRateTimes100]]