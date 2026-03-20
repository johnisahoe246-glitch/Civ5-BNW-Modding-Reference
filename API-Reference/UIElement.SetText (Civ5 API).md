{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This method is declared by {{Type5|EditBox}}, {{Type5|Grid}}, {{Type5|GridButton}}, {{Type5|Image}}, {{Type5|Label}}, {{Type5|Slider}}, '''TextBase''' and {{Type5|TextButton}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''void''' UIElement:SetText<b>(</b>'''string''' localizedString<b>)</b></code>


'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|localizedString:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Too many occurences. Only 50 out of 2489 are listed.''

{{PseudoH4|AdvisorCounselPopup.lua}}
:<code>UI/InGame/Popups/AdvisorCounselPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0127}}<syntaxhighlight lang="lua">Controls.MACounselText:SetText(strText);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ChangePassword.lua}}
:<code>UI/InGame/ChangePassword.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0107}}<syntaxhighlight lang="lua">Controls.RetypeNewPasswordEditBox:SetText( "" );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ChoosePantheonPopup.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/Popups/ChoosePantheonPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0104}}<syntaxhighlight lang="lua">itemInstance.Description:SetText(pantheon.Description);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ChooseReligionPopup.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/Popups/ChooseReligionPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0366}}<syntaxhighlight lang="lua">Controls.FollowerBeliefDescription:SetText(Locale.Lookup(belief.Description));</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CityView.lua}}
:<code>UI/InGame/CityView/CityView.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0820}}<syntaxhighlight lang="lua">Controls.ProductionButtonLabel:SetText( Locale.ConvertTextKey( "TXT_KEY_CITYVIEW_CHANGE_PROD") );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1116}}<syntaxhighlight lang="lua">Controls.SpecialBuildingsHeaderLabel:SetText(localizedLabel);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1299}}<syntaxhighlight lang="lua">Controls.ResourceDemandedString:SetText(szText);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1855}}<syntaxhighlight lang="lua">controlTable.BuyPlotAnchoredButtonLabel:SetText( "[COLOR_WARNING_TEXT]"..tostring(iPlotCost).."[ENDCOLOR]" );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CityView.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/CityView/CityView.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1497}}<syntaxhighlight lang="lua">Controls.EndTurnText:SetText(Locale.ConvertTextKey("TXT_KEY_CITYVIEW_RETURN_TO_ESPIONAGE"));</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CivilopediaScreen.lua}}
:<code>UI/Civilopedia/CivilopediaScreen.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1582}}<syntaxhighlight lang="lua">Controls.ArticleID:SetText( Locale.ConvertTextKey( "TXT_KEY_PEDIA_CIVILIZATIONS_PAGE_LABEL" ));</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|4745}}<syntaxhighlight lang="lua">thisListInstance.ListItemLabel:SetText( Locale.ConvertTextKey( "TXT_KEY_PEDIA_UNITS_PAGE_LABEL" ));</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|Credits.lua}}
:<code>UI/FrontEnd/Credits.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0071}}<syntaxhighlight lang="lua">majorTitle.Text:SetText(creditLine);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DebugMenu.lua}}
:<code>UI/InGame/DebugMenu.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0235}}<syntaxhighlight lang="lua">Controls.ParticleEffectsStats_Label4:SetText("Rendered Particles: "      .. tostring(responseData.NumRenderedParticles));</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DebugMode.lua}}
:<code>UI/InGame/DebugMode.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0477}}<syntaxhighlight lang="lua">Controls.CityPlayer_Label:SetText(" " .. g_iCurrPlayer .. " " );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0634}}<syntaxhighlight lang="lua">Controls.UnitVariableValue_Label:SetText( string.format("%.1f", g_fVariableValue) );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|Demographics.lua}}
:<code>UI/InGame/Popups/Demographics.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0146}}<syntaxhighlight lang="lua">instance.Rank:SetText( Locale.ToNumber(GetRank( m_PopulationTable, iPlayer ), "#") );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0370}}<syntaxhighlight lang="lua">instance.Average:SetText( Locale.ToNumber( GetAverage( m_ApprovalTable, iPlayer ), "#'%'" ) );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DiploCurrentDeals.lua}}
:<code>UI/InGame/Popups/DiploCurrentDeals.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0126}}<syntaxhighlight lang="lua">Controls.CurrentDealsButton:SetText( "[ICON_PLUS]" .. Locale.ConvertTextKey( "{TXT_KEY_DO_CURRENT_DEALS:upper}" ) );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0153}}<syntaxhighlight lang="lua">Controls.TurnStart:SetText( Locale.ConvertTextKey( "TXT_KEY_DO_ON_TURN", iBeginTurn ) );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DiploGlobalRelationships.lua}}
:<code>UI/InGame/Popups/DiploGlobalRelationships.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0098}}<syntaxhighlight lang="lua">textControls.Text:SetText(strText);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DiploList.lua}}
:<code>UI/InGame/DiploList.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0448}}<syntaxhighlight lang="lua">controlTable.StatusText:SetText( strDiploState);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|EconomicGeneralInfo.lua}}
:<code>UI/InGame/Popups/EconomicGeneralInfo.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0359}}<syntaxhighlight lang="lua">Controls.TileExpenseValue:SetText( Locale.ToNumber( pPlayer:GetImprovementGoldMaintenance(), "#.##" ) );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0362}}<syntaxhighlight lang="lua">Controls.DiploExpenseValue:SetText( Locale.ToNumber( pPlayer:GetGoldPerTurnFromDiplomacy(), "#.##" ) );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|EspionageOverview.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/Popups/EspionageOverview.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0593}}<syntaxhighlight lang="lua">agentEntry.AgentActivity:SetText(v.AgentActivity);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1490}}<syntaxhighlight lang="lua">instance.CivilizationName:SetText(v.From);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|FoRScenarioLoadScreen.lua (G&K)}}
:<code>DLC/Expansion/Scenarios/FallOfRomeScenario/FoRScenarioLoadScreen.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0293}}<syntaxhighlight lang="lua">Controls.BonusDescription:SetText( "" );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|HappinessInfo.lua}}
:<code>UI/InGame/Popups/HappinessInfo.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0527}}<syntaxhighlight lang="lua">Controls.OPopulationUnhappinessTitle:SetText(Locale.ConvertTextKey("TXT_KEY_OCCUPIED_POP_UNHAPPINESS", iOccupiedPop));</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|InstalledPanel.lua}}
:<code>UI/FrontEnd/Modding/InstalledPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0547}}<syntaxhighlight lang="lua">detailValue.Label:SetText(value or "");</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|LoadMenu.lua}}
:<code>UI/FrontEnd/LoadMenu.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0243}}<syntaxhighlight lang="lua">Controls.GameType:SetText( Locale.ConvertTextKey("TXT_KEY_MULTIPLAYER_HOTSEAT_GAME") );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|MPGameOptions.lua}}
:<code>UI/FrontEnd/Multiplayer/GameSetup/MPGameOptions.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0419}}<syntaxhighlight lang="lua">controlTable.Button:SetText( Locale.ConvertTextKey( v.Description ) );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|OptionsMenu.lua}}
:<code>UI/Options/OptionsMenu.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0226}}<syntaxhighlight lang="lua">Controls.CountdownTimer:SetText( "20" );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0379}}<syntaxhighlight lang="lua">Controls.TitleLabel:SetText( m_PanelNames[ which ] );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0522}}<syntaxhighlight lang="lua">Controls.LanguagePull:GetButton():SetText(Locale.GetCurrentLanguage().DisplayName);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ProductionPopup.lua}}
:<code>UI/InGame/Popups/ProductionPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0174}}<syntaxhighlight lang="lua">Controls.PurchaseIcon:SetText( "[ICON_PRODUCTION]" );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0692}}<syntaxhighlight lang="lua">Controls[controlName]:SetText( Locale.ConvertTextKey( thisUnitInfo.Description ) );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ResourceList.lua}}
:<code>UI/InGame/ResourceList.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0136}}<syntaxhighlight lang="lua">instance.TradeInfo:SetText( strTradeInfo );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|SaveMenu.lua}}
:<code>UI/InGame/Menus/SaveMenu.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0045}}<syntaxhighlight lang="lua">Controls.Message:SetText( Locale.ConvertTextKey("TXT_KEY_OVERWRITE_TXT") );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0166}}<syntaxhighlight lang="lua">Controls.NameBox:SetText( entry.DisplayName );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|SetCivNames.lua}}
:<code>UI/FrontEnd/GameSetup/SetCivNames.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0243}}<syntaxhighlight lang="lua">Controls.EditRetypePassword:SetText( name );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|SupportFunctions.lua}}
:<code>UI/SupportFunctions.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0022}}<syntaxhighlight lang="lua">control:SetText(trailingText);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TechPopup.lua}}
:<code>UI/InGame/TechPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0218}}<syntaxhighlight lang="lua">thisTechButtonInstance.TechQueueLabel:SetText( tostring( queuePosition-1 ) );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TechTree.lua}}
:<code>UI/InGame/TechTree/TechTree.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0377}}<syntaxhighlight lang="lua">thisEraBlockInstance.CurrentLabel:SetText( localizedLabel );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TerrainPanel.lua}}
:<code>UI/InGame/TerrainPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0040}}<syntaxhighlight lang="lua">Controls.WaterNoiseScale_Label:SetText(g_iWaterNoiseScale);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TradeLogic.lua}}
:<code>UI/InGame/WorldView/TradeLogic.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0595}}<syntaxhighlight lang="lua">Controls.CancelButton:SetText( Locale.ConvertTextKey( "TXT_KEY_DIPLO_REFUSE" ));</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0987}}<syntaxhighlight lang="lua">Controls.ThemCiv:SetText( "(" .. Locale.ConvertTextKey( GameInfo.Civilizations[ g_pThem:GetCivilizationType() ].ShortDescription ) .. ")" );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1685}}<syntaxhighlight lang="lua">Controls.UsTableGoldPerTurnButton:SetText( strString );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|VictoryProgress.lua}}
:<code>UI/InGame/Popups/VictoryProgress.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0182}}<syntaxhighlight lang="lua">Controls.Tech:SetText(pPlayer:GetScoreFromTechs());</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0739}}<syntaxhighlight lang="lua">controlTable.LiberatedCivs:SetText(libCiv);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|VictoryStatus.lua (G&K)}}
:<code>DLC/Expansion/Scenarios/SteampunkScenario/VictoryStatus.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0096}}<syntaxhighlight lang="lua">Controls.HelpLabel:SetText(sHelpText);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|WhosWinningPopup.lua}}
:<code>UI/InGame/Popups/WhosWinningPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0288}}<syntaxhighlight lang="lua">controlTable.PlayerNameText:SetText(strName);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|SetText]]