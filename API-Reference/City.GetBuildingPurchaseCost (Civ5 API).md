{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|City}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''int''' City:GetBuildingPurchaseCost<b>(</b>{{Type5|BuildingType}} building<b>)</b></code>


'''Returned Value'''
:No description available.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|building:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|ProductionPopup.lua}}
:<code>UI/InGame/Popups/ProductionPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0399}}<syntaxhighlight lang="lua">local cost = city:GetBuildingPurchaseCost( buildingID );</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetBuildingPurchaseCost]]
[[Category:Civ5 City Production API|GetBuildingPurchaseCost]]
[[Category:Civ5 Buildings API|GetBuildingPurchaseCost]]