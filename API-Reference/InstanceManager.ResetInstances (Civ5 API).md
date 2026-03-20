{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|InstanceManager}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''void''' InstanceManager:ResetInstances<b>(</b><b>)</b></code>




=Source code samples=
''Too many occurences. Only 50 out of 570 are listed.''

{{PseudoH4|AdvisorInfoPopup.lua}}
:<code>UI/InGame/Popups/AdvisorInfoPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0103}}<syntaxhighlight lang="lua">g_InstanceManager:ResetInstances();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ChooseReligionPopup.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/Popups/ChooseReligionPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0268}}<syntaxhighlight lang="lua">g_ReligionButtonManager:ResetInstances();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CityView.lua}}
:<code>UI/InGame/CityView/CityView.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0913}}<syntaxhighlight lang="lua">g_BuildingIM:ResetInstances();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0915}}<syntaxhighlight lang="lua">g_SlackerIM:ResetInstances();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0917}}<syntaxhighlight lang="lua">g_BuyPlotButtonIM:ResetInstances();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CivilopediaScreen.lua}}
:<code>UI/Civilopedia/CivilopediaScreen.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0142}}<syntaxhighlight lang="lua">g_ListItemManager:ResetInstances();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1319}}<syntaxhighlight lang="lua">g_BBTextManager:ResetInstances();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|2018}}<syntaxhighlight lang="lua">g_PrereqTechManager:ResetInstances();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|2036}}<syntaxhighlight lang="lua">g_LeadsToTechManager:ResetInstances();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|2101}}<syntaxhighlight lang="lua">g_UnlockedProjectsManager:ResetInstances();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|2122}}<syntaxhighlight lang="lua">g_RevealedResourcesManager:ResetInstances();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|2468}}<syntaxhighlight lang="lua">g_ObsoleteTechManager:ResetInstances();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|2489}}<syntaxhighlight lang="lua">g_UpgradeManager:ResetInstances();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|2531}}<syntaxhighlight lang="lua">g_ReplacesManager:ResetInstances();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|2639}}<syntaxhighlight lang="lua">g_RequiredPromotionsManager:ResetInstances();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|2927}}<syntaxhighlight lang="lua">g_RequiredBuildingsManager:ResetInstances();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|3569}}<syntaxhighlight lang="lua">g_UniqueImprovementsManager:ResetInstances();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|3938}}<syntaxhighlight lang="lua">g_FeaturesManager:ResetInstances();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|3959}}<syntaxhighlight lang="lua">g_ResourcesFoundManager:ResetInstances();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DiploList.lua}}
:<code>UI/InGame/DiploList.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0183}}<syntaxhighlight lang="lua">g_LeaderButtonIM:ResetInstances();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DiploRelationships.lua}}
:<code>UI/InGame/Popups/DiploRelationships.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0115}}<syntaxhighlight lang="lua">g_MajorCivButtonIM:ResetInstances();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|EnemyUnitPanel.lua}}
:<code>UI/InGame/WorldView/EnemyUnitPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0283}}<syntaxhighlight lang="lua">g_MyCombatDataIM:ResetInstances();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|GameMenu.lua}}
:<code>UI/InGame/Menus/GameMenu.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0306}}<syntaxhighlight lang="lua">g_GameOptionIM:ResetInstances();</syntaxhighlight>
{{CodeLine5|0307}}<syntaxhighlight lang="lua">g_VictoryConditionsIM:ResetInstances();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0439}}<syntaxhighlight lang="lua">g_ActivatedModsIM:ResetInstances();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|GPList.lua}}
:<code>UI/InGame/GPList.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0083}}<syntaxhighlight lang="lua">m_EngineerIM:ResetInstances();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0085}}<syntaxhighlight lang="lua">m_ScientistIM:ResetInstances();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|HallOfFame.lua}}
:<code>UI/InGame/Popups/HallOfFame.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0022}}<syntaxhighlight lang="lua">g_GamesIM:ResetInstances();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|InstalledPanel.lua}}
:<code>UI/FrontEnd/Modding/InstalledPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0360}}<syntaxhighlight lang="lua">g_DependentMods:ResetInstances();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0526}}<syntaxhighlight lang="lua">g_DetailsDependentMods:ResetInstances();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|MilitaryOverview.lua}}
:<code>UI/InGame/Popups/MilitaryOverview.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0139}}<syntaxhighlight lang="lua">m_MilitaryIM:ResetInstances();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|NetworkDebug.lua}}
:<code>UI/InGame/NetworkDebug.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0007}}<syntaxhighlight lang="lua">g_PlayerSliceInfoIM:ResetInstances();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ProductionPopup.lua}}
:<code>UI/InGame/Popups/ProductionPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0129}}<syntaxhighlight lang="lua">g_UnitInstanceManager:ResetInstances();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0131}}<syntaxhighlight lang="lua">g_WonderInstanceManager:ResetInstances();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|Ranking.lua}}
:<code>UI/InGame/Popups/Ranking.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0014}}<syntaxhighlight lang="lua">g_RankIM:ResetInstances();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ReligionOverview.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/Popups/ReligionOverview.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0480}}<syntaxhighlight lang="lua">g_WorldReligionsManager:ResetInstances();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0565}}<syntaxhighlight lang="lua">g_BeliefsManager:ResetInstances();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ReplayViewer.lua}}
:<code>UI/InGame/Popups/ReplayViewer.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0401}}<syntaxhighlight lang="lua">g_LineSegmentInstanceManager:ResetInstances();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0707}}<syntaxhighlight lang="lua">g_GraphLegendInstanceManager:ResetInstances();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ResourceList.lua}}
:<code>UI/InGame/ResourceList.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0079}}<syntaxhighlight lang="lua">m_LuxuryIM:ResetInstances();</syntaxhighlight>
{{CodeLine5|0080}}<syntaxhighlight lang="lua">m_BonusIM:ResetInstances();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TaskList.lua}}
:<code>UI/InGame/TaskList.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0023}}<syntaxhighlight lang="lua">g_TaskItemManager:ResetInstances();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TechPopup.lua}}
:<code>UI/InGame/TechPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0089}}<syntaxhighlight lang="lua">g_TechInstanceManager:ResetInstances();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TradeLogic.lua}}
:<code>UI/InGame/WorldView/TradeLogic.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1506}}<syntaxhighlight lang="lua">g_ThemTableCitiesIM:ResetInstances();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|UnitPanel.lua}}
:<code>UI/InGame/WorldView/UnitPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0137}}<syntaxhighlight lang="lua">g_PromotionIM:ResetInstances();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0511}}<syntaxhighlight lang="lua">g_EarnedPromotionIM:ResetInstances();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|VictoryProgress.lua}}
:<code>UI/InGame/Popups/VictoryProgress.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0198}}<syntaxhighlight lang="lua">g_DominationRowsIM:ResetInstances();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0430}}<syntaxhighlight lang="lua">g_CultureIM:ResetInstances();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0505}}<syntaxhighlight lang="lua">g_ScoreIM:ResetInstances();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0651}}<syntaxhighlight lang="lua">g_DiploIM:ResetInstances();</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|ResetInstances]]