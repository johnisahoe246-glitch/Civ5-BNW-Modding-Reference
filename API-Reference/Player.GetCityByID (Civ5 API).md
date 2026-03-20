{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Player}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>{{Type5|City}} Player:GetCityByID<b>(</b>{{Type5|CityID}} city<b>)</b></code>


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

{{PseudoH4|AnnexCityPopup.lua}}
:<code>UI/InGame/PopupsGeneric/AnnexCityPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0008}}<syntaxhighlight lang="lua">local newCity      = activePlayer:GetCityByID(cityID);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CityBannerManager.lua}}
:<code>UI/InGame/CityBannerManager.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0098}}<syntaxhighlight lang="lua">local city = player:GetCityByID(cityBanner.cityID);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0990}}<syntaxhighlight lang="lua">local city = player:GetCityByID(CityID);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1183}}<syntaxhighlight lang="lua">local city = activePlayer:GetCityByID(cityID);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1249}}<syntaxhighlight lang="lua">local city = player:GetCityByID( cityIndex );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CityBannerManager.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/CityBannerManager.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0870}}<syntaxhighlight lang="lua">local city = Players[iPlayerID]:GetCityByID(iCityID);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|EspionageOverview.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/Popups/EspionageOverview.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0794}}<syntaxhighlight lang="lua">local pCity = pPlayer:GetCityByID(cityInfo.CityID);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|GreatPersonRewardPopup.lua}}
:<code>UI/InGame/Popups/GreatPersonRewardPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0022}}<syntaxhighlight lang="lua">local pCity = Players[iPlayer]:GetCityByID(iCityID);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|LiberateMinorPopup.lua}}
:<code>UI/InGame/PopupsGeneric/LiberateMinorPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0009}}<syntaxhighlight lang="lua">local pNewCity         = pActivePlayer:GetCityByID(iCityID);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ProductionPopup.lua}}
:<code>UI/InGame/Popups/ProductionPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0758}}<syntaxhighlight lang="lua">local city = player:GetCityByID( popupInfo.Data1 );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TurnsRemaining.lua - DLC_04 DLC}}
:<code>DLC/DLC_04/Scenarios/1066Scenario/TurnsRemaining.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0103}}<syntaxhighlight lang="lua">local pCity = pPlayer:GetCityByID(iCity);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TurnsRemaining.lua (G&K)}}
:<code>DLC/Expansion/Scenarios/MedievalScenario/TurnsRemaining.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0316}}<syntaxhighlight lang="lua">local pCity = pPlayer:GetCityByID(cityIndex);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TurnsRemaining.lua (G&K)}}
:<code>DLC/Expansion/Scenarios/SteampunkScenario/TurnsRemaining.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0235}}<syntaxhighlight lang="lua">local pCity = pPlayer:GetCityByID(iCityID);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|VictoryStatus.lua (G&K)}}
:<code>DLC/Expansion/Scenarios/SteampunkScenario/VictoryStatus.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0177}}<syntaxhighlight lang="lua">local pYourBestCity = pForPlayer:GetCityByID(iYourBestCityID);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0190}}<syntaxhighlight lang="lua">local pCity = Players[iPlayerLoop]:GetCityByID(iBestCityID);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetCityByID]]
[[Category:Civ5 Cities API|GetCityByID]]