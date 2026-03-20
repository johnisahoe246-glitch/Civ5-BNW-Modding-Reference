{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Events}}.<br/>
This is a static method, invoke it with a dot.
}}


This event is triggered when a city is created.


=Usage=
<code>'''void''' Events.SerialEventCityCreated<b>(</b>{{Type5|Vector2}} vHexPos, {{Type5|PlayerID}} player, {{Type5|CityID}} cityID, {{Type5|ArtStyleType}} artStyleType, {{Type5|EraType}} eraType, '''int''' continent, '''int''' populationSize, '''int''' size, '''int''' fogState<b>)</b></code>


'''Event Type'''
:Regular event: you can subscribe to it through <code>Events.SerialEventCityCreated.Add(''<function handler>'')</code> or invoke it directly through <code>Events.SerialEventCityCreated(''<arguments list>'')</code>.

'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|vHexPos:
|valign="top"| ''Vector3 containing city x,y,z coordinates which can be converted to map coordinates with the {{Type5|ToGridFromHex}} function <br />e.g. '''local iX, iY = ToGridFromHex( vHexPos.x, vHexPos.y )''
|-
|valign="top" style="padding-right:6px;"|player:
|valign="top"| ''ID of the player who owns the created city; index into global Players table''
|-
|valign="top" style="padding-right:6px;"|cityID:
|valign="top"| ''ID of the city that was created; note IDs are specific to player and not truly unique''
|-
|valign="top" style="padding-right:6px;"|artStyleType:
|valign="top"| ''art style of city graphics; compare with types from ''ArtStyleTypes'' table (e.g. '''GameInfoTypes.ARTSTYLE_ASIAN''')''
|-
|valign="top" style="padding-right:6px;"|eraType:
|valign="top"| ''era of city graphics; compare with types from ''Eras'' table (e.g. '''GameInfoTypes.ERA_ANCIENT''')''
|-
|valign="top" style="padding-right:6px;"|continent:
|valign="top"| ''ID of continent where city is located''
|-
|valign="top" style="padding-right:6px;"|populationSize:
|valign="top"| ''unknown; name based on reference in original game files ({{Type5|UnitFlagManager.lua}} and {{Type5|CityBannerManager.lua}})''
|-
|valign="top" style="padding-right:6px;"|size:
|valign="top"| ''unknown; name based on reference in original game files ({{Type5|UnitFlagManager.lua}} and {{Type5|CityBannerManager.lua}})''
|-
|valign="top" style="padding-right:6px;"|fogState:
|valign="top"| ''visibility of this city for Active Player
: 0 = tile completely hidden by FoW
: 1 = tile revealed but not currently in vision
: 2 = tile in vision''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|CityBannerManager.lua}}
:<code>UI/InGame/CityBannerManager.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0650}}<syntaxhighlight lang="lua">Events.SerialEventCityCreated.Add( OnCityCreated );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CityList.lua}}
:<code>UI/InGame/CityList.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0073}}<syntaxhighlight lang="lua">Events.SerialEventCityCreated.Add( OnChangeEvent );</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|SerialEventCityCreated]]
[[Category:Civ5 Cities API|SerialEventCityCreated]]