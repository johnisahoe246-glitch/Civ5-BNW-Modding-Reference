{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Player}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''bool''' Player:IsMinorPermanentWar<b>(</b>{{Type5|TeamID}} activeTeam<b>)</b></code>


'''Returned Value'''
:No description available.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|activeTeam:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|CityBannerManager.lua}}
:<code>UI/InGame/CityBannerManager.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0482}}<syntaxhighlight lang="lua">elseif (player:IsMinorPermanentWar(iActiveTeam)) then      -- Permanent War</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CityStateStatusHelper.lua (G&K)}}
:<code>DLC/Expansion/UI/CityStateStatusHelper.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0180}}<syntaxhighlight lang="lua">elseif (pMinor:IsMinorPermanentWar(iActiveTeam)) then      -- Permanent War</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|InfoTooltipInclude.lua}}
:<code>UI/InGame/InfoTooltipInclude.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0356}}<syntaxhighlight lang="lua">elseif (pPlayer:IsMinorPermanentWar(iActiveTeam)) then      -- Permanent War</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TradeLogic.lua}}
:<code>UI/InGame/WorldView/TradeLogic.lua</code>
:{{CodeBegin5}}
{{CodeLine5|2584}}<syntaxhighlight lang="lua">if (pLoopPlayer:IsMinorPermanentWar(iFromPlayer)) then</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|IsMinorPermanentWar]]
[[Category:Civ5 Diplomacy API|IsMinorPermanentWar]]
[[Category:Civ5 City States API|IsMinorPermanentWar]]