{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|InstanceManager}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''unknown''' InstanceManager:GetInstance<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
''Too many occurences. Only 50 out of 953 are listed.''

{{PseudoH4|AdvancedSetup.lua}}
:<code>UI/FrontEnd/GameSetup/AdvancedSetup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0088}}<syntaxhighlight lang="lua">local gameOption = g_DropDownOptionsManager:GetInstance();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CityBannerManager.lua}}
:<code>UI/InGame/CityBannerManager.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0601}}<syntaxhighlight lang="lua">controlTable = g_TeamIM:GetInstance();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CityView.lua}}
:<code>UI/InGame/CityView/CityView.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0290}}<syntaxhighlight lang="lua">local controlTable = g_BuildingIM:GetInstance();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1734}}<syntaxhighlight lang="lua">local controlTable = g_PlotButtonIM:GetInstance();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CivilopediaScreen.lua}}
:<code>UI/Civilopedia/CivilopediaScreen.lua</code>
:{{CodeBegin5}}
{{CodeLine5|2058}}<syntaxhighlight lang="lua">local thisUnitInstance = g_UnlockedUnitsManager:GetInstance();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|2076}}<syntaxhighlight lang="lua">local thisBuildingInstance = g_UnlockedBuildingsManager:GetInstance();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|2125}}<syntaxhighlight lang="lua">local thisRevealedResourceInstance = g_RevealedResourcesManager:GetInstance();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|2644}}<syntaxhighlight lang="lua">local thisRequiredPromotionInstance = g_RequiredPromotionsManager:GetInstance();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|3021}}<syntaxhighlight lang="lua">local thisBuildingInstance = g_ReplacesManager:GetInstance();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|3572}}<syntaxhighlight lang="lua">local thisImprovementInstance = g_UniqueImprovementsManager:GetInstance();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|4179}}<syntaxhighlight lang="lua">local thisPrereqInstance = g_RevealTechsManager:GetInstance();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|4231}}<syntaxhighlight lang="lua">local thisTerrainInstance = g_ResourcesFoundManager:GetInstance();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|4617}}<syntaxhighlight lang="lua">local thisListInstance = g_ListItemManager:GetInstance();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|4630}}<syntaxhighlight lang="lua">local thisHeaderInstance = g_ListHeadingManager:GetInstance();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|4678}}<syntaxhighlight lang="lua">local thisTechInstance = g_ListItemManager:GetInstance();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|4692}}<syntaxhighlight lang="lua">local thisEraInstance = g_ListHeadingManager:GetInstance();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|Credits.lua}}
:<code>UI/FrontEnd/Credits.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0070}}<syntaxhighlight lang="lua">local majorTitle = g_MajorTitleManager:GetInstance();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0079}}<syntaxhighlight lang="lua">local entry = g_EntryManager:GetInstance();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DiploList.lua}}
:<code>UI/InGame/DiploList.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0256}}<syntaxhighlight lang="lua">local controlTable = g_LeaderButtonIM:GetInstance();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0432}}<syntaxhighlight lang="lua">local controlTable = g_MinorCivButtonIM:GetInstance();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DiscussionDialog.lua}}
:<code>UI/InGame/LeaderHead/DiscussionDialog.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0920}}<syntaxhighlight lang="lua">instanceControls = g_InstanceManager:GetInstance();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|GameMenu.lua}}
:<code>UI/InGame/Menus/GameMenu.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0339}}<syntaxhighlight lang="lua">local controlTable = g_GameOptionIM:GetInstance();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|InstalledPanel.lua}}
:<code>UI/FrontEnd/Modding/InstalledPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0565}}<syntaxhighlight lang="lua">local detail = g_DetailsDependentMods:GetInstance();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|MilitaryOverview.lua}}
:<code>UI/InGame/Popups/MilitaryOverview.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0148}}<syntaxhighlight lang="lua">instance = m_MilitaryIM:GetInstance();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0151}}<syntaxhighlight lang="lua">instance = m_CivilianIM:GetInstance();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|NetworkDebug.lua}}
:<code>UI/InGame/NetworkDebug.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0012}}<syntaxhighlight lang="lua">local item = g_PlayerSliceInfoIM:GetInstance();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|PathHelpManager.lua}}
:<code>UI/InGame/WorldView/PathHelpManager.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0030}}<syntaxhighlight lang="lua">local instance = m_InstanceManager:GetInstance();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ReplayViewer.lua}}
:<code>UI/InGame/Popups/ReplayViewer.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0436}}<syntaxhighlight lang="lua">local lineSegment = g_LineSegmentInstanceManager:GetInstance();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|SaveMenu.lua}}
:<code>UI/InGame/Menus/SaveMenu.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0508}}<syntaxhighlight lang="lua">local instance = g_InstanceManager:GetInstance();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|SocialPolicyPopup.lua}}
:<code>UI/InGame/Popups/SocialPolicyPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0583}}<syntaxhighlight lang="lua">controlTable = g_TraditionPipeManager:GetInstance();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0589}}<syntaxhighlight lang="lua">controlTable = g_PatronagePipeManager:GetInstance();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0595}}<syntaxhighlight lang="lua">controlTable = g_FreedomPipeManager:GetInstance();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0872}}<syntaxhighlight lang="lua">controlTable = g_CommerceInstanceManager:GetInstance();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0874}}<syntaxhighlight lang="lua">controlTable = g_RationalismInstanceManager:GetInstance();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0878}}<syntaxhighlight lang="lua">controlTable = g_OrderInstanceManager:GetInstance();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0880}}<syntaxhighlight lang="lua">controlTable = g_AutocracyInstanceManager:GetInstance();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|SocialPolicyPopup.lua (G&K)}}
:<code>DLC/Expansion/Scenarios/SteampunkScenario/SocialPolicyPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0389}}<syntaxhighlight lang="lua">controlTable = g_LaborPipeManager:GetInstance();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0391}}<syntaxhighlight lang="lua">controlTable = g_CulturePipeManager:GetInstance();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0648}}<syntaxhighlight lang="lua">controlTable = g_IndustryInstanceManager:GetInstance();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0652}}<syntaxhighlight lang="lua">controlTable = g_MilitaryInstanceManager:GetInstance();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TechTree.lua}}
:<code>UI/InGame/TechTree/TechTree.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0151}}<syntaxhighlight lang="lua">local hConnection = g_PipeManager:GetInstance();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0159}}<syntaxhighlight lang="lua">local vConnection = g_PipeManager:GetInstance();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0201}}<syntaxhighlight lang="lua">local startPipe = g_PipeManager:GetInstance();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0206}}<syntaxhighlight lang="lua">local pipe = g_PipeManager:GetInstance();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0220}}<syntaxhighlight lang="lua">pipe = g_PipeManager:GetInstance();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TradeLogic.lua}}
:<code>UI/InGame/WorldView/TradeLogic.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1712}}<syntaxhighlight lang="lua">instance = g_UsTableCitiesIM:GetInstance();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|UnitPanel.lua}}
:<code>UI/InGame/WorldView/UnitPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0223}}<syntaxhighlight lang="lua">instance = g_PromotionIM:GetInstance();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|VictoryProgress.lua}}
:<code>UI/InGame/Popups/VictoryProgress.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0221}}<syntaxhighlight lang="lua">curRow = g_DominationRowsIM:GetInstance();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0573}}<syntaxhighlight lang="lua">local controlTable = g_TechIM:GetInstance();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0815}}<syntaxhighlight lang="lua">local controlTable = cultureMgr:GetInstance();</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetInstance]]