{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|City}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''string''' City:GetName<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|CityBannerManager.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/CityBannerManager.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0286}}<syntaxhighlight lang="lua">controls.SpyIcon:LocalizeAndSetToolTip("TXT_KEY_CITY_SPY_YOUR_CITY_TT", strSpyRank, strSpyName, city:GetName(), strSpyRank, strSpyName);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0288}}<syntaxhighlight lang="lua">controls.SpyIcon:LocalizeAndSetToolTip("TXT_KEY_CITY_SPY_CITY_STATE_TT", strSpyRank, strSpyName, city:GetName(), strSpyRank, strSpyName);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0290}}<syntaxhighlight lang="lua">controls.SpyIcon:LocalizeAndSetToolTip("TXT_KEY_CITY_SPY_OTHER_CIV_TT", strSpyRank, strSpyName, city:GetName(), strSpyRank, strSpyName, strSpyRank, strSpyName);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CityList.lua}}
:<code>UI/InGame/CityList.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0129}}<syntaxhighlight lang="lua">sortEntry.CityName = pCity:GetName();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|EconomicGeneralInfo.lua}}
:<code>UI/InGame/Popups/EconomicGeneralInfo.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0211}}<syntaxhighlight lang="lua">instance.CityName:SetText( pCity:GetName() );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ProductionPopup.lua}}
:<code>UI/InGame/Popups/ProductionPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0204}}<syntaxhighlight lang="lua">Controls.CityName:SetText( city:GetName() );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ReligionOverview.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/Popups/ReligionOverview.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0498}}<syntaxhighlight lang="lua">local holyCityName = holyCity:GetName();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TurnsRemaining.lua - DLC_02 DLC}}
:<code>DLC/DLC_02/Scenarios/NewWorldScenario/TurnsRemaining.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0222}}<syntaxhighlight lang="lua">text = Locale.ConvertTextKey("TXT_KEY_NEWWORLD_SCENARIO_TREASURE_RETURNED", capital:GetName(), iGoldReceived, iVPReceived);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TurnsRemaining.lua (G&K)}}
:<code>DLC/Expansion/Scenarios/MedievalScenario/TurnsRemaining.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0209}}<syntaxhighlight lang="lua">popupInfo.Text = Locale.ConvertTextKey("TXT_KEY_MEDIEVAL_SCENARIO_NO_ORTHODOX_CITIES", pOrthodoxHolyCity:GetName(), pOrthodoxHolyCity:GetName());</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0214}}<syntaxhighlight lang="lua">popupInfo.Text = Locale.ConvertTextKey("TXT_KEY_MEDIEVAL_SCENARIO_NEW_ORTHODOX_HOLY_CITY", pOrthodoxHolyCity:GetName(), pNewHolyCity:GetName());</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0771}}<syntaxhighlight lang="lua">popupInfo.Text = Locale.ConvertTextKey("TXT_KEY_MEDIEVAL_SCENARIO_YOU_ADOPTED_PROTESTANTISM", pProtestantHolyCity:GetName());</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1489}}<syntaxhighlight lang="lua">popupInfo.Text = Locale.ConvertTextKey("TXT_KEY_MEDIEVAL_SCENARIO_FIRST_REFORMER", pBestCity:GetName());</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1508}}<syntaxhighlight lang="lua">popupInfo.Text = Locale.ConvertTextKey("TXT_KEY_MEDIEVAL_SCENARIO_SECOND_REFORMER", pBestCity:GetName());</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1525}}<syntaxhighlight lang="lua">popupInfo.Text = Locale.ConvertTextKey("TXT_KEY_MEDIEVAL_SCENARIO_THIRD_REFORMER", pBestCity:GetName());</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|UnitPanel.lua}}
:<code>UI/InGame/WorldView/UnitPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0476}}<syntaxhighlight lang="lua">local name = city:GetName();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|VictoryStatus.lua (G&K)}}
:<code>DLC/Expansion/Scenarios/SteampunkScenario/VictoryStatus.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0179}}<syntaxhighlight lang="lua">sYourBestCity = pYourBestCity:GetName();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0196}}<syntaxhighlight lang="lua">sWorldBestCity = pCity:GetName();</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetName]]