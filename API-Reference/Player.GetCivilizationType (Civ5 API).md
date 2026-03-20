{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Player}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>{{Type5|CivilizationType}} Player:GetCivilizationType<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|ChangePassword.lua}}
:<code>UI/InGame/ChangePassword.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0114}}<syntaxhighlight lang="lua">local civ = GameInfo.Civilizations[pPlayer:GetCivilizationType()];</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CityBannerManager.lua}}
:<code>UI/InGame/CityBannerManager.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0406}}<syntaxhighlight lang="lua">local civType = player:GetCivilizationType();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0433}}<syntaxhighlight lang="lua">civType = pOriginalOwner:GetCivilizationType();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CityStateDiploPopup.lua}}
:<code>UI/InGame/Popups/CityStateDiploPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0091}}<syntaxhighlight lang="lua">civType = pPlayer:GetCivilizationType();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ConfirmGiftPopup.lua}}
:<code>UI/InGame/PopupsGeneric/ConfirmGiftPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0023}}<syntaxhighlight lang="lua">strCivName = Locale.ConvertTextKey(GameInfo.Civilizations[pGiftedPlayer:GetCivilizationType()].ShortDescription);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DiploCurrentDeals.lua}}
:<code>UI/InGame/Popups/DiploCurrentDeals.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0093}}<syntaxhighlight lang="lua">local civName = Locale.ConvertTextKey( GameInfo.Civilizations[ pOtherPlayer:GetCivilizationType() ].ShortDescription );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DiploGlobalRelationships.lua}}
:<code>UI/InGame/Popups/DiploGlobalRelationships.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0049}}<syntaxhighlight lang="lua">local civType = pOtherPlayer:GetCivilizationType();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DiploList.lua}}
:<code>UI/InGame/DiploList.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0204}}<syntaxhighlight lang="lua">local myCivType = g_pPlayer:GetCivilizationType();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0459}}<syntaxhighlight lang="lua">civType = pOtherPlayer:GetCivilizationType();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DiscussionDialog.lua}}
:<code>UI/InGame/LeaderHead/DiscussionDialog.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0052}}<syntaxhighlight lang="lua">local themCivType = pAIPlayer:GetCivilizationType();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|EspionageOverview.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/Popups/EspionageOverview.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0954}}<syntaxhighlight lang="lua">local civilization = GameInfo.Civilizations[pActivePlayer:GetCivilizationType()];</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1444}}<syntaxhighlight lang="lua">local dpCivType = pPlayer:GetCivilizationType();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|Europe_Scenario.lua (G&K)}}
:<code>DLC/Expansion/Scenarios/MedievalScenario/Europe_Scenario.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0031}}<syntaxhighlight lang="lua">local playerCiv = player:GetCivilizationType();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|GameMenu.lua}}
:<code>UI/InGame/Menus/GameMenu.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0205}}<syntaxhighlight lang="lua">local myCivType = pPlayer:GetCivilizationType();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|GameplayUtilities.lua}}
:<code>Gameplay/Lua/GameplayUtilities.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0015}}<syntaxhighlight lang="lua">local civID = player:GetCivilizationType();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ProductionPopup.lua}}
:<code>UI/InGame/Popups/ProductionPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0252}}<syntaxhighlight lang="lua">local ourCiv = player:GetCivilizationType();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ReligionOverview.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/Popups/ReligionOverview.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0355}}<syntaxhighlight lang="lua">local civ = GameInfo.Civilizations[player:GetCivilizationType()];</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ReligionOverview.lua (G&K)}}
:<code>DLC/Expansion/Scenarios/MedievalScenario/ReligionOverview.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0142}}<syntaxhighlight lang="lua">local civType = pPlayer:GetCivilizationType();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ReplayViewer.lua}}
:<code>UI/InGame/Popups/ReplayViewer.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1283}}<syntaxhighlight lang="lua">Civilization = GameInfo.Civilizations[player:GetCivilizationType()].Type,</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ReturnCivilianPopup.lua}}
:<code>UI/InGame/PopupsGeneric/ReturnCivilianPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0027}}<syntaxhighlight lang="lua">local iNewUnit = pUnit:GetCaptureUnitType(pGiftingPlayer:GetCivilizationType());</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TechAwardPopup.lua}}
:<code>UI/InGame/Popups/TechAwardPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0014}}<syntaxhighlight lang="lua">local civType = GameInfo.Civilizations[player:GetCivilizationType()].Type;</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0146}}<syntaxhighlight lang="lua">civType = GameInfo.Civilizations[player:GetCivilizationType()].Type;</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TradeLogic.lua}}
:<code>UI/InGame/WorldView/TradeLogic.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0957}}<syntaxhighlight lang="lua">local themCivType = g_pThem:GetCivilizationType();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0987}}<syntaxhighlight lang="lua">Controls.ThemCiv:SetText( "(" .. Locale.ConvertTextKey( GameInfo.Civilizations[ g_pThem:GetCivilizationType() ].ShortDescription ) .. ")" );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|2778}}<syntaxhighlight lang="lua">szName = szName .. " (" .. Locale.ConvertTextKey(GameInfo.Civilizations[Players[iLoopPlayer]:GetCivilizationType()].ShortDescription) .. ")";</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TurnsRemaining.lua (G&K)}}
:<code>DLC/Expansion/Scenarios/MedievalScenario/TurnsRemaining.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0345}}<syntaxhighlight lang="lua">local civType = Players[iNewAlly]:GetCivilizationType();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1093}}<syntaxhighlight lang="lua">if (pPlayer:GetCivilizationType() == GameInfoTypes["CIVILIZATION_RUSSIA"]) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1101}}<syntaxhighlight lang="lua">if (pPlayer:GetCivilizationType() == GameInfoTypes["CIVILIZATION_ARABIA"]) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1107}}<syntaxhighlight lang="lua">if (pPlayer:GetCivilizationType() == GameInfoTypes["CIVILIZATION_SONGHAI"]) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|VictoryProgress.lua}}
:<code>UI/InGame/Popups/VictoryProgress.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0454}}<syntaxhighlight lang="lua">local myCivType = leadAI:GetCivilizationType();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|VoteResultsPopup.lua}}
:<code>UI/InGame/Popups/VoteResultsPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0145}}<syntaxhighlight lang="lua">local civType = pVoteCastPlayer:GetCivilizationType();</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetCivilizationType]]
[[Category:Civ5 Players API|GetCivilizationType]]