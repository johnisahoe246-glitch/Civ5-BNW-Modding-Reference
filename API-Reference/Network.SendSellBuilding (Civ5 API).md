{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Network}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''void''' Network.SendSellBuilding<b>(</b>{{Type5|CityID}} arg0, {{Type5|BuildingType}} buildingToSell<b>)</b></code>


'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|arg0:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|buildingToSell:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|CityView.lua}}
:<code>UI/InGame/CityView/CityView.lua</code>
:{{CodeBegin5}}
{{CodeLine5|2375}}<syntaxhighlight lang="lua">Network.SendSellBuilding(pCity:GetID(), g_iBuildingToSell);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|SendSellBuilding]]
[[Category:Civ5 Buildings API|SendSellBuilding]]