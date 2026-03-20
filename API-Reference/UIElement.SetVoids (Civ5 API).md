{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This method is declared by '''ButtonBase''', {{Type5|Grid}} and {{Type5|GridButton}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''void''' UIElement:SetVoids<b>(</b>{{Type5|ResourceType}} building, {{Type5|ResourceType}} addToList<b>)</b></code>


'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|building:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|addToList:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Too many occurences. Only 50 out of 343 are listed.''

{{PseudoH4|AdvancedSetup.lua}}
:<code>UI/FrontEnd/GameSetup/AdvancedSetup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0430}}<syntaxhighlight lang="lua">controlTable.Button:SetVoids( playerID, id );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0979}}<syntaxhighlight lang="lua">controlTable.Button:SetVoids( playerID, 0 );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0987}}<syntaxhighlight lang="lua">controlTable.Button:SetVoids( playerID, i );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CityBannerManager.lua}}
:<code>UI/InGame/CityBannerManager.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0392}}<syntaxhighlight lang="lua">controls.CityBannerProductionButton:SetVoids( city:GetID(), nil );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CityList.lua}}
:<code>UI/InGame/CityList.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0107}}<syntaxhighlight lang="lua">instance.Button:SetVoids( pCity:GetX(), pCity:GetY() );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0426}}<syntaxhighlight lang="lua">instance.ProdButton:SetVoids( city:GetID(), nil );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CityView.lua}}
:<code>UI/InGame/CityView/CityView.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0467}}<syntaxhighlight lang="lua">controlTable.BuildingFilledSpecialistSlot2:SetVoids( buildingID, 2 );</syntaxhighlight>
{{CodeLine5|0468}}<syntaxhighlight lang="lua">controlTable.BuildingFilledSpecialistSlot3:SetVoids( buildingID, 3 );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0474}}<syntaxhighlight lang="lua">controlTable.BuildingEmptySpecialistSlot1:SetVoids( buildingID, 1 );</syntaxhighlight>
{{CodeLine5|0475}}<syntaxhighlight lang="lua">controlTable.BuildingEmptySpecialistSlot2:SetVoids( buildingID, 2 );</syntaxhighlight>
{{CodeLine5|0476}}<syntaxhighlight lang="lua">controlTable.BuildingEmptySpecialistSlot3:SetVoids( buildingID, 3 );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CivilopediaScreen.lua}}
:<code>UI/Civilopedia/CivilopediaScreen.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1808}}<syntaxhighlight lang="lua">button:SetVoids( buttonId, addToList );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|2088}}<syntaxhighlight lang="lua">thisBuildingInstance.UnlockedBuildingButton:SetVoids( thisBuildingInfo.ID, addToList );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|2946}}<syntaxhighlight lang="lua">thisBuildingInstance.RequiredBuildingButton:SetVoids( thisBuildingInfo.ID, addToList );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|3553}}<syntaxhighlight lang="lua">thisBuildingInstance.UniqueBuildingButton:SetVoids( thisBuildingInfo.ID, addToList );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|3584}}<syntaxhighlight lang="lua">thisImprovementInstance.UniqueImprovementButton:SetVoids( thisImprovement.ID, addToList );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|4621}}<syntaxhighlight lang="lua">thisListInstance.ListItemButton:SetVoids( homePageOfCategoryID, addToList );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|4654}}<syntaxhighlight lang="lua">thisListInstance.ListItemButton:SetVoids( v.entryID, addToList );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|4682}}<syntaxhighlight lang="lua">thisTechInstance.ListItemButton:SetVoids( homePageOfCategoryID, addToList );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|4704}}<syntaxhighlight lang="lua">thisEraInstance.ListHeadingButton:SetVoids( eraID, 0 );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|5019}}<syntaxhighlight lang="lua">thisHeadingInstance.ListHeadingButton:SetVoids( branchID, 0 );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|5210}}<syntaxhighlight lang="lua">thisHeadingInstance.ListHeadingButton:SetVoids( traitID, 0 );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|5518}}<syntaxhighlight lang="lua">thisTechInstance.ListItemButton:SetVoids( v.entryID, addToList );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CivilopediaScreen.lua (G&K)}}
:<code>DLC/Expansion/UI/Civilopedia/CivilopediaScreen.lua</code>
:{{CodeBegin5}}
{{CodeLine5|4984}}<syntaxhighlight lang="lua">thisEraInstance.ListHeadingButton:SetVoids( categoryID, 0 );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|5652}}<syntaxhighlight lang="lua">thisListInstance.ListItemButton:SetVoids(0, addToList );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|6469}}<syntaxhighlight lang="lua">thisListInstance.ListItemButton:SetVoids( v.entryID[2], addToList );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DiploCorner.lua}}
:<code>UI/InGame/WorldView/DiploCorner.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0320}}<syntaxhighlight lang="lua">controlTable.Button:SetVoids( -1, -1 );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0339}}<syntaxhighlight lang="lua">controlTable.Button:SetVoids( g_iLocalTeam, -1 );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0354}}<syntaxhighlight lang="lua">controlTable.Button:SetVoids( -1, iPlayer );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DiploCurrentDeals.lua}}
:<code>UI/InGame/Popups/DiploCurrentDeals.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0057}}<syntaxhighlight lang="lua">controlTable.DealButton:SetVoids( i, 0 );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ProductionPopup.lua}}
:<code>UI/InGame/Popups/ProductionPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0224}}<syntaxhighlight lang="lua">Controls.CityButton:SetVoids( city:GetX(), city:GetY() );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ReligionOverview.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/Popups/ReligionOverview.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0412}}<syntaxhighlight lang="lua">controlTable.Button:SetVoids(v1, v2);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|StagingRoom.lua}}
:<code>UI/FrontEnd/Multiplayer/StagingRoom.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1043}}<syntaxhighlight lang="lua">controlTable.Button:SetVoids( playerID, v.ID );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1084}}<syntaxhighlight lang="lua">controlTable.Button:SetVoids( playerID, friendList[i].steamID );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1115}}<syntaxhighlight lang="lua">controlTable.Button:SetVoids( playerID, i-1 ); -- TODO: playerID is really more like the slot position.</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1137}}<syntaxhighlight lang="lua">controlTable.Button:SetVoids( playerID, info.ID );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1160}}<syntaxhighlight lang="lua">controlTable.Button:SetVoids( playerID, 1 );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TechButtonInclude.lua}}
:<code>UI/InGame/TechTree/TechButtonInclude.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0334}}<syntaxhighlight lang="lua">thisTechButtonInstance[buttonName]:SetVoids(void1, void2);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TradeLogic.lua}}
:<code>UI/InGame/WorldView/TradeLogic.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1713}}<syntaxhighlight lang="lua">instance.Button:SetVoids( g_iUs, pCity:GetID() );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1718}}<syntaxhighlight lang="lua">instance.Button:SetVoids( g_iThem, pCity:GetID() );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|2255}}<syntaxhighlight lang="lua">controlTable.Button:SetVoids( isUs, row.ID );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|2472}}<syntaxhighlight lang="lua">instance.Button:SetVoids( m_iFrom, iCityID );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|2639}}<syntaxhighlight lang="lua">Controls.UsPocketOtherPlayerWar:SetVoids( 1, WAR );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|2642}}<syntaxhighlight lang="lua">Controls.ThemPocketOtherPlayerWar:SetVoids( 0, WAR );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|2645}}<syntaxhighlight lang="lua">Controls.UsPocketOtherPlayerPeace:SetVoids( 1, PEACE );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|2648}}<syntaxhighlight lang="lua">Controls.ThemPocketOtherPlayerPeace:SetVoids( 0, PEACE );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|2785}}<syntaxhighlight lang="lua">controlTable.Button:SetVoids( iLoopPlayer, 1 );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|2795}}<syntaxhighlight lang="lua">controlTable.Button:SetVoids( iLoopPlayer, 0 );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|UnitFlagManager.lua}}
:<code>UI/InGame/UnitFlagManager.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0696}}<syntaxhighlight lang="lua">controlTable.Button:SetVoids( self.m_playerID, self.m_UnitID );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1069}}<syntaxhighlight lang="lua">controlTable.Button:SetVoids( pPlotUnit:GetOwner(), pPlotUnit:GetID() );</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|SetVoids]]