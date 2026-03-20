{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This method is declared by '''ControlBase'''.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''void''' UIElement:SetToolTipString<b>(</b>'''string''' foodToolTip<b>)</b></code>


'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|foodToolTip:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Too many occurences. Only 50 out of 751 are listed.''

{{PseudoH4|AdvancedSetup.lua}}
:<code>UI/FrontEnd/GameSetup/AdvancedSetup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0117}}<syntaxhighlight lang="lua">dropDownButton:SetToolTipString(possibleValue.ToolTip);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1109}}<syntaxhighlight lang="lua">Controls.StartButton:SetToolTipString(nil);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ChooseFaithGreatPerson.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/Popups/ChooseFaithGreatPerson.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0044}}<syntaxhighlight lang="lua">controlTable.Button:SetToolTipString(Locale.ConvertTextKey("TXT_KEY_NO_SCIENTIST_FROM_FAITH"));</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ChooseReligionPopup.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/Popups/ChooseReligionPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0308}}<syntaxhighlight lang="lua">religionButton.Button:SetToolTipString(t);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CityBannerManager.lua}}
:<code>UI/InGame/CityBannerManager.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0217}}<syntaxhighlight lang="lua">controls.OccupiedIcon:SetToolTipString(Locale.ConvertTextKey( "TXT_KEY_CITY_OCCUPIED"));</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0344}}<syntaxhighlight lang="lua">controls.CityBannerLeftBackground:SetToolTipString(tooltipString);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0515}}<syntaxhighlight lang="lua">controls.BannerButton:SetToolTipString(Locale.ConvertTextKey("TXT_KEY_HAVENT_MET"));</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CityStateDiploPopup.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/Popups/CityStateDiploPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0278}}<syntaxhighlight lang="lua">Controls.AllyIcon:SetToolTipString(strAllyTT);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0540}}<syntaxhighlight lang="lua">Controls.RevokePledgeButton:SetToolTipString(strRevokeProtectTT);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0999}}<syntaxhighlight lang="lua">Controls.UnitTributeButton:SetToolTipString(ttText);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CityView.lua}}
:<code>UI/InGame/CityView/CityView.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0426}}<syntaxhighlight lang="lua">controlTable.BuildingFilledSpecialistSlot3:SetToolTipString(ToolTipString);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0786}}<syntaxhighlight lang="lua">Controls.ProductionButton:SetToolTipString( Locale.ConvertTextKey( "TXT_KEY_CITYVIEW_QUEUE_PROD_TT") );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1333}}<syntaxhighlight lang="lua">Controls.RazeCityButton:SetToolTipString( Locale.ConvertTextKey( "TXT_KEY_CITYVIEW_RAZE_BUTTON_TT" ) );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1773}}<syntaxhighlight lang="lua">controlTable.PlotButtonImage:SetToolTipString( Locale.ConvertTextKey("TXT_KEY_CITYVIEW_NUTHA_CITY_TILE") );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CivilopediaScreen.lua}}
:<code>UI/Civilopedia/CivilopediaScreen.lua</code>
:{{CodeBegin5}}
{{CodeLine5|2087}}<syntaxhighlight lang="lua">thisBuildingInstance.UnlockedBuildingButton:SetToolTipString( Locale.ConvertTextKey( thisBuildingInfo.Description ) );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|Demographics.lua}}
:<code>UI/InGame/Popups/Demographics.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0171}}<syntaxhighlight lang="lua">instance.BestTT:SetToolTipString( Locale.ConvertTextKey("TXT_KEY_DEMOGRAPHICS_FOOD_MEASURE") );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0179}}<syntaxhighlight lang="lua">instance.WorstTT:SetToolTipString( Locale.ConvertTextKey("TXT_KEY_DEMOGRAPHICS_FOOD_MEASURE") );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DiploList.lua}}
:<code>UI/InGame/DiploList.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0443}}<syntaxhighlight lang="lua">controlTable.MinorButton:SetToolTipString(Locale.ConvertTextKey("TXT_KEY_ALWAYS_WAR_TT"));</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DiploRelationships.lua}}
:<code>UI/InGame/Popups/DiploRelationships.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0486}}<syntaxhighlight lang="lua">pStack.StatusMeter:SetToolTipString(strStatusTT);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0547}}<syntaxhighlight lang="lua">pStack.AllyLabel:SetToolTipString(strAllyTT);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DiscussionDialog.lua}}
:<code>UI/InGame/LeaderHead/DiscussionDialog.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0336}}<syntaxhighlight lang="lua">Controls.Button2:SetToolTipString(strButton2Tooltip);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|EconomicGeneralInfo.lua}}
:<code>UI/InGame/Popups/EconomicGeneralInfo.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0261}}<syntaxhighlight lang="lua">instance.TradeIncomeValue:SetToolTipString( strTooltip .. strPopInfo );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|EspionageOverview.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/Popups/EspionageOverview.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0638}}<syntaxhighlight lang="lua">agentEntry.AgentActivity:SetToolTipString(strActivityTT);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1199}}<syntaxhighlight lang="lua">entry.RigElectionEnabled:SetToolTipString(strCityStateTT);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|FoRScenarioLoadScreen.lua (G&K)}}
:<code>DLC/Expansion/Scenarios/FallOfRomeScenario/FoRScenarioLoadScreen.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0108}}<syntaxhighlight lang="lua">controlTable.Button:SetToolTipString(Locale.ConvertTextKey( info.Help ) );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|GameMenu.lua}}
:<code>UI/InGame/Menus/GameMenu.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0218}}<syntaxhighlight lang="lua">Controls.LeaderFrame:SetToolTipString( Locale.ConvertTextKey( leaderDescription ) );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0272}}<syntaxhighlight lang="lua">Controls.TypeFrame:SetToolTipString(Locale.ConvertTextKey("TXT_KEY_RANDOM_MAP_SCRIPT") );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0282}}<syntaxhighlight lang="lua">Controls.SizeFrame:SetToolTipString( Locale.ConvertTextKey( "TXT_KEY_RANDOM_MAP_SIZE" ) );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0289}}<syntaxhighlight lang="lua">Controls.DifficultyFrame:SetToolTipString( Locale.ConvertTextKey( info.Description ) );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|GameSetupScreen.lua}}
:<code>UI/FrontEnd/GameSetup/GameSetupScreen.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0513}}<syntaxhighlight lang="lua">Controls[buttonName]:SetToolTipString( unknownString );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|GPList.lua}}
:<code>UI/InGame/GPList.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0147}}<syntaxhighlight lang="lua">instance.GPMeter:SetToolTipString( strProgress );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|HappinessInfo.lua}}
:<code>UI/InGame/Popups/HappinessInfo.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0523}}<syntaxhighlight lang="lua">Controls.PopulationUnhappiness:SetToolTipString(strTooltip);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|LoadMenu.lua}}
:<code>UI/FrontEnd/LoadMenu.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0275}}<syntaxhighlight lang="lua">Controls.CivIcon:SetToolTipString(unknownString);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0357}}<syntaxhighlight lang="lua">Controls.MapType:SetToolTipString(name);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|Lobby.lua}}
:<code>UI/FrontEnd/Multiplayer/Lobby.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0346}}<syntaxhighlight lang="lua">controlTable.DLCHostedLabel:SetToolTipString(CreateDlcToolTip("TXT_KEY_LOBBY_REQUIRED_DLC", filteredPackages));</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|MiniMapPanel.lua}}
:<code>UI/InGame/WorldView/MiniMapPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0425}}<syntaxhighlight lang="lua">Controls.StrategicViewButton:SetToolTipString(sToolTip .. " (" .. keyDesc .. ")");</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ModsBrowser.lua}}
:<code>UI/FrontEnd/Modding/ModsBrowser.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0064}}<syntaxhighlight lang="lua">button:SetToolTipString(tooltip);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ProductionPopup.lua}}
:<code>UI/InGame/Popups/ProductionPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0238}}<syntaxhighlight lang="lua">Controls.Food:SetToolTipString(strFoodToolTip);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0244}}<syntaxhighlight lang="lua">Controls.Gold:SetToolTipString(strGoldToolTip);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|SaveMapMenu.lua}}
:<code>UI/InGame/Menus/SaveMapMenu.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0247}}<syntaxhighlight lang="lua">controlTable.ButtonText:SetToolTipString(v.Description);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|SelectMapType.lua}}
:<code>UI/FrontEnd/GameSetup/SelectMapType.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0214}}<syntaxhighlight lang="lua">item.Button:SetToolTipString(v.Description);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TechButtonInclude.lua}}
:<code>UI/InGame/TechTree/TechButtonInclude.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0222}}<syntaxhighlight lang="lua">thisButton:SetToolTipString( Locale.ConvertTextKey( "TXT_KEY_FASTER_EMBARKED_MOVEMENT" ) );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0277}}<syntaxhighlight lang="lua">thisButton:SetToolTipString( Locale.ConvertTextKey( "TXT_KEY_ALLOWS_DEFENSIVE_PACTS" ) );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TechButtonInclude.lua (G&K)}}
:<code>DLC/Expansion/Scenarios/SteampunkScenario/TechButtonInclude.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0474}}<syntaxhighlight lang="lua">thisButton:SetToolTipString( Locale.ConvertTextKey("TXT_KEY_REVEALS_RESOURCE_ON_MAP", resourceName));</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TradeLogic.lua}}
:<code>UI/InGame/WorldView/TradeLogic.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1094}}<syntaxhighlight lang="lua">Controls.UsPocketOpenBorders:SetToolTipString(strOurTooltip);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1240}}<syntaxhighlight lang="lua">Controls.ThemPocketTradeAgreement:SetToolTipString(strTooltip);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1454}}<syntaxhighlight lang="lua">Controls.ThemPocketLuxury:SetToolTipString( Locale.ConvertTextKey( "TXT_KEY_DIPLO_LUX_RESCR_TRADE_NO_THEM" ));</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1687}}<syntaxhighlight lang="lua">Controls.UsTableGoldPerTurn:SetToolTipString( strTooltip );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|VictoryStatus.lua (G&K)}}
:<code>DLC/Expansion/Scenarios/SteampunkScenario/VictoryStatus.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0139}}<syntaxhighlight lang="lua">gtTokenUI[s].TokenLabel:SetToolTipString(sLabelTT);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|VoteResultsPopup.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/Popups/VoteResultsPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0203}}<syntaxhighlight lang="lua">controlTable.VoteCastBox:SetToolTipString(strVoteCastTT);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|SetToolTipString]]