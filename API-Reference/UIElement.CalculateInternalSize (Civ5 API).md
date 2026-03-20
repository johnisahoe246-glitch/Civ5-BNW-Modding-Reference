{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of ControlBase.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''void''' UIElement:CalculateInternalSize<b>(</b><b>)</b></code>




=Source code samples=
''Too many occurences. Only 50 out of 226 are listed.''

{{PseudoH4|AdvancedSetup.lua}}
:<code>UI/FrontEnd/GameSetup/AdvancedSetup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0154}}<syntaxhighlight lang="lua">Controls.OptionsScrollPanel:CalculateInternalSize();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0327}}<syntaxhighlight lang="lua">Controls.ListingScrollPanel:CalculateInternalSize();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|AdvisorCounselPopup.lua}}
:<code>UI/InGame/Popups/AdvisorCounselPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0121}}<syntaxhighlight lang="lua">Controls.EA_ScrollPanel:CalculateInternalSize();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0128}}<syntaxhighlight lang="lua">Controls.MA_ScrollPanel:CalculateInternalSize();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0135}}<syntaxhighlight lang="lua">Controls.FA_ScrollPanel:CalculateInternalSize();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0142}}<syntaxhighlight lang="lua">Controls.SA_ScrollPanel:CalculateInternalSize();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|AdvisorInfoPopup.lua}}
:<code>UI/InGame/Popups/AdvisorInfoPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0076}}<syntaxhighlight lang="lua">Controls.DescriptionPanel:CalculateInternalSize();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0132}}<syntaxhighlight lang="lua">Controls.RelatedConceptPanel:CalculateInternalSize();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ChooseFaithGreatPerson.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/Popups/ChooseFaithGreatPerson.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0136}}<syntaxhighlight lang="lua">Controls.ItemScrollPanel:CalculateInternalSize();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ChooseReligionPopup.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/Popups/ChooseReligionPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0329}}<syntaxhighlight lang="lua">Controls.ReligionScrollPanel:CalculateInternalSize();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0532}}<syntaxhighlight lang="lua">Controls.BeliefScrollPanel:CalculateInternalSize();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CityStateDiploPopup.lua}}
:<code>UI/InGame/Popups/CityStateDiploPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0809}}<syntaxhighlight lang="lua">Controls.ButtonScrollPanel:CalculateInternalSize();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CityView.lua}}
:<code>UI/InGame/CityView/CityView.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0898}}<syntaxhighlight lang="lua">Controls.ProductionHelpScroll:CalculateInternalSize();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CivilopediaScreen.lua}}
:<code>UI/Civilopedia/CivilopediaScreen.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0125}}<syntaxhighlight lang="lua">Controls.ScrollPanel:CalculateInternalSize();</syntaxhighlight>
{{CodeLine5|0126}}<syntaxhighlight lang="lua">Controls.LeftScrollPanel:CalculateInternalSize();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|Credits.lua}}
:<code>UI/FrontEnd/Credits.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0088}}<syntaxhighlight lang="lua">Controls.MajorScroll:CalculateInternalSize();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DiploCorner.lua}}
:<code>UI/InGame/WorldView/DiploCorner.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0182}}<syntaxhighlight lang="lua">Controls.ChatScroll:CalculateInternalSize();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DiploCurrentDeals.lua}}
:<code>UI/InGame/Popups/DiploCurrentDeals.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0077}}<syntaxhighlight lang="lua">Controls.ListScrollPanel:CalculateInternalSize();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DiploGlobalRelationships.lua}}
:<code>UI/InGame/Popups/DiploGlobalRelationships.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0315}}<syntaxhighlight lang="lua">Controls.MajorCivScrollPanel:CalculateInternalSize();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DiploRelationships.lua}}
:<code>UI/InGame/Popups/DiploRelationships.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0110}}<syntaxhighlight lang="lua">Controls.MinorCivScrollPanel:CalculateInternalSize();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DiscussionDialog.lua}}
:<code>UI/InGame/LeaderHead/DiscussionDialog.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0826}}<syntaxhighlight lang="lua">Controls.LeaderScrollPanel:CalculateInternalSize();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|EconomicGeneralInfo.lua}}
:<code>UI/InGame/Popups/EconomicGeneralInfo.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0169}}<syntaxhighlight lang="lua">Controls.MainScroll:CalculateInternalSize();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0364}}<syntaxhighlight lang="lua">Controls.GoldScroll:CalculateInternalSize();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|EndGameReplay.lua}}
:<code>UI/InGame/Popups/EndGameReplay.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0036}}<syntaxhighlight lang="lua">Controls.ReplayMessageScrollPanel:CalculateInternalSize();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|EspionageOverview.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/Popups/EspionageOverview.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0781}}<syntaxhighlight lang="lua">Controls.AgentScrollPanel:CalculateInternalSize();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1077}}<syntaxhighlight lang="lua">Controls.MyCityScrollPanel:CalculateInternalSize();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1375}}<syntaxhighlight lang="lua">Controls.TheirCityScrollPanel:CalculateInternalSize();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1500}}<syntaxhighlight lang="lua">Controls.IntrigueMessageScrollPanel:CalculateInternalSize();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|HappinessInfo.lua}}
:<code>UI/InGame/Popups/HappinessInfo.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0027}}<syntaxhighlight lang="lua">Controls.HappinessScroll:CalculateInternalSize();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0091}}<syntaxhighlight lang="lua">Controls.UnhappinessScroll:CalculateInternalSize();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0108}}<syntaxhighlight lang="lua">Controls.ResourcesScroll:CalculateInternalSize();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|InstalledPanel.lua}}
:<code>UI/FrontEnd/Modding/InstalledPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0751}}<syntaxhighlight lang="lua">Controls.DescriptionScrollPanel:CalculateInternalSize();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|LoadMenu.lua}}
:<code>UI/FrontEnd/LoadMenu.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0159}}<syntaxhighlight lang="lua">Controls.ReferencedPackagesScrollPanel:CalculateInternalSize();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|MPList.lua}}
:<code>UI/InGame/WorldView/MPList.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0196}}<syntaxhighlight lang="lua">Controls.MPListScroll:CalculateInternalSize();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|NotificationLogPopup.lua}}
:<code>UI/InGame/Popups/NotificationLogPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0037}}<syntaxhighlight lang="lua">Controls.NotificationScrollPanel:CalculateInternalSize();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|NotificationPanel.lua}}
:<code>UI/InGame/WorldView/NotificationPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0369}}<syntaxhighlight lang="lua">Controls.SmallScrollPanel:CalculateInternalSize();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ReligionOverview.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/Popups/ReligionOverview.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0403}}<syntaxhighlight lang="lua">Controls.YourReligiousBeliefsScrollPanel:CalculateInternalSize();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0546}}<syntaxhighlight lang="lua">Controls.WorldReligionsScrollPanel:CalculateInternalSize();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0635}}<syntaxhighlight lang="lua">Controls.BeliefsScrollPanel:CalculateInternalSize();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ReplayViewer.lua}}
:<code>UI/InGame/Popups/ReplayViewer.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0751}}<syntaxhighlight lang="lua">Controls.GraphLegendScrollPanel:CalculateInternalSize();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TechTree.lua}}
:<code>UI/InGame/TechTree/TechTree.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0345}}<syntaxhighlight lang="lua">Controls.TechTreeScrollPanel:CalculateInternalSize();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TradeLogic.lua}}
:<code>UI/InGame/WorldView/TradeLogic.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0764}}<syntaxhighlight lang="lua">Controls.UsPocketPanel:CalculateInternalSize();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0768}}<syntaxhighlight lang="lua">Controls.ThemPocketPanel:CalculateInternalSize();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1588}}<syntaxhighlight lang="lua">Controls.UsTablePanel:CalculateInternalSize();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1590}}<syntaxhighlight lang="lua">Controls.ThemTablePanel:CalculateInternalSize();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|2496}}<syntaxhighlight lang="lua">m_panel:CalculateInternalSize();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|VictoryProgress.lua}}
:<code>UI/InGame/Popups/VictoryProgress.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0543}}<syntaxhighlight lang="lua">Controls.ScoreScrollPanel:CalculateInternalSize();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0744}}<syntaxhighlight lang="lua">Controls.DiploScrollPanel:CalculateInternalSize();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0806}}<syntaxhighlight lang="lua">Controls.CultureScrollPanel:CalculateInternalSize();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|VoteResultsPopup.lua}}
:<code>UI/InGame/Popups/VoteResultsPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0251}}<syntaxhighlight lang="lua">Controls.PlayerListScrollPanel:CalculateInternalSize();</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|CalculateInternalSize]]