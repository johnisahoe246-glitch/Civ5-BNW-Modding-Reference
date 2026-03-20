{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Game}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''void''' Game.CityPurchaseBuilding<b>(</b>{{Type5|City}} city, {{Type5|UnitType}} unitType, '''int''' buildingType, {{Type5|ProjectType}} projectTypes<b>)</b></code>


'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|city:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|unitType:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|buildingType:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|projectTypes:
|valign="top"| ''No description available.''
|}


=Source code samples=
{{PseudoH4|ProductionPopup.lua}}
:<code>UI/InGame/Popups/ProductionPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0069}}<syntaxhighlight lang="lua">Game.CityPurchaseBuilding(city, iData);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ProductionPopup.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/Popups/ProductionPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0117}}<syntaxhighlight lang="lua">Game.CityPurchaseBuilding(city, iData, eYield);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|CityPurchaseBuilding]]
[[Category:Civ5 Cities API|CityPurchaseBuilding]]
[[Category:Civ5 City Production API|CityPurchaseBuilding]]
[[Category:Civ5 Buildings API|CityPurchaseBuilding]]