{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This method is declared by '''ControlBase'''.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''void''' UIElement:SetDisabled<b>(</b>'''bool''' disableBanners<b>)</b></code>


'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|disableBanners:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Too many occurences. Only 50 out of 522 are listed.''

{{PseudoH4|AdvancedSetup.lua}}
:<code>UI/FrontEnd/GameSetup/AdvancedSetup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0098}}<syntaxhighlight lang="lua">gameOption.OptionDropDown:SetDisabled(option.Disabled);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1104}}<syntaxhighlight lang="lua">Controls.StartButton:SetDisabled(not args.Valid);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|AdvisorCounselPopup.lua}}
:<code>UI/InGame/Popups/AdvisorCounselPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0079}}<syntaxhighlight lang="lua">Controls.EconomicNextButton:SetDisabled(not CanAdvisorCounselAdvance(AdvisorTypes.ADVISOR_ECONOMIC));</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0086}}<syntaxhighlight lang="lua">Controls.ForeignPrevButton:SetDisabled (not CanAdvisorCounselReverse(AdvisorTypes.ADVISOR_FOREIGN));</syntaxhighlight>
{{CodeLine5|0087}}<syntaxhighlight lang="lua">Controls.SciencePrevButton:SetDisabled (not CanAdvisorCounselReverse(AdvisorTypes.ADVISOR_SCIENCE));</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ChooseFaithGreatPerson.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/Popups/ChooseFaithGreatPerson.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0039}}<syntaxhighlight lang="lua">controlTable.Button:SetDisabled(true);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CityView.lua}}
:<code>UI/InGame/CityView/CityView.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0539}}<syntaxhighlight lang="lua">controlTable.BuildingButton:SetDisabled( true );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0542}}<syntaxhighlight lang="lua">controlTable.BuildingFilledSpecialistSlot2:SetDisabled( true );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0555}}<syntaxhighlight lang="lua">controlTable.BuildingEmptySpecialistSlot3:SetDisabled( false );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0711}}<syntaxhighlight lang="lua">Controls.NextCityButton:SetDisabled( true );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0713}}<syntaxhighlight lang="lua">Controls.PrevCityButton:SetDisabled( false );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1271}}<syntaxhighlight lang="lua">Controls.BuyPlotButton:SetDisabled(true);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1417}}<syntaxhighlight lang="lua">Controls.BalancedFocusButton:SetDisabled( true );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1420}}<syntaxhighlight lang="lua">Controls.GoldFocusButton:SetDisabled( true );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1425}}<syntaxhighlight lang="lua">Controls.ResetButton:SetDisabled( true );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1431}}<syntaxhighlight lang="lua">Controls.RazeCityButton:SetDisabled( true );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1445}}<syntaxhighlight lang="lua">Controls.ProductionFocusButton:SetDisabled( false );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1450}}<syntaxhighlight lang="lua">Controls.AvoidGrowthButton:SetDisabled( false );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CityView.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/CityView/CityView.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1477}}<syntaxhighlight lang="lua">Controls.FaithFocusButton:SetDisabled( false );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DiploList.lua}}
:<code>UI/InGame/DiploList.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0348}}<syntaxhighlight lang="lua">controlTable.LeaderButton:SetDisabled( true );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DiscussionDialog.lua}}
:<code>UI/InGame/LeaderHead/DiscussionDialog.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0170}}<syntaxhighlight lang="lua">Controls.Button3:SetDisabled(false);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DiscussionDialog.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/LeaderHead/DiscussionDialog.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1093}}<syntaxhighlight lang="lua">Controls.Button5:SetDisabled(true);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|EconomicGeneralInfo.lua}}
:<code>UI/InGame/Popups/EconomicGeneralInfo.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0271}}<syntaxhighlight lang="lua">Controls.TradeToggle:SetDisabled( true );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0341}}<syntaxhighlight lang="lua">Controls.BuildingsToggle:SetDisabled( true );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|EspionageOverview.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/Popups/EspionageOverview.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0685}}<syntaxhighlight lang="lua">agentEntry.RelocateButton:SetDisabled(v.State == "TXT_KEY_SPY_STATE_DEAD");</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|HappinessInfo.lua}}
:<code>UI/InGame/Popups/HappinessInfo.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0233}}<syntaxhighlight lang="lua">Controls.LuxuryHappinessToggle:SetDisabled( true );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0588}}<syntaxhighlight lang="lua">Controls.CityUnhappinessToggle:SetDisabled( false );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0722}}<syntaxhighlight lang="lua">Controls.ResourcesExportedToggle:SetDisabled( false );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0766}}<syntaxhighlight lang="lua">Controls.ResourcesLocalToggle:SetDisabled( true );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|LoadMenu.lua}}
:<code>UI/FrontEnd/LoadMenu.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0449}}<syntaxhighlight lang="lua">Controls.Delete:SetDisabled(true);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|Lobby.lua}}
:<code>UI/FrontEnd/Multiplayer/Lobby.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0152}}<syntaxhighlight lang="lua">Controls.HostButton:SetDisabled( true );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0169}}<syntaxhighlight lang="lua">Controls.RefreshButton:SetDisabled( false );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|MiniMapPanel.lua}}
:<code>UI/InGame/WorldView/MiniMapPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0042}}<syntaxhighlight lang="lua">Controls.ShowResources:SetDisabled( false );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|MPGameOptions.lua}}
:<code>UI/FrontEnd/Multiplayer/GameSetup/MPGameOptions.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0980}}<syntaxhighlight lang="lua">Controls.MaxTurnsCheck:SetDisabled( not bCanEdit );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|OptionsMenu.lua}}
:<code>UI/Options/OptionsMenu.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0319}}<syntaxhighlight lang="lua">Controls.MPQuickCombatCheckbox:SetDisabled( true );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0335}}<syntaxhighlight lang="lua">Controls.SpokenLanguagePull:SetDisabled(true);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|PlayerChange.lua}}
:<code>UI/InGame/PlayerChange.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0076}}<syntaxhighlight lang="lua">Controls.ContinueButton:SetDisabled( not bValid );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|SetCityName.lua}}
:<code>UI/InGame/Popups/SetCityName.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0087}}<syntaxhighlight lang="lua">Controls.AcceptButton:SetDisabled(not bValid);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|SocialPolicyPopup.lua}}
:<code>UI/InGame/Popups/SocialPolicyPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0364}}<syntaxhighlight lang="lua">thisButton:SetDisabled( true );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TradeLogic.lua}}
:<code>UI/InGame/WorldView/TradeLogic.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1044}}<syntaxhighlight lang="lua">Controls.UsPocketGoldPerTurn:SetDisabled(false);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1059}}<syntaxhighlight lang="lua">Controls.ThemPocketGoldPerTurn:SetDisabled(false);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1142}}<syntaxhighlight lang="lua">Controls.UsPocketDefensivePact:SetDisabled(true);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1247}}<syntaxhighlight lang="lua">Controls.UsPocketTradeAgreement:SetDisabled(false);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1258}}<syntaxhighlight lang="lua">Controls.ThemPocketTradeAgreement:SetDisabled(false);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1296}}<syntaxhighlight lang="lua">Controls.ThemPocketCities:SetDisabled( true );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1318}}<syntaxhighlight lang="lua">Controls.UsPocketOtherPlayer:SetDisabled( false );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1323}}<syntaxhighlight lang="lua">Controls.ThemPocketOtherPlayer:SetDisabled( false );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|2563}}<syntaxhighlight lang="lua">g_OtherPlayersButtons[ iLoopPlayer ][ SubTableName ].Button:SetDisabled( false );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TradeLogic.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/WorldView/TradeLogic.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1107}}<syntaxhighlight lang="lua">Controls.UsPocketAllowEmbassy:SetDisabled(false);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|UnitFlagManager.lua}}
:<code>UI/InGame/UnitFlagManager.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1594}}<syntaxhighlight lang="lua">pFlag.m_Instance.NormalButton:SetDisabled( false );</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|SetDisabled]]