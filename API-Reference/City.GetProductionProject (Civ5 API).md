{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|City}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>{{Type5|ProjectType}} City:GetProductionProject<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|CityView.lua}}
:<code>UI/InGame/CityView/CityView.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0849}}<syntaxhighlight lang="lua">local projectProduction = pCity:GetProductionProject();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|2220}}<syntaxhighlight lang="lua">local projectProduction = city:GetProductionProject();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ProductionPopup.lua}}
:<code>UI/InGame/Popups/ProductionPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0510}}<syntaxhighlight lang="lua">projectProduction = city:GetProductionProject();</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetProductionProject]]
[[Category:Civ5 City Production API|GetProductionProject]]
[[Category:Civ5 Buildings API|GetProductionProject]]