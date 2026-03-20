{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Player}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''int''' Player:CountNumBuildings<b>(</b>{{Type5|BuildingType}} building<b>)</b></code>


'''Returned Value'''
:No description available.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|building:
|valign="top"| ''No description available.''
|}


=Source code samples=
{{PseudoH4|DiploGlobalRelationships.lua}}
:<code>UI/InGame/Popups/DiploGlobalRelationships.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0108}}<syntaxhighlight lang="lua">if (pOtherPlayer:CountNumBuildings(iBuilding) > 0) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TurnsRemaining.lua - DLC_04 DLC}}
:<code>DLC/DLC_04/Scenarios/1066Scenario/TurnsRemaining.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0047}}<syntaxhighlight lang="lua">local shireCourtText = Locale.ConvertTextKey("TXT_KEY_1066_SCENARIO_SHIRE_COURT_STATUS", Players[iLondonPlayer]:CountNumBuildings(GameInfo.Buildings["BUILDING_COURTHOUSE"].ID));</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|CountNumBuildings]]
[[Category:Civ5 Buildings API|CountNumBuildings]]