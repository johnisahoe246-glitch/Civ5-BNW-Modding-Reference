{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|City}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>{{Type5|UnitType}} City:GetProductionUnit<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|CityView.lua}}
:<code>UI/InGame/CityView/CityView.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0847}}<syntaxhighlight lang="lua">local unitProduction = pCity:GetProductionUnit();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|2218}}<syntaxhighlight lang="lua">local unitProduction = city:GetProductionUnit();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ProductionPopup.lua}}
:<code>UI/InGame/Popups/ProductionPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0508}}<syntaxhighlight lang="lua">unitProduction = city:GetProductionUnit();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TutorialChecks.lua}}
:<code>Tutorial/TutorialChecks.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0258}}<syntaxhighlight lang="lua">local UnitType = v:GetProductionUnit();</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetProductionUnit]]
[[Category:Civ5 City Production API|GetProductionUnit]]
[[Category:Civ5 Units API|GetProductionUnit]]