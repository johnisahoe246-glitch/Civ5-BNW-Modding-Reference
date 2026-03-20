{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|City}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''int''' City:GetBuildingFaithPurchaseCost<b>(</b>{{Type5|BuildingType}} building, '''bool''' arg1 = nil<b>)</b></code>


'''Returned Value'''
:No description available.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|building:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|arg1:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|ProductionPopup.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/Popups/ProductionPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0487}}<syntaxhighlight lang="lua">local cost = city:GetBuildingFaithPurchaseCost( buildingID );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ReligionOverview.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/Popups/ReligionOverview.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0427}}<syntaxhighlight lang="lua">local faithCost = capital:GetBuildingFaithPurchaseCost(GameInfo.Buildings[v2].ID, true);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0457}}<syntaxhighlight lang="lua">local faithCost = capital:GetBuildingFaithPurchaseCost(building.ID);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetBuildingFaithPurchaseCost]]
[[Category:Civ5 City Production API|GetBuildingFaithPurchaseCost]]
[[Category:Civ5 Buildings API|GetBuildingFaithPurchaseCost]]
[[Category:Civ5 Religion API|GetBuildingFaithPurchaseCost]]