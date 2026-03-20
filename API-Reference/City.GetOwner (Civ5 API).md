{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|City}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>{{Type5|PlayerID}} City:GetOwner<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|CityBannerManager.lua}}
:<code>UI/InGame/CityBannerManager.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0031}}<syntaxhighlight lang="lua">if (city:GetOwner() ~= Game.GetActivePlayer()) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CityView.lua}}
:<code>UI/InGame/CityView/CityView.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0070}}<syntaxhighlight lang="lua">if pCity:GetOwner() ~= Game.GetActivePlayer() then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0645}}<syntaxhighlight lang="lua">local pPlayer = Players[pCity:GetOwner()];</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1726}}<syntaxhighlight lang="lua">if ( plot:GetOwner() == pCity:GetOwner() ) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1793}}<syntaxhighlight lang="lua">elseif ( plot:IsVisibleEnemyUnit(pCity:GetOwner()) ) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CityView.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/CityView/CityView.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1493}}<syntaxhighlight lang="lua">if (pCity:GetOwner() ~= Game.GetActivePlayer()) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|EnemyUnitPanel.lua}}
:<code>UI/InGame/WorldView/EnemyUnitPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1457}}<syntaxhighlight lang="lua">local myPlayerID = myCity:GetOwner();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|InfoTooltipInclude.lua}}
:<code>UI/InGame/InfoTooltipInclude.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0562}}<syntaxhighlight lang="lua">local iAmount = Players[pCity:GetOwner()]:GetCultureCityModifier();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0577}}<syntaxhighlight lang="lua">iAmount = Players[pCity:GetOwner()]:GetCultureWonderMultiplier();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ProductionPopup.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/Popups/ProductionPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0135}}<syntaxhighlight lang="lua">local player = city:GetOwner();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TurnsRemaining.lua (G&K)}}
:<code>DLC/Expansion/Scenarios/MedievalScenario/TurnsRemaining.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0213}}<syntaxhighlight lang="lua">Game.SetFounder(GameInfoTypes["RELIGION_ORTHODOXY"], pNewHolyCity:GetOwner());</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0506}}<syntaxhighlight lang="lua">if (pHolyCity:GetOwner() == ePlayer) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0510}}<syntaxhighlight lang="lua">local eOwner = pHolyCity:GetOwner();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1471}}<syntaxhighlight lang="lua">local iPlayer = pBestCity:GetOwner();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1561}}<syntaxhighlight lang="lua">if (pCity:GetOwner() < 12) then</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetOwner]]
[[Category:Civ5 Terrain Ownership API|GetOwner]]