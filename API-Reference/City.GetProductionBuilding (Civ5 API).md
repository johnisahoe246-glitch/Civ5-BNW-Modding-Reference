{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|City}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>{{Type5|BuildingType}} City:GetProductionBuilding<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|CityView.lua}}
:<code>UI/InGame/CityView/CityView.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0848}}<syntaxhighlight lang="lua">local buildingProduction = pCity:GetProductionBuilding();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|2219}}<syntaxhighlight lang="lua">local buildingProduction = city:GetProductionBuilding();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ProductionPopup.lua}}
:<code>UI/InGame/Popups/ProductionPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0509}}<syntaxhighlight lang="lua">buildingProduction = city:GetProductionBuilding();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TutorialChecks.lua}}
:<code>Tutorial/TutorialChecks.lua</code>
:{{CodeBegin5}}
{{CodeLine5|2907}}<syntaxhighlight lang="lua">if (building.NoOccupiedUnhappiness and not pCity:IsHasBuilding(buildingID) and pCity:GetProductionBuilding() ~= buildingID) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|2957}}<syntaxhighlight lang="lua">if (not pCity:CanConstruct(buildingID) and not pCity:IsHasBuilding(buildingID) and pCity:GetProductionBuilding() ~= buildingID) then</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetProductionBuilding]]
[[Category:Civ5 City Production API|GetProductionBuilding]]
[[Category:Civ5 Buildings API|GetProductionBuilding]]