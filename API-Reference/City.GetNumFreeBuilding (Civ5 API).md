{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|City}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''int''' City:GetNumFreeBuilding<b>(</b>{{Type5|BuildingType}} index<b>)</b></code>


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
{{CodeLine5|0298}}<syntaxhighlight lang="lua">if (pCity:GetNumFreeBuilding(buildingID) > 0) then</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetNumFreeBuilding]]
[[Category:Civ5 Buildings API|GetNumFreeBuilding]]