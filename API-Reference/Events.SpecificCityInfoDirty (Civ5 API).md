{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Events}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''void''' Events.SpecificCityInfoDirty<b>(</b>{{Type5|PlayerID}} player, {{Type5|CityID}} cityID, {{Type5|CityUpdateType}} updateType<b>)</b></code>


'''Event Type'''
:Regular event: you can subscribe to it through <code>Events.SpecificCityInfoDirty.Add(''<function handler>'')</code> or invoke it directly through <code>Events.SpecificCityInfoDirty(''<arguments list>'')</code>.

'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|player:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|cityID:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|updateType:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|CityBannerManager.lua}}
:<code>UI/InGame/CityBannerManager.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0931}}<syntaxhighlight lang="lua">Events.SpecificCityInfoDirty.Add(OnSpecificCityInfoDirty);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CityList.lua}}
:<code>UI/InGame/CityList.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0074}}<syntaxhighlight lang="lua">Events.SpecificCityInfoDirty.Add( OnChangeEvent );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ProductionPopup.lua}}
:<code>UI/InGame/Popups/ProductionPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0084}}<syntaxhighlight lang="lua">Events.SpecificCityInfoDirty( player, cityID, CityUpdateTypes.CITY_UPDATE_TYPE_BANNER);</syntaxhighlight>
{{CodeLine5|0085}}<syntaxhighlight lang="lua">Events.SpecificCityInfoDirty( player, cityID, CityUpdateTypes.CITY_UPDATE_TYPE_PRODUCTION);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|WorldView.lua}}
:<code>UI/InGame/WorldView/WorldView.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0490}}<syntaxhighlight lang="lua">Events.SpecificCityInfoDirty( activePlayerID, pHeadSelectedCity:GetID(), CityUpdateTypes.CITY_UPDATE_TYPE_BANNER);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|SpecificCityInfoDirty]]
[[Category:Civ5 Cities API|SpecificCityInfoDirty]]