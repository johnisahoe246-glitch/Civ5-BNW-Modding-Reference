{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|InstanceManager}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>{{Type5|InstanceManager}} InstanceManager:new<b>(</b>'''string''' instanceName, '''string''' instanceRootName, '''ControlBase''' hostControl<b>)</b></code>


'''Returned Value'''
:No description available.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|instanceName:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|instanceRootName:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|hostControl:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Too many occurences. Only 50 out of 335 are listed.''

{{PseudoH4|AdvancedSetup.lua}}
:<code>UI/FrontEnd/GameSetup/AdvancedSetup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0031}}<syntaxhighlight lang="lua">g_GameOptionsManager = InstanceManager:new("GameOptionInstance", "GameOptionRoot", Controls.GameOptionsStack);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ChoosePantheonPopup.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/Popups/ChoosePantheonPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0012}}<syntaxhighlight lang="lua">local g_ItemManager = InstanceManager:new( "ItemInstance", "Button", Controls.ItemStack );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ChooseReligionPopup.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/Popups/ChooseReligionPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0010}}<syntaxhighlight lang="lua">local g_BeliefItemManager = InstanceManager:new( "BeliefItemInstance", "Button", Controls.BeliefStack );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CityBannerManager.lua}}
:<code>UI/InGame/CityBannerManager.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0009}}<syntaxhighlight lang="lua">local g_SVStrikeIM = InstanceManager:new( "SVRangeStrikeButton", "Anchor", Controls.StrategicViewStrikeButtons );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CityView.lua}}
:<code>UI/InGame/CityView/CityView.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0008}}<syntaxhighlight lang="lua">local g_BuildingIM   = InstanceManager:new( "BuildingInstance", "BuildingButton", Controls.BuildingStack );</syntaxhighlight>
{{CodeLine5|0009}}<syntaxhighlight lang="lua">local g_GPIM   = InstanceManager:new( "GPInstance", "GPBox", Controls.GPStack );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CivilopediaScreen.lua}}
:<code>UI/Civilopedia/CivilopediaScreen.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0075}}<syntaxhighlight lang="lua">local g_ListItemManager = InstanceManager:new( "ListItemInstance", "ListItemButton", Controls.ListOfArticles );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0079}}<syntaxhighlight lang="lua">local g_UpgradeManager = InstanceManager:new( "UpgradeInstance", "UpgradeButton", Controls.UpgradeInnerFrame );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0082}}<syntaxhighlight lang="lua">local g_UnlockedBuildingsManager = InstanceManager:new( "UnlockedBuildingInstance", "UnlockedBuildingButton", Controls.UnlockedBuildingsInnerFrame );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0091}}<syntaxhighlight lang="lua">local g_RequiredPromotionsManager = InstanceManager:new( "RequiredPromotionInstance", "RequiredPromotionButton", Controls.RequiredPromotionsInnerFrame );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0093}}<syntaxhighlight lang="lua">local g_FreeFormTextManager = InstanceManager:new( "FreeFormTextInstance", "FFTextFrame", Controls.FFTextStack );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0097}}<syntaxhighlight lang="lua">local g_UniqueBuildingsManager = InstanceManager:new( "UniqueBuildingInstance", "UniqueBuildingButton", Controls.UniqueBuildingsInnerFrame );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0101}}<syntaxhighlight lang="lua">local g_FeaturesManager = InstanceManager:new( "FeatureInstance", "FeatureButton", Controls.FeaturesInnerFrame );</syntaxhighlight>
{{CodeLine5|0102}}<syntaxhighlight lang="lua">local g_ResourcesFoundManager = InstanceManager:new( "ResourceFoundInstance", "ResourceFoundButton", Controls.ResourcesFoundInnerFrame );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0104}}<syntaxhighlight lang="lua">local g_ReplacesManager = InstanceManager:new( "ReplaceInstance", "ReplaceButton", Controls.ReplacesInnerFrame );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0106}}<syntaxhighlight lang="lua">local g_ImprovementsManager = InstanceManager:new( "ImprovementInstance", "ImprovementButton", Controls.ImprovementsInnerFrame );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|Credits.lua}}
:<code>UI/FrontEnd/Credits.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0005}}<syntaxhighlight lang="lua">g_MajorTitleManager = InstanceManager:new("MajorTitleInstance", "Text", Controls.CreditsList);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DiploList.lua}}
:<code>UI/InGame/DiploList.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0014}}<syntaxhighlight lang="lua">local g_LeaderButtonIM = InstanceManager:new( "LeaderButtonInstance", "LeaderButton", Controls.MajorStack );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DiploRelationships.lua}}
:<code>UI/InGame/Popups/DiploRelationships.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0266}}<syntaxhighlight lang="lua">local g_MajorCivTradeRowIM = InstanceManager:new( "MajorCivTradeRowInstance", "Row", pStack.TradeStack );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|EndGameReplay.lua}}
:<code>UI/InGame/Popups/EndGameReplay.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0008}}<syntaxhighlight lang="lua">g_ReplayMessageInstanceManager = InstanceManager:new("ReplayMessageInstance", "MessageText", Controls.ReplayMessageStack);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|EnemyUnitPanel.lua}}
:<code>UI/InGame/WorldView/EnemyUnitPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0006}}<syntaxhighlight lang="lua">local g_MyCombatDataIM = InstanceManager:new( "UsCombatInfo", "Text", Controls.MyCombatResultsStack );</syntaxhighlight>
{{CodeLine5|0007}}<syntaxhighlight lang="lua">local g_TheirCombatDataIM = InstanceManager:new( "ThemCombatInfo", "Text", Controls.TheirCombatResultsStack );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|GameMenu.lua}}
:<code>UI/InGame/Menus/GameMenu.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0009}}<syntaxhighlight lang="lua">local g_VictoryConditionsIM = InstanceManager:new( "GameOption", "Text", Controls.VictoryConditions );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0015}}<syntaxhighlight lang="lua">local g_ActivatedModsIM = InstanceManager:new( "ModEntryInstance", "Text", Controls.ModsStack );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|GPList.lua}}
:<code>UI/InGame/GPList.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0014}}<syntaxhighlight lang="lua">local m_ArtistIM = InstanceManager:new( "GPInstance", "Root", Controls.ArtistStack );</syntaxhighlight>
{{CodeLine5|0015}}<syntaxhighlight lang="lua">local m_EngineerIM = InstanceManager:new( "GPInstance", "Root", Controls.EngineerStack );</syntaxhighlight>
{{CodeLine5|0016}}<syntaxhighlight lang="lua">local m_MerchantIM = InstanceManager:new( "GPInstance", "Root", Controls.MerchantStack );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|InGame.lua}}
:<code>UI/InGame/InGame.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0013}}<syntaxhighlight lang="lua">local g_InstanceManager = InstanceManager:new( "AlertMessageInstance", "AlertMessageLabel", Controls.AlertStack );</syntaxhighlight>
{{CodeLine5|0014}}<syntaxhighlight lang="lua">local g_PopupIM = InstanceManager:new( "PopupText", "Anchor", Controls.PopupTextContainer );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|InstalledPanel.lua}}
:<code>UI/FrontEnd/Modding/InstalledPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0069}}<syntaxhighlight lang="lua">g_DetailLabels = InstanceManager:new("DetailLabelInstance", "Label", Controls.DetailLabelsStack);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|MiniMapPanel.lua}}
:<code>UI/InGame/WorldView/MiniMapPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0004}}<syntaxhighlight lang="lua">local g_LegendIM = InstanceManager:new( "LegendKey", "Item", Controls.LegendStack );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ModsMenu.lua}}
:<code>UI/FrontEnd/Modding/ModsMenu.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0006}}<syntaxhighlight lang="lua">g_InstanceManager = InstanceManager:new( "ModInstance", "Label", Controls.ModsStack );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|MPGameOptions.lua}}
:<code>UI/FrontEnd/Multiplayer/GameSetup/MPGameOptions.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0007}}<syntaxhighlight lang="lua">g_DLCAllowedManager = InstanceManager:new("GameOptionInstance", "GameOptionRoot", Controls.DLCAllowedStack);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|PreGameScreen.lua}}
:<code>UI/FrontEnd/PreGameScreen.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0001}}<syntaxhighlight lang="lua">local g_InstanceManager = InstanceManager:new( "LeaderButtonInstance", "LeaderButton", Controls.ButtonStack );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|PremiumContentMenu.lua}}
:<code>UI/FrontEnd/PremiumContentMenu.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0005}}<syntaxhighlight lang="lua">g_InstanceManager = InstanceManager:new( "ListingButtonInstance", "Base", Controls.ListingStack );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|SocialPolicyPopup.lua}}
:<code>UI/InGame/Popups/SocialPolicyPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0014}}<syntaxhighlight lang="lua">local g_PatronagePipeManager = InstanceManager:new( "ConnectorPipe", "ConnectorImage", Controls.PatronagePanel );</syntaxhighlight>
{{CodeLine5|0015}}<syntaxhighlight lang="lua">local g_CommercePipeManager = InstanceManager:new( "ConnectorPipe", "ConnectorImage", Controls.CommercePanel );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0018}}<syntaxhighlight lang="lua">local g_OrderPipeManager = InstanceManager:new( "ConnectorPipe", "ConnectorImage", Controls.OrderPanel );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0022}}<syntaxhighlight lang="lua">local g_TraditionInstanceManager = InstanceManager:new( "PolicyButton", "PolicyIcon", Controls.TraditionPanel );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0027}}<syntaxhighlight lang="lua">local g_RationalismInstanceManager = InstanceManager:new( "PolicyButton", "PolicyIcon", Controls.RationalismPanel );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|SocialPolicyPopup.lua (G&K)}}
:<code>DLC/Expansion/Scenarios/SteampunkScenario/SocialPolicyPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0016}}<syntaxhighlight lang="lua">local g_CulturePipeManager = InstanceManager:new( "ConnectorPipe", "ConnectorImage", Controls.CulturePanel );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0019}}<syntaxhighlight lang="lua">local g_MilitaryPipeManager = InstanceManager:new( "ConnectorPipe", "ConnectorImage", Controls.MilitaryPanel );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TechTree.lua}}
:<code>UI/InGame/TechTree/TechTree.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0012}}<syntaxhighlight lang="lua">local g_PipeManager = InstanceManager:new( "TechPipeInstance", "TechPipeIcon", Controls.TechTreeScrollPanel );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|UnitFlagManager.lua}}
:<code>UI/InGame/UnitFlagManager.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0005}}<syntaxhighlight lang="lua">local g_CivilianManager = InstanceManager:new( "NewUnitFlag", "Anchor", Controls.CivilianFlags );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|UnitPanel.lua}}
:<code>UI/InGame/WorldView/UnitPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0007}}<syntaxhighlight lang="lua">local g_SecondaryIM  = InstanceManager:new( "UnitAction",  "UnitActionButton", Controls.SecondaryStack );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0009}}<syntaxhighlight lang="lua">local g_PromotionIM  = InstanceManager:new( "UnitAction",  "UnitActionButton", Controls.WorkerActionPanel );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|VictoryProgress.lua}}
:<code>UI/InGame/Popups/VictoryProgress.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0007}}<syntaxhighlight lang="lua">local g_DominationRowsIM = InstanceManager:new( "DominationRow", "RowStack", Controls.DominationStack );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0023}}<syntaxhighlight lang="lua">local g_TechIM = InstanceManager:new( "TechCiv", "Civ", Controls.TechStack );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0785}}<syntaxhighlight lang="lua">curItemIM = InstanceManager:new( "CultureItem", "Item", controlTable.CultureStack );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|YieldIconManager.lua}}
:<code>UI/InGame/YieldIconManager.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0007}}<syntaxhighlight lang="lua">local g_AnchorIM = InstanceManager:new( "AnchorInstance", "Anchor", Controls.Scrap );</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|new]]