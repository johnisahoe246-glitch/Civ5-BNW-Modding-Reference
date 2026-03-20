{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This method is declared by '''ControlBase'''.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''void''' UIElement:SetHide<b>(</b>'''int''' disablePolicies<b>)</b></code>


'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|disablePolicies:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Too many occurences. Only 50 out of 4034 are listed.''

{{PseudoH4|Advisors.lua}}
:<code>UI/InGame/WorldView/Advisors.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0108}}<syntaxhighlight lang="lua">advisor:SetHide(false);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CityBannerManager.lua}}
:<code>UI/InGame/CityBannerManager.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0074}}<syntaxhighlight lang="lua">svStrikeButton.CityRangeStrikeAnim:SetHide(true);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0194}}<syntaxhighlight lang="lua">controls.ResistanceIcon:SetHide(true);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0219}}<syntaxhighlight lang="lua">controls.OccupiedIcon:SetHide(true);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0644}}<syntaxhighlight lang="lua">controlTable.Anchor:SetHide( true );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0943}}<syntaxhighlight lang="lua">instance.SubControls.Anchor:SetHide( false );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CityStateDiploPopup.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/Popups/CityStateDiploPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0842}}<syntaxhighlight lang="lua">Controls.LargeGiftAnim:SetHide(false);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CityStateGreetingPopup.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/Popups/CityStateGreetingPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0084}}<syntaxhighlight lang="lua">Controls.QuestLabel:SetHide(true);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CityView.lua}}
:<code>UI/InGame/CityView/CityView.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0056}}<syntaxhighlight lang="lua">Controls.ProductionHelp:SetHide(true);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1156}}<syntaxhighlight lang="lua">Controls.SpecialistControlBox:SetHide( true );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1340}}<syntaxhighlight lang="lua">Controls.UnrazeCityButton:SetHide(false);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CivilopediaScreen.lua}}
:<code>UI/Civilopedia/CivilopediaScreen.lua</code>
:{{CodeBegin5}}
{{CodeLine5|2819}}<syntaxhighlight lang="lua">Controls.GoldChangeFrame:SetHide( false );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|3276}}<syntaxhighlight lang="lua">Controls.PolicyBranchFrame:SetHide( false );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|6118}}<syntaxhighlight lang="lua">Controls.CostFrame:SetHide( true );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|6134}}<syntaxhighlight lang="lua">Controls.FreePromotionsFrame:SetHide( true );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DiploCorner.lua}}
:<code>UI/InGame/WorldView/DiploCorner.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0429}}<syntaxhighlight lang="lua">Controls.DiploList:SetHide( true );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DiploList.lua}}
:<code>UI/InGame/DiploList.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0336}}<syntaxhighlight lang="lua">controlTable.DiploState:SetHide( true );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0388}}<syntaxhighlight lang="lua">Controls.MajorButton:SetHide( false );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|EconomicGeneralInfo.lua}}
:<code>UI/InGame/Popups/EconomicGeneralInfo.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0409}}<syntaxhighlight lang="lua">Controls.BuildingsStack:SetHide( not bWasHidden );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|EspionageOverview.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/Popups/EspionageOverview.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0455}}<syntaxhighlight lang="lua">Controls.AgentActivityProgressBack:SetHide(bHideActivityInfo);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1239}}<syntaxhighlight lang="lua">entry.ViewCityIcon:SetHide(true);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1619}}<syntaxhighlight lang="lua">imageControl:SetHide(true);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|GPList.lua}}
:<code>UI/InGame/GPList.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0270}}<syntaxhighlight lang="lua">Controls.EngineerStack:SetHide( not bWasHidden );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|HappinessInfo.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/Popups/HappinessInfo.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0067}}<syntaxhighlight lang="lua">Controls.LocalCityStack:SetHide( not bWasHidden );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|InGame.lua}}
:<code>UI/InGame/InGame.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0074}}<syntaxhighlight lang="lua">Controls.NetworkDebug:SetHide( not Controls.NetworkDebug:IsHidden() );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0079}}<syntaxhighlight lang="lua">Controls.DebugMenu:SetHide( bHideDebug );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0299}}<syntaxhighlight lang="lua">Controls.WorldView:SetHide( true );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|MilitaryOverview.lua}}
:<code>UI/InGame/Popups/MilitaryOverview.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0270}}<syntaxhighlight lang="lua">Controls.CivilianSeperator:SetHide( true );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|NotificationPanel.lua}}
:<code>UI/InGame/WorldView/NotificationPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0277}}<syntaxhighlight lang="lua">button:SetHide( false );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ProductionPopup.lua}}
:<code>UI/InGame/Popups/ProductionPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0314}}<syntaxhighlight lang="lua">Controls.UnitButton:SetHide( true );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ReligionOverview.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/Popups/ReligionOverview.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0618}}<syntaxhighlight lang="lua">Controls.BeliefsScrollPanel:SetHide(false);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|SaveMenu.lua}}
:<code>UI/InGame/Menus/SaveMenu.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0621}}<syntaxhighlight lang="lua">Controls.SaveMapButton:SetHide( true );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|SocialPolicyPopup.lua}}
:<code>UI/InGame/Popups/SocialPolicyPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0225}}<syntaxhighlight lang="lua">Controls.AnarchyBlock:SetHide( not player:IsAnarchy() );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0380}}<syntaxhighlight lang="lua">thisLockedBox:SetHide(false);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|StagingRoom.lua}}
:<code>UI/FrontEnd/Multiplayer/StagingRoom.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0283}}<syntaxhighlight lang="lua">m_SlotInstances[i].Root:SetHide( true );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0445}}<syntaxhighlight lang="lua">slotInstance.CivPulldown:SetHide( bCantChange );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0860}}<syntaxhighlight lang="lua">Controls.ChatBox:SetHide( false );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TechAwardPopup.lua}}
:<code>UI/InGame/Popups/TechAwardPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0070}}<syntaxhighlight lang="lua">Controls.TechIcon:SetHide( true );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TechPopup.lua}}
:<code>UI/InGame/TechPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0160}}<syntaxhighlight lang="lua">thisTechButtonInstance.CurrentlyResearching:SetHide( false );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TextPopup.lua}}
:<code>UI/InGame/Popups/TextPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0026}}<syntaxhighlight lang="lua">Controls.TopImage:SetHide( false );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TradeLogic.lua}}
:<code>UI/InGame/WorldView/TradeLogic.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0576}}<syntaxhighlight lang="lua">Controls.ModifyButton:SetHide( false );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0609}}<syntaxhighlight lang="lua">Controls.WhatDoYouWantButton:SetHide(true);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1487}}<syntaxhighlight lang="lua">Controls.UsPocketOpenBorders:SetHide(false);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1492}}<syntaxhighlight lang="lua">Controls.ThemPocketDefensivePact:SetHide(false);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1526}}<syntaxhighlight lang="lua">Controls.UsTableLuxuryStack:SetHide( true );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1854}}<syntaxhighlight lang="lua">Controls.ThemTableDeclareWarStack:SetHide( false );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|UnitPanel.lua}}
:<code>UI/InGame/WorldView/UnitPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0653}}<syntaxhighlight lang="lua">Controls.HealthBar:SetHide(true);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0663}}<syntaxhighlight lang="lua">Controls.RedBar:SetHide(false);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|UnitPanel.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/WorldView/UnitPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0316}}<syntaxhighlight lang="lua">Controls.SecondaryStack:SetHide(true);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|VictoryProgress.lua (G&K)}}
:<code>DLC/Expansion/Scenarios/MedievalScenario/VictoryProgress.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0707}}<syntaxhighlight lang="lua">controlTable.UNIcon:SetHide(iTeam ~= iVaticanExtraVoteTeam);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|SetHide]]