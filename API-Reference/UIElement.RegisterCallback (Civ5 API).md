{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This method is declared by '''ButtonBase''', {{Type5|EditBox}}, {{Type5|Grid}}, {{Type5|GridButton}}, {{Type5|Image}}, {{Type5|RadioButton}}, {{Type5|Stack}} and {{Type5|TextButton}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''void''' UIElement:RegisterCallback<b>(</b>{{Type5|MouseType}} OnSearchTextEnter, ('''void''' func<b>(</b>{{Type5|PolicyBranchType}} policyBranchIndex, {{Type5|UnitType}} y, {{Type5|Button}} button<b>)</b>) OnClose = nil<b>)</b></code>


'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|OnSearchTextEnter:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|OnClose:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Too many occurences. Only 50 out of 1542 are listed.''

{{PseudoH4|AdvancedSetup.lua}}
:<code>UI/FrontEnd/GameSetup/AdvancedSetup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1117}}<syntaxhighlight lang="lua">Controls.EditButton:RegisterCallback( Mouse.eLClick, function()</syntaxhighlight>
{{CodeLine5|1118}}<syntaxhighlight lang="lua">UIManager:PushModal(Controls.SetCivNames);</syntaxhighlight>
{{CodeLine5|1119}}<syntaxhighlight lang="lua">end);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|AdvisorInfoPopup.lua}}
:<code>UI/InGame/Popups/AdvisorInfoPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0190}}<syntaxhighlight lang="lua">Controls.Civilopedia_List:RegisterCallback( Mouse.eLClick, OnCivilopediaListClicked );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CityStateDiploPopup.lua}}
:<code>UI/InGame/Popups/CityStateDiploPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0577}}<syntaxhighlight lang="lua">Controls.UnitGiftButton:RegisterCallback( Mouse.eLClick, OnGiftUnit );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CityView.lua}}
:<code>UI/InGame/CityView/CityView.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0457}}<syntaxhighlight lang="lua">controlTable.BuildingFilledSpecialistSlot3:RegisterCallback( Mouse.eLClick, RemoveSpecialist );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0984}}<syntaxhighlight lang="lua">controlTable.GPImage:RegisterCallback( Mouse.eRClick, GetPedia );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1941}}<syntaxhighlight lang="lua">Controls.b3up:RegisterCallback( Mouse.eLClick, OnSwapClick );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CivilopediaScreen.lua}}
:<code>UI/Civilopedia/CivilopediaScreen.lua</code>
:{{CodeBegin5}}
{{CodeLine5|4705}}<syntaxhighlight lang="lua">thisEraInstance.ListHeadingButton:RegisterCallback( Mouse.eLClick, CivilopediaCategory[CategoryTech].SelectHeading );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|5188}}<syntaxhighlight lang="lua">thisListInstance.ListItemButton:RegisterCallback( Mouse.eLClick, CivilopediaCategory[CategoryCityStates].buttonClicked );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|5315}}<syntaxhighlight lang="lua">thisListInstance.ListItemButton:RegisterCallback( Mouse.eLClick, CivilopediaCategory[CategoryResources].buttonClicked );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|5574}}<syntaxhighlight lang="lua">thisUnitInstance.ListItemButton:RegisterCallback( Mouse.eLClick, CivilopediaCategory[CategoryUnits].SelectArticle );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|6409}}<syntaxhighlight lang="lua">Controls.OK:RegisterCallback(Mouse.eLClick, OnSearchNotFoundOK );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DebugMenu.lua}}
:<code>UI/InGame/DebugMenu.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0105}}<syntaxhighlight lang="lua">Controls.FluidFOWPanel_Button:RegisterCallback(Mouse.eLClick, ModeClicked );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0246}}<syntaxhighlight lang="lua">Controls.ParticleEffects_Button:RegisterCallback( Mouse.eLClick, ModeClicked );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DebugMode.lua}}
:<code>UI/InGame/DebugMode.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0067}}<syntaxhighlight lang="lua">Controls.CreateCity_Button:RegisterCallback( Mouse.eLClick, ModeClicked );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0079}}<syntaxhighlight lang="lua">Controls.AttackUnit_Button:RegisterCallback( Mouse.eLClick, ModeClicked );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0148}}<syntaxhighlight lang="lua">Controls.CityContinent_ButtonUp:RegisterCallback( Mouse.eLClick, ChangeCityContinent );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0379}}<syntaxhighlight lang="lua">Controls.BuildingEra_ButtonUp:RegisterCallback( Mouse.eLClick, ChangeCityAssetEra );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0640}}<syntaxhighlight lang="lua">Controls.UnitVariableValue_ButtonGrtDown:RegisterCallback( Mouse.eLClick, ModUnitVariableValue );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DiploCurrentDeals.lua}}
:<code>UI/InGame/Popups/DiploCurrentDeals.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0131}}<syntaxhighlight lang="lua">Controls.HistoricDealsButton:RegisterCallback( Mouse.eLClick, ToggleStack );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DiploOverview.lua}}
:<code>UI/InGame/Popups/DiploOverview.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0043}}<syntaxhighlight lang="lua">Controls.DealsButton:RegisterCallback( Mouse.eLClick, OnDeals );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0060}}<syntaxhighlight lang="lua">Controls.RelationsButton:RegisterCallback( Mouse.eLClick, OnRelations );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DiploTrade.lua}}
:<code>UI/InGame/LeaderHead/DiploTrade.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0007}}<syntaxhighlight lang="lua">Controls.WhatWillMakeThisWorkButton:RegisterCallback( Mouse.eLClick, OnEqualizeDeal );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DiscussionDialog.lua}}
:<code>UI/InGame/LeaderHead/DiscussionDialog.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0973}}<syntaxhighlight lang="lua">Controls.DenounceConfirmYes:RegisterCallback( Mouse.eLClick, OnDenonceConfirmYes );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|EndGameMenu.lua}}
:<code>UI/InGame/Popups/EndGameMenu.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0227}}<syntaxhighlight lang="lua">Controls.GameOverButton:RegisterCallback( Mouse.eLClick, OnGameOver );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|EspionageOverview.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/Popups/EspionageOverview.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0314}}<syntaxhighlight lang="lua">Controls.CancelButton:RegisterCallback(Mouse.eLClick, function() Refresh(); end);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0733}}<syntaxhighlight lang="lua">agentEntry.StageCoupButton:RegisterCallback(Mouse.eLClick, OnCoupClicked);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|GPList.lua}}
:<code>UI/InGame/GPList.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0281}}<syntaxhighlight lang="lua">Controls.EngineerToggle:RegisterCallback( Mouse.eLClick, OnEngineerToggle );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0379}}<syntaxhighlight lang="lua">Controls.SortCity:RegisterCallback( Mouse.eLClick, OnSort );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|HappinessInfo.lua}}
:<code>UI/InGame/Popups/HappinessInfo.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0127}}<syntaxhighlight lang="lua">Controls.ResourcesImportedToggle:RegisterCallback( Mouse.eLClick, OnResourcesImportedToggle );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|HappinessInfo.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/Popups/HappinessInfo.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0077}}<syntaxhighlight lang="lua">Controls.LocalCityToggle:RegisterCallback( Mouse.eLClick, OnLocalCityToggle );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|InGame.lua}}
:<code>UI/InGame/InGame.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1048}}<syntaxhighlight lang="lua">Controls.ScrollTop:RegisterCallback( Mouse.eMouseExit, ScrollMouseExit );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|InstalledPanel.lua}}
:<code>UI/FrontEnd/Modding/InstalledPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0302}}<syntaxhighlight lang="lua">listing.Button:RegisterCallback(Mouse.eMouseEnter, OnListingMouseEnter);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|Lobby.lua}}
:<code>UI/FrontEnd/Multiplayer/Lobby.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0363}}<syntaxhighlight lang="lua">controlTable.Button:RegisterCallback( Mouse.eLClick, SelectGame );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|MainMenu.lua}}
:<code>UI/FrontEnd/MainMenu.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0066}}<syntaxhighlight lang="lua">Controls.ModsButton:RegisterCallback( Mouse.eLClick, ModsButtonClick );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ModsBrowser.lua}}
:<code>UI/FrontEnd/Modding/ModsBrowser.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0036}}<syntaxhighlight lang="lua">Controls.BackButton:RegisterCallback(Mouse.eLClick, NavigateBack);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|MPGameOptions.lua}}
:<code>UI/FrontEnd/Multiplayer/GameSetup/MPGameOptions.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0829}}<syntaxhighlight lang="lua">controlTable.Button:RegisterCallback(Mouse.eLClick, function()</syntaxhighlight>
{{CodeLine5|0830}}<syntaxhighlight lang="lua">dropDownButton:SetText(possibleValue.Name);</syntaxhighlight>
{{CodeLine5|0831}}<syntaxhighlight lang="lua">dropDownButton:SetToolTipString(possibleValue.ToolTip);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0833}}<syntaxhighlight lang="lua">PreGame.SetMapOption(option.ID, possibleValue.Value);</syntaxhighlight>
{{CodeLine5|0834}}<syntaxhighlight lang="lua">SendGameOptionChanged();</syntaxhighlight>
{{CodeLine5|0835}}<syntaxhighlight lang="lua">end);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|NotificationPanel.lua}}
:<code>UI/InGame/WorldView/NotificationPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0043}}<syntaxhighlight lang="lua">Controls[ "ProductionButton" ]:RegisterCallback( Mouse.eLClick, GenericLeftClick );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|NotificationPanel.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/WorldView/NotificationPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0043}}<syntaxhighlight lang="lua">Controls["StealTechButton"]:RegisterCallback(Mouse.eLClick, GenericLeftClick);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ReligionOverview.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/Popups/ReligionOverview.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0212}}<syntaxhighlight lang="lua">Controls.TabButtonYourReligion:RegisterCallback( Mouse.eLClick, function() TabSelect("YourReligion"); end);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|SetCivNames.lua}}
:<code>UI/FrontEnd/GameSetup/SetCivNames.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0172}}<syntaxhighlight lang="lua">Controls.EditCivAdjective:RegisterCallback(Validate);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|SinglePlayer.lua}}
:<code>UI/FrontEnd/SinglePlayer.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0133}}<syntaxhighlight lang="lua">Controls.ScenariosButton:RegisterCallback( Mouse.eLClick, ScenariosClicked );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|StagingRoom.lua}}
:<code>UI/FrontEnd/Multiplayer/StagingRoom.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0062}}<syntaxhighlight lang="lua">Controls.InviteButton:RegisterCallback( Mouse.eLClick, OnInviteButton );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TerrainPanel.lua}}
:<code>UI/InGame/TerrainPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0093}}<syntaxhighlight lang="lua">Controls.WaterGradientScale_ButtonUp:RegisterCallback( Mouse.eLClick, IncWaterGradientScale );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TradeLogic.lua}}
:<code>UI/InGame/WorldView/TradeLogic.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0838}}<syntaxhighlight lang="lua">Controls.ProposeButton:RegisterCallback( Mouse.eLClick, OnPropose );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|2078}}<syntaxhighlight lang="lua">Controls.ThemPocketOpenBorders:RegisterCallback( Mouse.eLClick, PocketOpenBordersHandler );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|2171}}<syntaxhighlight lang="lua">Controls.UsTableResearchAgreement:RegisterCallback( Mouse.eLClick, TableResearchAgreementHandler );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|2473}}<syntaxhighlight lang="lua">instance.Button:RegisterCallback( Mouse.eLClick, OnChooseCity );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|2675}}<syntaxhighlight lang="lua">Controls.UsPocketLeaderClose:RegisterCallback( Mouse.eLClick, LeaderClose );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|VictoryProgress.lua}}
:<code>UI/InGame/Popups/VictoryProgress.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0132}}<syntaxhighlight lang="lua">Controls.SpaceRaceClose:RegisterCallback( Mouse.eLClick, OnSpaceRaceClose );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|WorldPicker.lua}}
:<code>UI/FrontEnd/WorldPicker.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0022}}<syntaxhighlight lang="lua">Controls.TinyWorldSizeButton:RegisterCallback( eLClick, TinyWorldSizeButtonClick );</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|RegisterCallback]]