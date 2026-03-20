{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|City}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''void''' City:ChooseProduction<b>(</b>{{Type5|UnitType}} trainUnit, {{Type5|BuildingType}} constructBuilding, {{Type5|ProjectType}} createProject, '''bool''' finish, '''bool''' front<b>)</b></code>


'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|trainUnit:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|constructBuilding:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|createProject:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|finish:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|front:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|PuppetCityPopup.lua}}
:<code>UI/InGame/PopupsGeneric/PuppetCityPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0057}}<syntaxhighlight lang="lua">newCity:ChooseProduction();</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|ChooseProduction]]
[[Category:Civ5 City Production API|ChooseProduction]]