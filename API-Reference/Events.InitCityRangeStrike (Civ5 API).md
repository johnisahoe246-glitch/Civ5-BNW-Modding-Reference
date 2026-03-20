{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Events}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''void''' Events.InitCityRangeStrike<b>(</b>{{Type5|PlayerID}} Player, {{Type5|CityID}} CityID<b>)</b></code>


'''Event Type'''
:Regular event: you can subscribe to it through <code>Events.InitCityRangeStrike.Add(''<function handler>'')</code> or invoke it directly through <code>Events.InitCityRangeStrike(''<arguments list>'')</code>.

'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|Player:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|CityID:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|CityBannerManager.lua}}
:<code>UI/InGame/CityBannerManager.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1006}}<syntaxhighlight lang="lua">Events.InitCityRangeStrike( PlayerID, CityID );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1033}}<syntaxhighlight lang="lua">Events.InitCityRangeStrike.Add( OnInitCityRangeStrike );</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|InitCityRangeStrike]]
[[Category:Civ5 Cities API|InitCityRangeStrike]]
[[Category:Civ5 Combat API|InitCityRangeStrike]]