{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|City}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''int''' City:GetSpecialistGreatPersonProgress<b>(</b>{{Type5|SpecialistType}} index<b>)</b></code>


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
{{CodeLine5|0971}}<syntaxhighlight lang="lua">local iProgress = pCity:GetSpecialistGreatPersonProgress(iSpecialistIndex);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|GPList.lua}}
:<code>UI/InGame/GPList.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0106}}<syntaxhighlight lang="lua">iProgress = pCity:GetSpecialistGreatPersonProgress(iSpecialistIndex);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0214}}<syntaxhighlight lang="lua">local iProgress = city:GetSpecialistGreatPersonProgress(iSpecialistIndex);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetSpecialistGreatPersonProgress]]
[[Category:Civ5 Specialists API|GetSpecialistGreatPersonProgress]]