{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|City}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''int''' City:GetCurrentProductionDifferenceTimes100<b>(</b>'''bool''' ignoreFood, '''bool''' overflow<b>)</b></code>


'''Returned Value'''
:No description available.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|ignoreFood:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|overflow:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|CityView.lua}}
:<code>UI/InGame/CityView/CityView.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1529}}<syntaxhighlight lang="lua">local iProductionPerTurn = pCity:GetCurrentProductionDifferenceTimes100(false, false) / 100;--pCity:GetYieldRate(YieldTypes.YIELD_PRODUCTION);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1569}}<syntaxhighlight lang="lua">local bGeneratingProduction = pCity:IsProductionProcess() or pCity:GetCurrentProductionDifferenceTimes100(false, false) == 0;</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ProductionPopup.lua}}
:<code>UI/InGame/Popups/ProductionPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0259}}<syntaxhighlight lang="lua">if (city:GetCurrentProductionDifferenceTimes100(false, false) > 0) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0605}}<syntaxhighlight lang="lua">local iProductionPerTurn = city:GetCurrentProductionDifferenceTimes100(false, false) / 100;</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0632}}<syntaxhighlight lang="lua">local bGeneratingProduction = city:IsProductionProcess() or city:GetCurrentProductionDifferenceTimes100(false, false) == 0;</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetCurrentProductionDifferenceTimes100]]
[[Category:Civ5 City Production API|GetCurrentProductionDifferenceTimes100]]