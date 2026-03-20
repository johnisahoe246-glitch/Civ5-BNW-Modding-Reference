{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Network}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''void''' Network.SendSetCityAvoidGrowth<b>(</b>{{Type5|CityID}} arg0, '''bool''' arg1<b>)</b></code>


'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|arg0:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|arg1:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|CityView.lua}}
:<code>UI/InGame/CityView/CityView.lua</code>
:{{CodeBegin5}}
{{CodeLine5|2294}}<syntaxhighlight lang="lua">Network.SendSetCityAvoidGrowth( pCity:GetID(), not pCity:IsForcedAvoidGrowth() );</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|SendSetCityAvoidGrowth]]
[[Category:Civ5 Cities API|SendSetCityAvoidGrowth]]
[[Category:Civ5 Food & Population API|SendSetCityAvoidGrowth]]