{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of ControlBase.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''void''' UIElement:SetCheck<b>(</b>'''bool''' cityBanners<b>)</b></code>


'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|cityBanners:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Too many occurences. Only 50 out of 144 are listed.''

{{PseudoH4|AdvancedSetup.lua}}
:<code>UI/FrontEnd/GameSetup/AdvancedSetup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0918}}<syntaxhighlight lang="lua">Controls.MaxTurnsCheck:SetCheck(true);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|AdvisorModal.lua}}
:<code>UI/InGame/Popups/AdvisorModal.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0036}}<syntaxhighlight lang="lua">Controls.DontShowAgainCheckbox:SetCheck(false);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CityView.lua}}
:<code>UI/InGame/CityView/CityView.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0934}}<syntaxhighlight lang="lua">Controls.FoodFocusButton:SetCheck( true );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0938}}<syntaxhighlight lang="lua">Controls.GoldFocusButton:SetCheck( true );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0940}}<syntaxhighlight lang="lua">Controls.ResearchFocusButton:SetCheck( true );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0942}}<syntaxhighlight lang="lua">Controls.CultureFocusButton:SetCheck( true );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0944}}<syntaxhighlight lang="lua">Controls.GPFocusButton:SetCheck( true );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0948}}<syntaxhighlight lang="lua">Controls.AvoidGrowthButton:SetCheck( pCity:IsForcedAvoidGrowth() );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|2036}}<syntaxhighlight lang="lua">Controls.NoAutoSpecialistCheckbox:SetCheck(true);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DebugMenu.lua}}
:<code>UI/InGame/DebugMenu.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0163}}<syntaxhighlight lang="lua">Controls.ToggleUnitFlags_Checkbox:SetCheck( bUnitFlags );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DebugMode.lua}}
:<code>UI/InGame/DebugMode.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0574}}<syntaxhighlight lang="lua">Controls.UnitSpecRenderDiffuse_Checkbox:SetCheck( g_iUnitSpecularRender == 1 );</syntaxhighlight>
{{CodeLine5|0575}}<syntaxhighlight lang="lua">Controls.UnitSpecRenderSpecular_Checkbox:SetCheck( g_iUnitSpecularRender == 2 );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0602}}<syntaxhighlight lang="lua">Controls.UnitMemberFSMDebug_Checkbox:SetCheck( g_bUnitMemberFSMDebugCheck );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0665}}<syntaxhighlight lang="lua">Controls.UnitMemberSelectAll_Checkbox:SetCheck( false );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|InstalledPanel.lua}}
:<code>UI/FrontEnd/Modding/InstalledPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0852}}<syntaxhighlight lang="lua">Controls.ShowDLCMods:SetCheck(showDLCMods == "1");</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|LoadMenu.lua}}
:<code>UI/FrontEnd/LoadMenu.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0598}}<syntaxhighlight lang="lua">Controls.AutoCheck:SetCheck(g_ShowAutoSaves);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|MiniMapPanel.lua}}
:<code>UI/InGame/WorldView/MiniMapPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0169}}<syntaxhighlight lang="lua">Controls.ShowGrid:SetCheck( mapOptions.ShowGrid );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0172}}<syntaxhighlight lang="lua">Controls.HideRecommendation:SetCheck( mapOptions.HideTileRecommendations );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0176}}<syntaxhighlight lang="lua">Controls.ShowFogOfWar:SetCheck( mapOptions.SVShowFOW );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0327}}<syntaxhighlight lang="lua">Controls.ShowGrid:SetCheck( true );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0382}}<syntaxhighlight lang="lua">Controls.ShowYield:SetCheck( true );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0386}}<syntaxhighlight lang="lua">Controls.ShowYield:SetCheck( false );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0390}}<syntaxhighlight lang="lua">Controls.ShowResources:SetCheck( true );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0394}}<syntaxhighlight lang="lua">Controls.ShowResources:SetCheck( false );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|MPGameOptions.lua}}
:<code>UI/FrontEnd/Multiplayer/GameSetup/MPGameOptions.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0355}}<syntaxhighlight lang="lua">Controls.ScenarioCheck:SetCheck( loadScenarioChecked );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0882}}<syntaxhighlight lang="lua">victoryCondition.GameOptionRoot:SetCheck(PreGame.IsVictory(row.ID));</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0973}}<syntaxhighlight lang="lua">Controls.MaxTurnsCheck:SetCheck(false);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0992}}<syntaxhighlight lang="lua">dlcEntries.GameOptionRoot:SetCheck(PreGame.IsDLCAllowed(row.PackageID));</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|NetworkDebug.lua}}
:<code>UI/InGame/NetworkDebug.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0092}}<syntaxhighlight lang="lua">Controls.VerboseLoggingToggle:SetCheck(Network.GetDebugLogLevel() == 2);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|OptionsMenu.lua}}
:<code>UI/Options/OptionsMenu.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0637}}<syntaxhighlight lang="lua">Controls.AutoWorkersDontReplaceCB:SetCheck( OptionsManager.IsAutoWorkersDontReplace_Cached() );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0639}}<syntaxhighlight lang="lua">Controls.NoRewardPopupsCheckbox:SetCheck( OptionsManager.IsNoRewardPopups_Cached() );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0641}}<syntaxhighlight lang="lua">Controls.NoTileRecommendationsCheckbox:SetCheck( OptionsManager.IsNoTileRecommendations_Cached() );</syntaxhighlight>
{{CodeLine5|0642}}<syntaxhighlight lang="lua">Controls.CivilianYieldsCheckbox:SetCheck( OptionsManager.IsCivilianYields_Cached() );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0644}}<syntaxhighlight lang="lua">Controls.MultiplayerAutoEndTurnCheckbox:SetCheck(OptionsManager.GetMultiplayerAutoEndTurnEnabled_Cached());</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0649}}<syntaxhighlight lang="lua">Controls.SPQuickMovementCheckBox:SetCheck(OptionsManager.GetSinglePlayerQuickMovementEnabled_Cached());</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0653}}<syntaxhighlight lang="lua">Controls.SPQuickCombatCheckBox:SetCheck(m_bInGameQuickCombatState_Cached);</syntaxhighlight>
{{CodeLine5|0654}}<syntaxhighlight lang="lua">Controls.SPQuickMovementCheckBox:SetCheck(m_bInGameQuickMovementState_Cached);</syntaxhighlight>
{{CodeLine5|0655}}<syntaxhighlight lang="lua">Controls.MPQuickCombatCheckbox:SetCheck(OptionsManager.GetMultiplayerQuickCombatEnabled_Cached());</syntaxhighlight>
{{CodeLine5|0656}}<syntaxhighlight lang="lua">Controls.MPQuickMovementCheckbox:SetCheck(OptionsManager.GetMultiplayerQuickMovementEnabled_Cached());</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0669}}<syntaxhighlight lang="lua">Controls.PolicyInfo:SetCheck( OptionsManager.GetPolicyInfo_Cached() );</syntaxhighlight>
{{CodeLine5|0670}}<syntaxhighlight lang="lua">Controls.AutoUnitCycleCheck:SetCheck( OptionsManager.GetAutoUnitCycle_Cached() );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0699}}<syntaxhighlight lang="lua">Controls.SmallUIAssetsCheck:SetCheck( false );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0703}}<syntaxhighlight lang="lua">Controls.AutoUIAssetsCheck:SetCheck( false );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0709}}<syntaxhighlight lang="lua">Controls.SkipIntroVideoCheck:SetCheck( OptionsManager.GetSkipIntroVideo_Cached() );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ReplayViewer.lua}}
:<code>UI/InGame/Popups/ReplayViewer.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0729}}<syntaxhighlight lang="lua">graphLegendInstance.ShowHide:SetCheck(checked);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|SetCivNames.lua}}
:<code>UI/FrontEnd/GameSetup/SetCivNames.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0245}}<syntaxhighlight lang="lua">Controls.UsePasswordCheck:SetCheck( name ~= "" );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|StagingRoom.lua}}
:<code>UI/FrontEnd/Multiplayer/StagingRoom.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0419}}<syntaxhighlight lang="lua">slotInstance.EnableCheck:SetCheck( false );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0430}}<syntaxhighlight lang="lua">slotInstance.LockCheck:SetCheck( false );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TerrainPanel.lua}}
:<code>UI/InGame/TerrainPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0031}}<syntaxhighlight lang="lua">Controls.WaterAutoReload_Checkbox:SetCheck(g_bWaterReload);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0045}}<syntaxhighlight lang="lua">Controls.WaterAutoReload_Checkbox:SetCheck(g_iWaterReload);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|SetCheck]]