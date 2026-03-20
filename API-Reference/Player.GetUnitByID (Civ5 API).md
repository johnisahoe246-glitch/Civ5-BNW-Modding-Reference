{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Player}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>{{Type5|Unit}} Player:GetUnitByID<b>(</b>{{Type5|UnitID}} unit<b>)</b></code>


'''Returned Value'''
:{{Type5|Unit}} object
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|unit:
|valign="top"| ''unit ID''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|BarbarianRansomPopup.lua}}
:<code>UI/InGame/PopupsGeneric/BarbarianRansomPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0008}}<syntaxhighlight lang="lua">local pUnit = pPlayer:GetUnitByID(iUnitID);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CityBannerManager.lua}}
:<code>UI/InGame/CityBannerManager.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1142}}<syntaxhighlight lang="lua">local unit = player:GetUnitByID( unitID );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ConfirmGiftPopup.lua}}
:<code>UI/InGame/PopupsGeneric/ConfirmGiftPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0017}}<syntaxhighlight lang="lua">pUnit = pGiftingPlayer:GetUnitByID(iUnitIndex);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TurnsRemaining.lua - DLC_02 DLC}}
:<code>DLC/DLC_02/Scenarios/NewWorldScenario/TurnsRemaining.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0134}}<syntaxhighlight lang="lua">local unit = player:GetUnitByID(iUnitID);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TurnsRemaining.lua (G&K)}}
:<code>DLC/Expansion/Scenarios/FallOfRomeScenario/TurnsRemaining.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1023}}<syntaxhighlight lang="lua">pUnit = Players[iPlayer]:GetUnitByID(iUnitID);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|UnitFlagManager.lua}}
:<code>UI/InGame/UnitFlagManager.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0078}}<syntaxhighlight lang="lua">local pUnit = Players[ playerID ]:GetUnitByID( unitID );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0306}}<syntaxhighlight lang="lua">local unit = Players[ self.m_PlayerID ]:GetUnitByID( self.m_UnitID );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0372}}<syntaxhighlight lang="lua">local pUnit = Players[ self.m_PlayerID ]:GetUnitByID( self.m_UnitID );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0884}}<syntaxhighlight lang="lua">Players[ playerID ]:GetUnitByID( unitID ) == nil or</syntaxhighlight>
{{CodeLine5|0885}}<syntaxhighlight lang="lua">Players[ playerID ]:GetUnitByID( unitID ):IsDead() )</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0973}}<syntaxhighlight lang="lua">local thisUnit = Players[ playerID ]:GetUnitByID( unitID );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1578}}<syntaxhighlight lang="lua">local pUnit = pPlayer:GetUnitByID( unitID );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|UnitMemberOverlay.lua}}
:<code>UI/InGame/UnitMemberOverlay.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0251}}<syntaxhighlight lang="lua">local unit = playerUnitList:GetUnitByID( unitID );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0539}}<syntaxhighlight lang="lua">local unit = playersUnitList:GetUnitByID( unitID );</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetUnitByID]]
[[Category:Civ5 Units API|GetUnitByID]]