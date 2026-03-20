{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|City}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''int''' City:GetSpecialistCount<b>(</b>{{Type5|SpecialistType}} index<b>)</b></code>


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
{{CodeLine5|0924}}<syntaxhighlight lang="lua">local numSlackersInThisCity = pCity:GetSpecialistCount( slackerType );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0988}}<syntaxhighlight lang="lua">local iCount = pCity:GetSpecialistCount( pSpecialistInfo.ID );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|GPList.lua}}
:<code>UI/InGame/GPList.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0225}}<syntaxhighlight lang="lua">local iCount = city:GetSpecialistCount( specialistInfo.ID );</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetSpecialistCount]]
[[Category:Civ5 Specialists API|GetSpecialistCount]]