{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Player}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''int''' Player:IsCapitalConnectedToCity<b>(</b>{{Type5|City}} city<b>)</b></code>


'''Returned Value'''
:No description available.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|city:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|CityBannerManager.lua}}
:<code>UI/InGame/CityBannerManager.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0165}}<syntaxhighlight lang="lua">if (not city:IsCapital() and player:IsCapitalConnectedToCity(city) and not city:IsBlockaded()) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CityView.lua}}
:<code>UI/InGame/CityView/CityView.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0654}}<syntaxhighlight lang="lua">if (not isCapital and pPlayer:IsCapitalConnectedToCity(pCity) and not pCity:IsBlockaded()) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|EconomicGeneralInfo.lua}}
:<code>UI/InGame/Popups/EconomicGeneralInfo.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0248}}<syntaxhighlight lang="lua">if( pPlayer:IsCapitalConnectedToCity( pCity ) ) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|HappinessInfo.lua}}
:<code>UI/InGame/Popups/HappinessInfo.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0306}}<syntaxhighlight lang="lua">if (pPlayer:IsCapitalConnectedToCity(pCity)) then</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|IsCapitalConnectedToCity]]
[[Category:Civ5 Cities API|IsCapitalConnectedToCity]]