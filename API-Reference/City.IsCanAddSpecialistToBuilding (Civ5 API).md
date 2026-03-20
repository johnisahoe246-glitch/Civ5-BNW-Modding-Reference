{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|City}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''bool''' City:IsCanAddSpecialistToBuilding<b>(</b>{{Type5|BuildingType}} building<b>)</b></code>


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

{{PseudoH4|CityView.lua}}
:<code>UI/InGame/CityView/CityView.lua</code>
:{{CodeBegin5}}
{{CodeLine5|2042}}<syntaxhighlight lang="lua">if (pCity:IsCanAddSpecialistToBuilding(iBuilding)) then</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|IsCanAddSpecialistToBuilding]]
[[Category:Civ5 Buildings API|IsCanAddSpecialistToBuilding]]
[[Category:Civ5 Specialists API|IsCanAddSpecialistToBuilding]]