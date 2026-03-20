{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Events}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''void''' Events.SerialEventCitySetDamage<b>(</b>{{Type5|PlayerID}} player, {{Type5|CityID}} cityID, '''int''' damage, '''int''' previousDamage<b>)</b></code>


'''Event Type'''
:Regular event: you can subscribe to it through <code>Events.SerialEventCitySetDamage.Add(''<function handler>'')</code> or invoke it directly through <code>Events.SerialEventCitySetDamage(''<arguments list>'')</code>.

'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|player:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|cityID:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|damage:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|previousDamage:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|CityBannerManager.lua}}
:<code>UI/InGame/CityBannerManager.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0900}}<syntaxhighlight lang="lua">Events.SerialEventCitySetDamage.Add(OnCitySetDamage);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CityList.lua}}
:<code>UI/InGame/CityList.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0070}}<syntaxhighlight lang="lua">Events.SerialEventCitySetDamage.Add( OnChangeEvent );</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|SerialEventCitySetDamage]]
[[Category:Civ5 Cities API|SerialEventCitySetDamage]]
[[Category:Civ5 Combat API|SerialEventCitySetDamage]]