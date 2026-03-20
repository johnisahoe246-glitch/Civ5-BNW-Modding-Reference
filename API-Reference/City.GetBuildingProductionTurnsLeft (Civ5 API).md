{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|City}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''int''' City:GetBuildingProductionTurnsLeft<b>(</b>{{Type5|BuildingType}} building, '''int''' num<b>)</b></code>


'''Returned Value'''
:No description available.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|building:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|num:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|CityView.lua}}
:<code>UI/InGame/CityView/CityView.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0590}}<syntaxhighlight lang="lua">Controls[controlTurns]:SetText(  Locale.ConvertTextKey("TXT_KEY_PRODUCTION_HELP_NUM_TURNS", city:GetBuildingProductionTurnsLeft(queuedData1, queuedItemNumber-1)) );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ProductionPopup.lua}}
:<code>UI/InGame/Popups/ProductionPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0374}}<syntaxhighlight lang="lua">strTurnsLeft = Locale.ConvertTextKey( "TXT_KEY_STR_TURNS", city:GetBuildingProductionTurnsLeft( buildingID ));</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0700}}<syntaxhighlight lang="lua">Controls[controlTurns]:SetText( Locale.ConvertTextKey("TXT_KEY_PRODUCTION_HELP_NUM_TURNS", city:GetBuildingProductionTurnsLeft(queuedData1, i-1)) );</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetBuildingProductionTurnsLeft]]
[[Category:Civ5 City Production API|GetBuildingProductionTurnsLeft]]
[[Category:Civ5 Buildings API|GetBuildingProductionTurnsLeft]]