{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Locale}}.<br/>
This is a static method, invoke it with a dot.
}}


Converts a text key into a localized string


=Usage=
<code>'''string''' Locale.ConvertTextKey<b>(</b>'''string''' key, ...<b>)</b></code>


'''Returned Value'''
:Returns the textkey if it cannot be found in the dictionary, or a translated string.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|key:
|valign="top"| ''A valid text key.''
|-
|valign="top" style="padding-right:6px;"|...:
|valign="top"| ''none or many arguments that are used when composing the final localized string.''
|}
'''Notes'''
:This is an alias for Locale.Lookup.
:This localized string may or may not be in the user's current language.  With support for fall-back language support, the localization system will attempt to search all available languages for the string.


=Examples=
<syntaxhighlight lang="lua" class="civ5-example">
local foo = Locale.ConvertTextKey("TXT_KEY_MAIN_MENU");
print(foo); -- prints "Main Menu" in English</syntaxhighlight>


=Source code samples=
''Too many occurences. Only 50 out of 4278 are listed.''

{{PseudoH4|ActionInfoPanel.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/WorldView/ActionInfoPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0380}}<syntaxhighlight lang="lua">strEndTurnMessage = Locale.ConvertTextKey("TXT_KEY_NOTIFICATION_SUMMARY_FOUND_RELIGION");</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CityStateDiploPopup.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/Popups/CityStateDiploPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0343}}<syntaxhighlight lang="lua">strResourceText = strResourceText .. pResource.IconString .. " [COLOR_POSITIVE_TEXT]" .. Locale.ConvertTextKey(pResource.Description) .. " (" .. iAmount .. ") [ENDCOLOR]";</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CityStateStatusHelper.lua (G&K)}}
:<code>DLC/Expansion/UI/CityStateStatusHelper.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0380}}<syntaxhighlight lang="lua">strStatusTT = strStatusTT .. Locale.ConvertTextKey("TXT_KEY_CSTATE_RESOURCES_RECEIVED", strExportedResourceText);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CityView.lua}}
:<code>UI/InGame/CityView/CityView.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1212}}<syntaxhighlight lang="lua">local localizedLabel = "[ICON_PLUS] "..Locale.ConvertTextKey( "TXT_KEY_CITYVIEW_REGULARBUILDING_TEXT" );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|2226}}<syntaxhighlight lang="lua">searchString = Locale.ConvertTextKey( thisUnitInfo.Description );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CivilopediaScreen.lua}}
:<code>UI/Civilopedia/CivilopediaScreen.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1608}}<syntaxhighlight lang="lua">UpdateSuperWideTextBlock( Locale.ConvertTextKey( "TXT_KEY_PEDIA_CIVS_HELP_TEXT" ), thisBBTextInstance.BBTextLabel, thisBBTextInstance.BBTextInnerFrame, thisBBTextInstance.BBTextFrame );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|2248}}<syntaxhighlight lang="lua">abilitiesString = abilitiesString ..  Locale.ConvertTextKey( "TXT_KEY_ABLTY_OCEAN_EMBARK_STRING" );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|2870}}<syntaxhighlight lang="lua">local strLabel = Locale.ConvertTextKey(GameInfo.Specialists[iGPType].GreatPeopleTitle);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|3828}}<syntaxhighlight lang="lua">UpdateTextBlock( Locale.ConvertTextKey( thisCityState.Civilopedia ), Controls.HistoryLabel, Controls.HistoryInnerFrame, Controls.HistoryFrame );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|3902}}<syntaxhighlight lang="lua">Controls.YieldLabel:SetText( Locale.ConvertTextKey( "TXT_KEY_PEDIA_NO_YIELD" ) );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DeclareWarMovePopup.lua}}
:<code>UI/InGame/PopupsGeneric/DeclareWarMovePopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0038}}<syntaxhighlight lang="lua">popupText = Locale.ConvertTextKey("TXT_KEY_POPUP_DOES_THIS_MEAN_WAR_PROTECTED_CITY_STATE", Teams[eRivalTeam]:GetNameKey());</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|Demographics.lua}}
:<code>UI/InGame/Popups/Demographics.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0209}}<syntaxhighlight lang="lua">instance.AverageTT:SetToolTipString( Locale.ConvertTextKey("TXT_KEY_DEMOGRAPHICS_PRODUCTION_MEASURE") );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DiploGlobalRelationships.lua}}
:<code>UI/InGame/Popups/DiploGlobalRelationships.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0133}}<syntaxhighlight lang="lua">controlTable.DenounceLabel:SetText(Locale.ConvertTextKey("TXT_KEY_DIPLO_YOU_HAVE_BACKSTABBED"));</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DiploRelationships.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/Popups/DiploRelationships.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0173}}<syntaxhighlight lang="lua">strDiploState = Locale.ConvertTextKey( "TXT_KEY_DIPLO_MAJOR_CIV_DIPLO_STATE_LIBERATED" );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DiploVotePopup.lua}}
:<code>UI/InGame/Popups/DiploVotePopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0081}}<syntaxhighlight lang="lua">TruncateString(controlTable.ButtonText, textBoxSize, Locale.ConvertTextKey("TXT_KEY_POP_UN_TEAM_LABEL", pOtherTeam:GetID() + 1) , " (" .. Locale.ConvertTextKey("TXT_KEY_POP_VOTE_RESULTS_YOUR_TEAM") .. ")");</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DiscussionDialog.lua}}
:<code>UI/InGame/LeaderHead/DiscussionDialog.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0312}}<syntaxhighlight lang="lua">strButton1Text = Locale.ConvertTextKey( "TXT_KEY_DIPLO_DISCUSS_YES_LET_US_PREPARE" );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DiscussionDialog.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/LeaderHead/DiscussionDialog.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0430}}<syntaxhighlight lang="lua">strButton4Tooltip = Locale.ConvertTextKey( "TXT_KEY_DIPLO_MAY_NOT_ATTACK" );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|EconomicGeneralInfo.lua}}
:<code>UI/InGame/Popups/EconomicGeneralInfo.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0299}}<syntaxhighlight lang="lua">strUnitTT = strUnitTT .. "[NEWLINE][NEWLINE]" .. Locale.ConvertTextKey("TXT_KEY_HANDICAP_MAINTENANCE_MOD", iUnitMaintMod);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|FoRScenarioLoadScreen.lua (G&K)}}
:<code>DLC/Expansion/Scenarios/FallOfRomeScenario/FoRScenarioLoadScreen.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0267}}<syntaxhighlight lang="lua">local title = Locale.ConvertTextKey("TXT_KEY_RANDOM_LEADER_CIV", leaderDescription, civ.ShortDescription);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|GameSetupScreen.lua}}
:<code>UI/FrontEnd/GameSetup/GameSetupScreen.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0528}}<syntaxhighlight lang="lua">title = Locale.ConvertTextKey( "TXT_KEY_RANDOM_LEADER_CIV", name, civName );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|GenericWorldAnchor.lua}}
:<code>UI/InGame/GenericWorldAnchor.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0263}}<syntaxhighlight lang="lua">strToolTip = strToolTip .. Locale.ConvertTextKey(strCustomHelp);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|GoodyHutPopup.lua}}
:<code>UI/InGame/Popups/GoodyHutPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0029}}<syntaxhighlight lang="lua">Controls.DescriptionLabel:SetText(Locale.ConvertTextKey(pGoodyInfo.Description));</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|HappinessInfo.lua}}
:<code>UI/InGame/Popups/HappinessInfo.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0448}}<syntaxhighlight lang="lua">Controls.OCityCountUnhappinessTitle:SetText(Locale.ConvertTextKey("TXT_KEY_NUMBER_OF_OCCUPIED_CITIES", iNumOccupiedCities));</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0605}}<syntaxhighlight lang="lua">Controls.ResourcesAvailableToggle:SetText("[ICON_PLUS]" .. Locale.ConvertTextKey("TXT_KEY_EO_RESOURCES_AVAILBLE"));</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|InfoTooltipInclude.lua}}
:<code>UI/InGame/InfoTooltipInclude.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0203}}<syntaxhighlight lang="lua">strHelpText = strHelpText .. Locale.ConvertTextKey("TXT_KEY_PRODUCTION_BUILDING_PRODUCTION", iProduction);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0780}}<syntaxhighlight lang="lua">strInfo = strInfo .. "[ICON_BULLET]" .. Locale.ConvertTextKey("TXT_KEY_DIPLO_DOF") .. "[NEWLINE]";</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|LoadMenu.lua}}
:<code>UI/FrontEnd/LoadMenu.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0233}}<syntaxhighlight lang="lua">Controls.EraTurn:SetText( Locale.ConvertTextKey("TXT_KEY_CUR_ERA_TURNS_FORMAT",</syntaxhighlight>
{{CodeLine5|0234}}<syntaxhighlight lang="lua">Locale.ConvertTextKey(GameInfo.Eras[header.CurrentEra].Description), header.TurnNumber) );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0378}}<syntaxhighlight lang="lua">Controls.Handicap:SetToolTipString( Locale.ConvertTextKey( info.Description ) );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|LoadTutorial.lua}}
:<code>UI/FrontEnd/LoadTutorial.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0167}}<syntaxhighlight lang="lua">Controls.TutorialNumber:SetText(  Locale.ConvertTextKey(Tutorials[ g_iSelected ].Num) );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|OptionsMenu.lua}}
:<code>UI/Options/OptionsMenu.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0568}}<syntaxhighlight lang="lua">m_FOWText[ 1 ] = Locale.ConvertTextKey("TXT_KEY_OPSCREEN_SETTINGS_LOW");</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0607}}<syntaxhighlight lang="lua">m_TutorialLevelText[ 3 ] = Locale.ConvertTextKey("TXT_KEY_OPSCREEN_TUTORIAL_OFF");</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ProductionPopup.lua}}
:<code>UI/InGame/Popups/ProductionPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0505}}<syntaxhighlight lang="lua">strItemName = Locale.ConvertTextKey(city:GetProductionNameKey());</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ReturnCivilianPopup.lua}}
:<code>UI/InGame/PopupsGeneric/ReturnCivilianPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0055}}<syntaxhighlight lang="lua">local buttonText = Locale.ConvertTextKey("TXT_KEY_POP_RETURN_CIVILIAN_CONFIRMATION_RETURN");</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|SocialPolicyPopup.lua}}
:<code>UI/InGame/Popups/SocialPolicyPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0235}}<syntaxhighlight lang="lua">szText = Locale.ConvertTextKey("TXT_KEY_CULTURE_PER_TURN_LABEL", player:GetTotalJONSCulturePerTurn());</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0357}}<syntaxhighlight lang="lua">strToolTip = strToolTip .. " " .. Locale.ConvertTextKey("TXT_KEY_POLICY_BRANCH_CANNOT_UNLOCK_CULTURE", player:GetNextPolicyCost());</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|StagingRoom.lua}}
:<code>UI/FrontEnd/Multiplayer/StagingRoom.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0314}}<syntaxhighlight lang="lua">local playerName = playerInfo.playerName or Locale.ConvertTextKey( "TXT_KEY_MULTIPLAYER_DEFAULT_PLAYER_NAME", playerID + 1);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TechButtonInclude.lua}}
:<code>UI/InGame/TechTree/TechButtonInclude.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0299}}<syntaxhighlight lang="lua">thisButton:SetToolTipString( Locale.ConvertTextKey( "TXT_KEY_ALLOWS_TRADE_AGREEMENTS" ) );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TopPanel.lua}}
:<code>UI/InGame/TopPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0761}}<syntaxhighlight lang="lua">strText = strText .. Locale.ConvertTextKey("TXT_KEY_NEXT_POLICY_TURN_LABEL", iTurns);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TopPanel.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/TopPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0629}}<syntaxhighlight lang="lua">strText = strText .. "  [ICON_BULLET]" .. Locale.ConvertTextKey("TXT_KEY_TP_HAPPINESS_CITIES", iCityHappiness);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TradeLogic.lua}}
:<code>UI/InGame/WorldView/TradeLogic.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0595}}<syntaxhighlight lang="lua">Controls.CancelButton:SetText( Locale.ConvertTextKey( "TXT_KEY_DIPLO_REFUSE" ));</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0755}}<syntaxhighlight lang="lua">control:SetText( "[ICON_MINUS]" .. Locale.ConvertTextKey( label ) );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1293}}<syntaxhighlight lang="lua">Controls.ThemPocketCities:SetToolTipString( Locale.ConvertTextKey( "TXT_KEY_DIPLO_TO_TRADE_CITY_TT" ));</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1670}}<syntaxhighlight lang="lua">strTooltip = Locale.ConvertTextKey( "TXT_KEY_DIPLO_CURRENT_GOLD", g_Deal:GetGoldAvailable(g_iThem, iItemToBeChanged) );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1950}}<syntaxhighlight lang="lua">local strTooltip = Locale.ConvertTextKey( "TXT_KEY_DIPLO_CURRENT_GOLD", g_Deal:GetGoldAvailable(g_iThem, iItemToBeChanged) );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TradeLogic.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/WorldView/TradeLogic.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1094}}<syntaxhighlight lang="lua">strOurTooltip = strOurTooltip .. " [COLOR_WARNING_TEXT]" .. Locale.ConvertTextKey("TXT_KEY_DIPLO_ALLOW_EMBASSY_NO_TECH_OTHER_PLAYER" ) .. "[ENDCOLOR]";</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TurnsRemaining.lua - DLC_04 DLC}}
:<code>DLC/DLC_04/Scenarios/1066Scenario/TurnsRemaining.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0166}}<syntaxhighlight lang="lua">Text = Locale.ConvertTextKey("TXT_KEY_1066_SCENARIO_ALLY_LOST", strPlayerKey);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TurnsRemaining.lua (G&K)}}
:<code>DLC/Expansion/Scenarios/MedievalScenario/TurnsRemaining.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0773}}<syntaxhighlight lang="lua">popupInfo.Text = Locale.ConvertTextKey("TXT_KEY_MEDIEVAL_SCENARIO_OTHER_ADOPTED_PROTESTANTISM", pPlayer:GetName());</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|UnitFlagManager.lua}}
:<code>UI/InGame/UnitFlagManager.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1585}}<syntaxhighlight lang="lua">local desc = Locale.ConvertTextKey("TXT_KEY_PLOTROLL_UNIT_DESCRIPTION_CIV",  pPlayer:GetCivilizationAdjectiveKey(), pUnit:GetNameKey());</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|UnitPanel.lua}}
:<code>UI/InGame/WorldView/UnitPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1055}}<syntaxhighlight lang="lua">strActionHelp = "[NEWLINE]" .. Locale.ConvertTextKey( "TXT_KEY_MISSION_START_GOLDENAGE_HELP", iGALength );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|VictoryProgress.lua}}
:<code>UI/InGame/Popups/VictoryProgress.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0905}}<syntaxhighlight lang="lua">controlTableTT:SetToolTipString(Locale.ConvertTextKey( "TXT_KEY_POP_VOTE_RESULTS_YOU" ));</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|ConvertTextKey]]