{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|City}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''int''' City:GetNumSpecialistsInBuilding<b>(</b>{{Type5|BuildingType}} index<b>)</b></code>


'''Returned Value'''
:No description available.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|index:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|CityView.lua}}
:<code>UI/InGame/CityView/CityView.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0349}}<syntaxhighlight lang="lua">iNumAssignedSpecialists = pCity:GetNumSpecialistsInBuilding(buildingID)</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0351}}<syntaxhighlight lang="lua">if specialistTable[buildingID] == nil then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|2054}}<syntaxhighlight lang="lua">local iNumSpecialistsAssigned = pCity:GetNumSpecialistsInBuilding(iBuilding);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetNumSpecialistsInBuilding]]
[[Category:Civ5 Buildings API|GetNumSpecialistsInBuilding]]
[[Category:Civ5 Specialists API|GetNumSpecialistsInBuilding]]