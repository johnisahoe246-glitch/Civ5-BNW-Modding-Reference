{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a global function. Use: <code>include("InfoTooltipInclude.lua")</code>
}}


=Usage=
<code>'''string''' GetCityStateStatus<b>(</b>{{Type5|Player}} player, {{Type5|PlayerID}} forPlayer, '''int''' war<b>)</b></code>


'''Returned Value'''
:No description available.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|player:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|forPlayer:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|war:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|CityBannerManager.lua}}
:<code>UI/InGame/CityBannerManager.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0503}}<syntaxhighlight lang="lua">local strStatusTT = GetCityStateStatus(player, iActivePlayer, bWar);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CityStateDiploPopup.lua}}
:<code>UI/InGame/Popups/CityStateDiploPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0137}}<syntaxhighlight lang="lua">local strStatusTT = GetCityStateStatus(pPlayer, iActivePlayer, bWar);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DiploList.lua}}
:<code>UI/InGame/DiploList.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0470}}<syntaxhighlight lang="lua">local strStatusTT = GetCityStateStatus(pOtherPlayer, Game.GetActivePlayer(), bWar);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetCityStateStatus]]
[[Category:Civ5 Cities API|GetCityStateStatus]]