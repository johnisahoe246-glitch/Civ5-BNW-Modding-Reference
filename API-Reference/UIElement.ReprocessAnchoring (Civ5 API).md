{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This method is declared by '''ControlBase'''.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''void''' UIElement:ReprocessAnchoring<b>(</b><b>)</b></code>




=Source code samples=
''Too many occurences. Only 50 out of 346 are listed.''

{{PseudoH4|AdvancedSetup.lua}}
:<code>UI/FrontEnd/GameSetup/AdvancedSetup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0152}}<syntaxhighlight lang="lua">Controls.DropDownOptionsStack:ReprocessAnchoring();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0245}}<syntaxhighlight lang="lua">Controls.MaxTurnStack:ReprocessAnchoring();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|AdvisorInfoPopup.lua}}
:<code>UI/InGame/Popups/AdvisorInfoPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0131}}<syntaxhighlight lang="lua">Controls.RelatedConceptButtonStack:ReprocessAnchoring();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ChoosePantheonPopup.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/Popups/ChoosePantheonPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0034}}<syntaxhighlight lang="lua">Controls.BottomPanel:ReprocessAnchoring();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ChooseReligionPopup.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/Popups/ChooseReligionPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0531}}<syntaxhighlight lang="lua">Controls.BeliefStack:ReprocessAnchoring();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CityBannerManager.lua}}
:<code>UI/InGame/CityBannerManager.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0222}}<syntaxhighlight lang="lua">controls.IconsStack:ReprocessAnchoring();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0783}}<syntaxhighlight lang="lua">BannerInstance.BannerButton:ReprocessAnchoring();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CityStateDiploPopup.lua}}
:<code>UI/InGame/Popups/CityStateDiploPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0804}}<syntaxhighlight lang="lua">Controls.GoldGiftStack:ReprocessAnchoring();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CityView.lua}}
:<code>UI/InGame/CityView/CityView.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0729}}<syntaxhighlight lang="lua">Controls.TitleStack:ReprocessAnchoring();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1257}}<syntaxhighlight lang="lua">Controls.WorkerManagementBox:ReprocessAnchoring();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CivilopediaScreen.lua}}
:<code>UI/Civilopedia/CivilopediaScreen.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1291}}<syntaxhighlight lang="lua">Controls.WideStack:ReprocessAnchoring();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1293}}<syntaxhighlight lang="lua">Controls.FFTextStack:ReprocessAnchoring();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1297}}<syntaxhighlight lang="lua">Controls.SuperWideStack:ReprocessAnchoring();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DiploCorner.lua}}
:<code>UI/InGame/WorldView/DiploCorner.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0172}}<syntaxhighlight lang="lua">controlTable.Box:ReprocessAnchoring();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DiploRelationships.lua}}
:<code>UI/InGame/Popups/DiploRelationships.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0109}}<syntaxhighlight lang="lua">Controls.MinorButtonStack:ReprocessAnchoring();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0212}}<syntaxhighlight lang="lua">controlTable.TradeStack:ReprocessAnchoring();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|EconomicGeneralInfo.lua}}
:<code>UI/InGame/Popups/EconomicGeneralInfo.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0345}}<syntaxhighlight lang="lua">Controls.BuildingsStack:ReprocessAnchoring();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|EspionageOverview.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/Popups/EspionageOverview.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0775}}<syntaxhighlight lang="lua">agentEntry.AgentActivitiesStack:ReprocessAnchoring();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0780}}<syntaxhighlight lang="lua">Controls.AgentStack:ReprocessAnchoring();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1076}}<syntaxhighlight lang="lua">Controls.MyCityStack:ReprocessAnchoring();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1499}}<syntaxhighlight lang="lua">Controls.IntrigueMessageStack:ReprocessAnchoring();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|FoRScenarioLoadScreen.lua (G&K)}}
:<code>DLC/Expansion/Scenarios/FallOfRomeScenario/FoRScenarioLoadScreen.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0115}}<syntaxhighlight lang="lua">Controls.DifficultyStack:ReprocessAnchoring();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|GameMenu.lua}}
:<code>UI/InGame/Menus/GameMenu.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0430}}<syntaxhighlight lang="lua">Controls.OptionsStack:ReprocessAnchoring();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|GPList.lua}}
:<code>UI/InGame/GPList.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0178}}<syntaxhighlight lang="lua">Controls.ArtistStack:ReprocessAnchoring();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0184}}<syntaxhighlight lang="lua">Controls.ScientistStack:ReprocessAnchoring();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|HallOfFame.lua}}
:<code>UI/InGame/Popups/HallOfFame.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0168}}<syntaxhighlight lang="lua">controlTable.IconStack:ReprocessAnchoring();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0171}}<syntaxhighlight lang="lua">controlTable.SettingStack:ReprocessAnchoring();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0182}}<syntaxhighlight lang="lua">Controls.GameStack:ReprocessAnchoring();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|HappinessInfo.lua}}
:<code>UI/InGame/Popups/HappinessInfo.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0090}}<syntaxhighlight lang="lua">Controls.UnhappinessStack:ReprocessAnchoring();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0293}}<syntaxhighlight lang="lua">Controls.CityBuildingStack:ReprocessAnchoring();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0595}}<syntaxhighlight lang="lua">Controls.CityUnhappinessStack:ReprocessAnchoring();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0646}}<syntaxhighlight lang="lua">Controls.ResourcesAvailableStack:ReprocessAnchoring();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0770}}<syntaxhighlight lang="lua">Controls.ResourcesLocalStack:ReprocessAnchoring();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|HappinessInfo.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/Popups/HappinessInfo.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0351}}<syntaxhighlight lang="lua">Controls.LocalCityStack:ReprocessAnchoring();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|InstalledPanel.lua}}
:<code>UI/FrontEnd/Modding/InstalledPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0335}}<syntaxhighlight lang="lua">Controls.ListingStack:ReprocessAnchoring();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|MiniMapPanel.lua}}
:<code>UI/InGame/WorldView/MiniMapPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0060}}<syntaxhighlight lang="lua">Controls.SideStack:ReprocessAnchoring();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|NotificationLogPopup.lua}}
:<code>UI/InGame/Popups/NotificationLogPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0036}}<syntaxhighlight lang="lua">Controls.NotificationButtonStack:ReprocessAnchoring();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|OptionsMenu.lua}}
:<code>UI/Options/OptionsMenu.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0228}}<syntaxhighlight lang="lua">Controls.LabelStack:ReprocessAnchoring();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|PlotHelpText.lua}}
:<code>UI/InGame/WorldView/PlotHelpText.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0073}}<syntaxhighlight lang="lua">Controls.TextBox:ReprocessAnchoring();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|Ranking.lua}}
:<code>UI/InGame/Popups/Ranking.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0043}}<syntaxhighlight lang="lua">controlTable.MyStack:ReprocessAnchoring();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ReplayViewer.lua}}
:<code>UI/InGame/Popups/ReplayViewer.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0750}}<syntaxhighlight lang="lua">Controls.GraphLegendStack:ReprocessAnchoring();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ResourceList.lua}}
:<code>UI/InGame/ResourceList.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0154}}<syntaxhighlight lang="lua">Controls.LuxuryStack:ReprocessAnchoring();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|SelectCivilization.lua}}
:<code>UI/FrontEnd/GameSetup/SelectCivilization.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0237}}<syntaxhighlight lang="lua">Controls.Stack:ReprocessAnchoring();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TradeLogic.lua}}
:<code>UI/InGame/WorldView/TradeLogic.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1589}}<syntaxhighlight lang="lua">Controls.UsTablePanel:ReprocessAnchoring();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1850}}<syntaxhighlight lang="lua">Controls.UsTableDeclareWarStack:ReprocessAnchoring();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1856}}<syntaxhighlight lang="lua">Controls.ThemTableDeclareWarStack:ReprocessAnchoring();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|UnitList.lua}}
:<code>UI/InGame/UnitList.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0228}}<syntaxhighlight lang="lua">instance.UnitStack:ReprocessAnchoring();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|UnitPanel.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/WorldView/UnitPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0321}}<syntaxhighlight lang="lua">Controls.SecondaryStack:ReprocessAnchoring();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|VictoryProgress.lua}}
:<code>UI/InGame/Popups/VictoryProgress.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0805}}<syntaxhighlight lang="lua">Controls.CultureCivs:ReprocessAnchoring();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|VoteResultsPopup.lua}}
:<code>UI/InGame/Popups/VoteResultsPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0250}}<syntaxhighlight lang="lua">Controls.PlayerListStack:ReprocessAnchoring();</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|ReprocessAnchoring]]