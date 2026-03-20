{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|City}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''int''' City:GetProductionModifier<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|CityView.lua}}
:<code>UI/InGame/CityView/CityView.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1530}}<syntaxhighlight lang="lua">local iProductionModifier = pCity:GetProductionModifier() + 100;</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|EconomicGeneralInfo.lua}}
:<code>UI/InGame/Popups/EconomicGeneralInfo.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0152}}<syntaxhighlight lang="lua">local totalProductionPerTurn = math.floor(productionYield + (productionYield * (pCity:GetProductionModifier() / 100)));</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ProductionPopup.lua}}
:<code>UI/InGame/Popups/ProductionPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0211}}<syntaxhighlight lang="lua">local productionPerTurn = math.floor(productionYield + (productionYield * (city:GetProductionModifier() / 100)));</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0606}}<syntaxhighlight lang="lua">local iProductionModifier = city:GetProductionModifier() + 100;</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetProductionModifier]]
[[Category:Civ5 City Production API|GetProductionModifier]]