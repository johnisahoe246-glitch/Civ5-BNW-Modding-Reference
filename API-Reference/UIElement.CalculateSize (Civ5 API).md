{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of ControlBase.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''void''' UIElement:CalculateSize<b>(</b><b>)</b></code>




=Source code samples=
''Too many occurences. Only 50 out of 424 are listed.''

{{PseudoH4|AdvancedSetup.lua}}
:<code>UI/FrontEnd/GameSetup/AdvancedSetup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0151}}<syntaxhighlight lang="lua">Controls.DropDownOptionsStack:CalculateSize();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0244}}<syntaxhighlight lang="lua">Controls.MaxTurnStack:CalculateSize();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0250}}<syntaxhighlight lang="lua">Controls.GameOptionsFullStack:CalculateSize();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1067}}<syntaxhighlight lang="lua">Controls.VictoryConditionsStack:CalculateSize();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|AdvisorInfoPopup.lua}}
:<code>UI/InGame/Popups/AdvisorInfoPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0130}}<syntaxhighlight lang="lua">Controls.RelatedConceptButtonStack:CalculateSize();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CityStateDiploPopup.lua}}
:<code>UI/InGame/Popups/CityStateDiploPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0806}}<syntaxhighlight lang="lua">Controls.ButtonStack:CalculateSize();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CityView.lua}}
:<code>UI/InGame/CityView/CityView.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0728}}<syntaxhighlight lang="lua">Controls.TitleStack:CalculateSize();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1256}}<syntaxhighlight lang="lua">Controls.WorkerManagementBox:CalculateSize();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1305}}<syntaxhighlight lang="lua">Controls.NotificationStack:CalculateSize();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CivilopediaScreen.lua}}
:<code>UI/Civilopedia/CivilopediaScreen.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1294}}<syntaxhighlight lang="lua">Controls.NarrowStack:CalculateSize();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1296}}<syntaxhighlight lang="lua">Controls.SuperWideStack:CalculateSize();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CustomMod.lua}}
:<code>UI/FrontEnd/Modding/CustomMod.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0132}}<syntaxhighlight lang="lua">Controls.LoadFileButtonStack:CalculateSize();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DiploCurrentDeals.lua}}
:<code>UI/InGame/Popups/DiploCurrentDeals.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0074}}<syntaxhighlight lang="lua">Controls.CurrentDealsStack:CalculateSize();</syntaxhighlight>
{{CodeLine5|0075}}<syntaxhighlight lang="lua">Controls.HistoricDealsStack:CalculateSize();</syntaxhighlight>
{{CodeLine5|0076}}<syntaxhighlight lang="lua">Controls.AllDealsStack:CalculateSize();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DiploGlobalRelationships.lua}}
:<code>UI/InGame/Popups/DiploGlobalRelationships.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0279}}<syntaxhighlight lang="lua">controlTable.WondersStack:CalculateSize();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0301}}<syntaxhighlight lang="lua">controlTable.PlayerInfoStack:CalculateSize();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DiploList.lua}}
:<code>UI/InGame/DiploList.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0368}}<syntaxhighlight lang="lua">controlTable.StatusStack:CalculateSize();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0395}}<syntaxhighlight lang="lua">Controls.MinorStack:CalculateSize();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DiploRelationships.lua}}
:<code>UI/InGame/Popups/DiploRelationships.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0091}}<syntaxhighlight lang="lua">controlTable.CityStack:CalculateSize();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DiscussionDialog.lua}}
:<code>UI/InGame/LeaderHead/DiscussionDialog.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0824}}<syntaxhighlight lang="lua">Controls.LeaderStack:CalculateSize();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|EconomicGeneralInfo.lua}}
:<code>UI/InGame/Popups/EconomicGeneralInfo.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0223}}<syntaxhighlight lang="lua">Controls.CityStack:CalculateSize();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0383}}<syntaxhighlight lang="lua">Controls.GoldStack:CalculateSize();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|EspionageOverview.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/Popups/EspionageOverview.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0341}}<syntaxhighlight lang="lua">Controls.ConfirmContent:CalculateSize();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0774}}<syntaxhighlight lang="lua">agentEntry.AgentActivitiesStack:CalculateSize();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1075}}<syntaxhighlight lang="lua">Controls.MyCityStack:CalculateSize();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1373}}<syntaxhighlight lang="lua">Controls.TheirCityStack:CalculateSize();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1498}}<syntaxhighlight lang="lua">Controls.IntrigueMessageStack:CalculateSize();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|GameMenu.lua}}
:<code>UI/InGame/Menus/GameMenu.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0420}}<syntaxhighlight lang="lua">Controls.SetupOptions:CalculateSize();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0426}}<syntaxhighlight lang="lua">Controls.AdvancedOptions:CalculateSize();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|HappinessInfo.lua}}
:<code>UI/InGame/Popups/HappinessInfo.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0106}}<syntaxhighlight lang="lua">Controls.ResourcesStack:CalculateSize();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0356}}<syntaxhighlight lang="lua">Controls.GarrisonStack:CalculateSize();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0645}}<syntaxhighlight lang="lua">Controls.ResourcesAvailableStack:CalculateSize();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ProductionPopup.lua}}
:<code>UI/InGame/Popups/ProductionPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0727}}<syntaxhighlight lang="lua">Controls.UnitButtonStack:CalculateSize();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0730}}<syntaxhighlight lang="lua">Controls.BuildingButtonStack:CalculateSize();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|Ranking.lua}}
:<code>UI/InGame/Popups/Ranking.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0042}}<syntaxhighlight lang="lua">controlTable.MyStack:CalculateSize();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ReligionOverview.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/Popups/ReligionOverview.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0336}}<syntaxhighlight lang="lua">Controls.GreatPersonList:CalculateSize();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0633}}<syntaxhighlight lang="lua">Controls.BeliefsStack:CalculateSize();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ResourceList.lua}}
:<code>UI/InGame/ResourceList.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0153}}<syntaxhighlight lang="lua">Controls.LuxuryStack:CalculateSize();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|SelectCivilization.lua}}
:<code>UI/FrontEnd/GameSetup/SelectCivilization.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0236}}<syntaxhighlight lang="lua">Controls.Stack:CalculateSize();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TradeLogic.lua}}
:<code>UI/InGame/WorldView/TradeLogic.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1563}}<syntaxhighlight lang="lua">Controls.UsPocketLuxuryStack:CalculateSize();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1568}}<syntaxhighlight lang="lua">Controls.UsTableCitiesStack:CalculateSize();</syntaxhighlight>
{{CodeLine5|1569}}<syntaxhighlight lang="lua">Controls.ThemTableCitiesStack:CalculateSize();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1571}}<syntaxhighlight lang="lua">Controls.ThemPocketLeaderStack:CalculateSize();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1575}}<syntaxhighlight lang="lua">Controls.ThemTableMakePeaceStack:CalculateSize();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1581}}<syntaxhighlight lang="lua">Controls.UsTableStack:CalculateSize();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|2495}}<syntaxhighlight lang="lua">m_pocketStack:CalculateSize();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|UnitList.lua}}
:<code>UI/InGame/UnitList.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0227}}<syntaxhighlight lang="lua">instance.UnitStack:CalculateSize();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|UnitPanel.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/WorldView/UnitPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0289}}<syntaxhighlight lang="lua">Controls.PrimaryStack:CalculateSize();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|VictoryProgress.lua}}
:<code>UI/InGame/Popups/VictoryProgress.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0541}}<syntaxhighlight lang="lua">Controls.ScoreStack:CalculateSize();</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|CalculateSize]]