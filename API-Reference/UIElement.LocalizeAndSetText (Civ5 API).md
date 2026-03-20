{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This method is declared by {{Type5|EditBox}}, {{Type5|GridButton}}, {{Type5|Image}}, {{Type5|Label}}, '''TextBase''' and {{Type5|TextButton}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''void''' UIElement:LocalizeAndSetText<b>(</b>'''string''' name, '''int''' searchString = nil, '''string''' minFaithForProphet = nil, '''unknown''' arg3, '''unknown''' arg4, '''unknown''' arg5, '''unknown''' arg6, '''unknown''' arg7, '''unknown''' arg8, '''string''' arg9, '''unknown''' arg10, '''unknown''' arg11<b>)</b></code>


'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|name:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|searchString:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|minFaithForProphet:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|arg3:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|arg4:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|arg5:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|arg6:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|arg7:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|arg8:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|arg9:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|arg10:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|arg11:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Too many occurences. Only 50 out of 668 are listed.''

{{PseudoH4|AdvancedSetup.lua}}
:<code>UI/FrontEnd/GameSetup/AdvancedSetup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0491}}<syntaxhighlight lang="lua">pullDown:GetButton():LocalizeAndSetText(era.Description);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0636}}<syntaxhighlight lang="lua">Controls.MapSizePullDown:GetButton():LocalizeAndSetText("TXT_KEY_RANDOM_MAP_SIZE");</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0986}}<syntaxhighlight lang="lua">controlTable.Button:LocalizeAndSetText("TXT_KEY_MULTIPLAYER_DEFAULT_TEAM_NAME", i + 1);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1025}}<syntaxhighlight lang="lua">Controls.TeamLabel:LocalizeAndSetText( "TXT_KEY_MULTIPLAYER_DEFAULT_TEAM_NAME", PreGame.GetTeam(0) + 1 );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ChooseMayaBonus.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/Popups/ChooseMayaBonus.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0018}}<syntaxhighlight lang="lua">Controls.DescriptionLabel:LocalizeAndSetText("TXT_KEY_CHOOSE_LONG_COUNT_TT");</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ChooseReligionPopup.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/Popups/ChooseReligionPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0340}}<syntaxhighlight lang="lua">Controls.FounderBeliefDescription:LocalizeAndSetText("TXT_KEY_CHOOSE_RELIGION_SELECT_FOUNDER_BELIEF");</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0501}}<syntaxhighlight lang="lua">Controls.NewName:LocalizeAndSetText(g_CurrentReligionName);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CivsAlive.lua - DLC_01 DLC}}
:<code>DLC/DLC_01/Scenarios/Mongol Scenario/CivsAlive.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0035}}<syntaxhighlight lang="lua">Controls.CivsAliveLabel:LocalizeAndSetText("TXT_KEY_MONGOL_SCENARIO_CIVSALIVE", iRemainingToDestroy, iTurnsRemaining);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CustomMod.lua}}
:<code>UI/FrontEnd/Modding/CustomMod.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0096}}<syntaxhighlight lang="lua">Controls.Title:LocalizeAndSetText( "TXT_KEY_SELECT_CUSTOM_GAME" );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|Demographics.lua}}
:<code>UI/InGame/Popups/Demographics.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0163}}<syntaxhighlight lang="lua">instance.Name:LocalizeAndSetText( "TXT_KEY_DEMOGRAPHICS_FOOD" );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DiploGlobalRelationships.lua}}
:<code>UI/InGame/Popups/DiploGlobalRelationships.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0269}}<syntaxhighlight lang="lua">textControls.Text:LocalizeAndSetText("TXT_KEY_ALLIED_WITH", thirdName);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|EconomicGeneralInfo.lua}}
:<code>UI/InGame/Popups/EconomicGeneralInfo.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0379}}<syntaxhighlight lang="lua">Controls.CityToggle:LocalizeAndSetText("TXT_KEY_EO_INCOME_CITIES_COLLAPSE");</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0397}}<syntaxhighlight lang="lua">Controls.TradeToggle:LocalizeAndSetText("TXT_KEY_EO_INCOME_TRADE_DETAILS");</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0411}}<syntaxhighlight lang="lua">Controls.BuildingsToggle:LocalizeAndSetText("TXT_KEY_EO_BUILDINGS_COLLAPSE");</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|EnemyUnitPanel.lua}}
:<code>UI/InGame/WorldView/EnemyUnitPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0447}}<syntaxhighlight lang="lua">controlTable.Text:LocalizeAndSetText(  "TXT_KEY_EUPANEL_BONUS_GOLDEN_AGE" );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0509}}<syntaxhighlight lang="lua">controlTable.Text:LocalizeAndSetText( "TXT_KEY_EUPANEL_REVERSE_GG_NEAR" );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0830}}<syntaxhighlight lang="lua">controlTable.Text:LocalizeAndSetText( "TXT_KEY_EUPANEL_FIGHT_AT_HOME_BONUS" );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0838}}<syntaxhighlight lang="lua">controlTable.Text:LocalizeAndSetText( "TXT_KEY_EUPANEL_ATTACK_IN_FRIEND_LANDS" );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0904}}<syntaxhighlight lang="lua">controlTable.Text:LocalizeAndSetText( "TXT_KEY_EUPANEL_BONUS_VS_CLASS" , unitClassType );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0963}}<syntaxhighlight lang="lua">controlTable.Text:LocalizeAndSetText( "TXT_KEY_EUPANEL_HILL_ATTACK_BONUS" );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1196}}<syntaxhighlight lang="lua">controlTable.Text:LocalizeAndSetText(  "TXT_KEY_EUPANEL_EXTRA_PERCENT" );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1218}}<syntaxhighlight lang="lua">controlTable.Text:LocalizeAndSetText(  "TXT_KEY_EUPANEL_OUTSIDE_HOME_BONUS" );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|EspionageOverview.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/Popups/EspionageOverview.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0395}}<syntaxhighlight lang="lua">Controls.AgentLocation:LocalizeAndSetText(city:GetName());</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0545}}<syntaxhighlight lang="lua">agentEntry.AgentName:LocalizeAndSetText(v.Name);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1053}}<syntaxhighlight lang="lua">Controls.ConfirmText:LocalizeAndSetText("TXT_KEY_EO_RELOCATE_SPY_QUESTION");</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|GameMenu.lua}}
:<code>UI/InGame/Menus/GameMenu.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0377}}<syntaxhighlight lang="lua">controlTable.Text:LocalizeAndSetText("TXT_KEY_AD_HANDICAP_SETTING", Locale.ConvertTextKey( info.Description ) );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0411}}<syntaxhighlight lang="lua">controlTable.Text:LocalizeAndSetText(option.Description);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|GPList.lua}}
:<code>UI/InGame/GPList.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0255}}<syntaxhighlight lang="lua">Controls.ArtistToggle:LocalizeAndSetText("TXT_KEY_GP_ARTIST_DETAILS_COLLAPSE");</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0291}}<syntaxhighlight lang="lua">Controls.MerchantToggle:LocalizeAndSetText("TXT_KEY_GP_MERCHANT_DETAILS");</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0306}}<syntaxhighlight lang="lua">Controls.ScientistToggle:LocalizeAndSetText("TXT_KEY_GP_SCIENTIST_DETAILS_COLLAPSE");</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|HallOfFame.lua}}
:<code>UI/InGame/Popups/HallOfFame.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0042}}<syntaxhighlight lang="lua">controlTable.DidWin:LocalizeAndSetText("TXT_KEY_VICTORY_BANG");</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0057}}<syntaxhighlight lang="lua">controlTable.LeaderName:LocalizeAndSetText(v.LeaderName);</syntaxhighlight>
{{CodeLine5|0058}}<syntaxhighlight lang="lua">controlTable.CivName:LocalizeAndSetText(v.CivilizationName);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0130}}<syntaxhighlight lang="lua">controlTable.WinType:LocalizeAndSetText("");</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|HappinessInfo.lua}}
:<code>UI/InGame/Popups/HappinessInfo.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0021}}<syntaxhighlight lang="lua">Controls.LuxuryHappinessToggle:LocalizeAndSetText("TXT_KEY_EO_LUXURY_HAPPINESS_COLLAPSE");</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|InstalledPanel.lua}}
:<code>UI/FrontEnd/Modding/InstalledPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0259}}<syntaxhighlight lang="lua">listing.StatusLabel:LocalizeAndSetText("TXT_KEY_MODDING_INSTALL_PROGRESS", FileSizeAsString(downloadedBytes), FileSizeAsString(totalBytes));</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|JoiningRoom.lua}}
:<code>UI/FrontEnd/Multiplayer/JoiningRoom.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0124}}<syntaxhighlight lang="lua">Controls.JoiningLabel:LocalizeAndSetText( "TXT_KEY_MULTIPLAYER_JOINING_ROOM" );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|MilitaryOverview.lua}}
:<code>UI/InGame/Popups/MilitaryOverview.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0162}}<syntaxhighlight lang="lua">instance.UnitName:LocalizeAndSetText( sortEntry.name );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|MPGameOptions.lua}}
:<code>UI/FrontEnd/Multiplayer/GameSetup/MPGameOptions.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0339}}<syntaxhighlight lang="lua">Controls.EraPull:GetButton():LocalizeAndSetText( info.Description );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0427}}<syntaxhighlight lang="lua">Controls.GameSpeedPullDown:GetButton():LocalizeAndSetText(GameInfo.GameSpeeds[id].Description);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0442}}<syntaxhighlight lang="lua">controlTable.Button:LocalizeAndSetText( "TXT_KEY_RANDOM_MAP_SIZE" );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|MPGameSetupScreen.lua}}
:<code>UI/FrontEnd/Multiplayer/GameSetup/MPGameSetupScreen.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0114}}<syntaxhighlight lang="lua">Controls.TitleLabel:LocalizeAndSetText( "TXT_KEY_MOD_MP_GAME_SETUP_HEADER" );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|MPList.lua}}
:<code>UI/InGame/WorldView/MPList.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0159}}<syntaxhighlight lang="lua">controlTable.Name:LocalizeAndSetText( "TXT_KEY_POP_VOTE_RESULTS_UNMET_PLAYER" );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ProductionPopup.lua}}
:<code>UI/InGame/Popups/ProductionPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0175}}<syntaxhighlight lang="lua">Controls.PurchaseString:LocalizeAndSetText( "TXT_KEY_CITYVIEW_PRODUCE_BUTTON" );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ReligionOverview.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/Popups/ReligionOverview.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0238}}<syntaxhighlight lang="lua">entry.FaithModifier:LocalizeAndSetText("TXT_KEY_TP_FAITH_FROM_MINORS", iFaithFromMinorCivs);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ReplayViewer.lua}}
:<code>UI/InGame/Popups/ReplayViewer.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0722}}<syntaxhighlight lang="lua">graphLegendInstance.LegendName:LocalizeAndSetText(player.CivShortDescription);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|StagingRoom.lua}}
:<code>UI/FrontEnd/Multiplayer/StagingRoom.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0208}}<syntaxhighlight lang="lua">slotInstance.TeamLabel:LocalizeAndSetText( "TXT_KEY_MULTIPLAYER_DEFAULT_TEAM_NAME", teamID );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0339}}<syntaxhighlight lang="lua">slotInstance.CivLabel:LocalizeAndSetText( "TXT_KEY_RANDOM_LEADER" );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|SteampunkScenarioLoadScreen.lua (G&K)}}
:<code>DLC/Expansion/Scenarios/SteampunkScenario/SteampunkScenarioLoadScreen.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0340}}<syntaxhighlight lang="lua">Controls.Title:LocalizeAndSetText("TXT_KEY_RANDOM_LEADER_CIV", leaderDescription, civ.ShortDescription);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|UnitPanel.lua}}
:<code>UI/InGame/WorldView/UnitPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0591}}<syntaxhighlight lang="lua">Controls.UnitStatNameMovement:LocalizeAndSetText("TXT_KEY_UPANEL_RANGEMOVEMENT");</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|LocalizeAndSetText]]