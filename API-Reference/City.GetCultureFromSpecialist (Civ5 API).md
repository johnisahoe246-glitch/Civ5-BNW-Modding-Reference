{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|City}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''int''' City:GetCultureFromSpecialist<b>(</b>{{Type5|SpecialistType}} specialist<b>)</b></code>


'''Returned Value'''
:No description available.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|specialist:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|CityView.lua}}
:<code>UI/InGame/CityView/CityView.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1059}}<syntaxhighlight lang="lua">local iCultureFromSpecialist = pCity:GetCultureFromSpecialist(iSpecialistID);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetCultureFromSpecialist]]
[[Category:Civ5 Culture API|GetCultureFromSpecialist]]
[[Category:Civ5 Specialists API|GetCultureFromSpecialist]]