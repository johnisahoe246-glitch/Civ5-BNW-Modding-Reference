{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Player}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''bool''' Player:IsAllies<b>(</b>{{Type5|PlayerID}} major<b>)</b></code>


'''Returned Value'''
:No description available.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|major:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|CityBannerManager.lua}}
:<code>UI/InGame/CityBannerManager.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0474}}<syntaxhighlight lang="lua">if (player:IsAllies(iActivePlayer)) then      -- Allies</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CityStateDiploPopup.lua}}
:<code>UI/InGame/Popups/CityStateDiploPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0072}}<syntaxhighlight lang="lua">local bAllies = pPlayer:IsAllies(iActivePlayer);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CityStateStatusHelper.lua (G&K)}}
:<code>DLC/Expansion/UI/CityStateStatusHelper.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0062}}<syntaxhighlight lang="lua">local bAllies = pMinor:IsAllies(iMajor);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0172}}<syntaxhighlight lang="lua">if (pMinor:IsAllies(iMajor)) then      -- Allies</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0378}}<syntaxhighlight lang="lua">if (pMinor:IsAllies(iMajor)) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DiploGlobalRelationships.lua}}
:<code>UI/InGame/Popups/DiploGlobalRelationships.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0262}}<syntaxhighlight lang="lua">if (pThirdPlayer:IsAllies(iOtherPlayer)) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DiploRelationships.lua}}
:<code>UI/InGame/Popups/DiploRelationships.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0381}}<syntaxhighlight lang="lua">if (pPlayer:IsAllies(iActivePlayer)) then      -- Allies</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|InfoTooltipInclude.lua}}
:<code>UI/InGame/InfoTooltipInclude.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0338}}<syntaxhighlight lang="lua">if (pPlayer:IsAllies(iForPlayer)) then      -- Allies</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TurnsRemaining.lua (G&K)}}
:<code>DLC/Expansion/Scenarios/MedievalScenario/TurnsRemaining.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0492}}<syntaxhighlight lang="lua">if (Players[eOwner]:IsAllies(ePlayer)) then</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|IsAllies]]