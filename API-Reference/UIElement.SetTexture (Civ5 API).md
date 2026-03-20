{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of ControlBase.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''void''' UIElement:SetTexture<b>(</b>'''string''' textureName<b>)</b></code>


'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|textureName:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Too many occurences. Only 50 out of 406 are listed.''

{{PseudoH4|CityBannerManager.lua}}
:<code>UI/InGame/CityBannerManager.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0565}}<syntaxhighlight lang="lua">controls.StatusIconBG:SetTexture( row.StatusIcon );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CityStateStatusHelper.lua (G&K)}}
:<code>DLC/Expansion/UI/CityStateStatusHelper.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0123}}<syntaxhighlight lang="lua">negBarCtrl:SetTexture(info.NegativeStatusMeter);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CityView.lua}}
:<code>UI/InGame/CityView/CityView.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0435}}<syntaxhighlight lang="lua">controlTable.BuildingFilledSpecialistSlot3:SetTexture(scientistTexture);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0445}}<syntaxhighlight lang="lua">controlTable.BuildingFilledSpecialistSlot1:SetTexture(engineerTexture);</syntaxhighlight>
{{CodeLine5|0446}}<syntaxhighlight lang="lua">controlTable.BuildingFilledSpecialistSlot2:SetTexture(engineerTexture);</syntaxhighlight>
{{CodeLine5|0447}}<syntaxhighlight lang="lua">controlTable.BuildingFilledSpecialistSlot3:SetTexture(engineerTexture);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0449}}<syntaxhighlight lang="lua">controlTable.BuildingFilledSpecialistSlot1:SetTexture(workerTexture);</syntaxhighlight>
{{CodeLine5|0450}}<syntaxhighlight lang="lua">controlTable.BuildingFilledSpecialistSlot2:SetTexture(workerTexture);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1501}}<syntaxhighlight lang="lua">Controls.HealthMeter:SetTexture("CityNamePanelHealthBarRed.dds");</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CivilopediaScreen.lua}}
:<code>UI/Civilopedia/CivilopediaScreen.lua</code>
:{{CodeBegin5}}
{{CodeLine5|2938}}<syntaxhighlight lang="lua">thisBuildingInstance.RequiredBuildingImage:SetTexture( defaultErrorTextureSheet );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CivilopediaScreen.lua (G&K)}}
:<code>DLC/Expansion/UI/Civilopedia/CivilopediaScreen.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1816}}<syntaxhighlight lang="lua">Controls.Portrait:SetTexture("Religion256.dds");</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CustomMod.lua}}
:<code>UI/FrontEnd/Modding/CustomMod.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0084}}<syntaxhighlight lang="lua">Controls.DetailsBackgroundImage:SetTexture(filePath);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DiploList.lua}}
:<code>UI/InGame/DiploList.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0476}}<syntaxhighlight lang="lua">controlTable.StatusIconBG:SetTexture(info.row.StatusIcon);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DiploRelationships.lua}}
:<code>UI/InGame/Popups/DiploRelationships.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0482}}<syntaxhighlight lang="lua">pStack.StatusIconBG:SetTexture(info.row.StatusIcon);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|EndGameMenu.lua}}
:<code>UI/InGame/Popups/EndGameMenu.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0171}}<syntaxhighlight lang="lua">Controls.BackgroundImage:SetTexture(GameInfo.Victories["VICTORY_TIME"].VictoryBackground);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|EnemyUnitPanel.lua}}
:<code>UI/InGame/WorldView/EnemyUnitPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0067}}<syntaxhighlight lang="lua">Controls.UnitIcon:SetTexture( textureAtlas );</syntaxhighlight>
{{CodeLine5|0068}}<syntaxhighlight lang="lua">Controls.UnitIconShadow:SetTexture( textureAtlas );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|EspionageOverview.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/Popups/EspionageOverview.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0660}}<syntaxhighlight lang="lua">agentEntry.AgentActivityProgress:SetTexture(progressBarState.ProgressBarTexture);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|FoRScenarioLoadScreen.lua (G&K)}}
:<code>DLC/Expansion/Scenarios/FallOfRomeScenario/FoRScenarioLoadScreen.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0215}}<syntaxhighlight lang="lua">controlTable.Icon:SetTexture( textureAtlas );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0217}}<syntaxhighlight lang="lua">controlTable.IconShadow:SetTexture( textureAtlas );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0288}}<syntaxhighlight lang="lua">Controls.IconShadow:SetTexture( questionTextureSheet );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|FrontEnd.lua}}
:<code>UI/FrontEnd/FrontEnd.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0013}}<syntaxhighlight lang="lua">Controls.AtlasLogo:SetTexture( "CivilzationVAtlas.dds" );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|GameSetupScreen.lua}}
:<code>UI/FrontEnd/GameSetup/GameSetupScreen.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0511}}<syntaxhighlight lang="lua">Controls[buttonName]:SetTexture( questionTextureSheet );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|HallOfFame.lua}}
:<code>UI/InGame/Popups/HallOfFame.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0095}}<syntaxhighlight lang="lua">controlTable.WinCivIcon:SetTexture( textureAtlas );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|IconSupport.lua}}
:<code>UI/IconSupport.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0122}}<syntaxhighlight lang="lua">imageControl:SetTexture(filename);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0171}}<syntaxhighlight lang="lua">iconControl:SetTexture( textureAtlas );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|InfoCorner.lua}}
:<code>UI/InGame/InfoCorner.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0060}}<syntaxhighlight lang="lua">Controls.PDButton:SetTexture( m_InfoData[iInfoType].Image );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0111}}<syntaxhighlight lang="lua">controlTable.MOImage:SetTexture( "assets/UI/Art/Icons/MainClose.dds" );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0114}}<syntaxhighlight lang="lua">controlTable.Button:SetTexture( value.Image );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|InstalledPanel.lua}}
:<code>UI/FrontEnd/Modding/InstalledPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0440}}<syntaxhighlight lang="lua">v.ImageControl:SetTexture("SelectedDown.dds");</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|LoadMenu.lua}}
:<code>UI/FrontEnd/LoadMenu.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0285}}<syntaxhighlight lang="lua">Controls.CivIcon:SetTexture( textureAtlas );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0394}}<syntaxhighlight lang="lua">Controls.SpeedIcon:SetTexture( questionTextureSheet );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0482}}<syntaxhighlight lang="lua">Controls.MapType:SetTexture( questionTextureSheet );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|MainMenu.lua}}
:<code>UI/FrontEnd/MainMenu.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0019}}<syntaxhighlight lang="lua">Controls.Civ5Logo:SetTexture( "CivilzationV_Logo.dds" );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|MiniMapPanel.lua}}
:<code>UI/InGame/WorldView/MiniMapPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0037}}<syntaxhighlight lang="lua">Controls.StrategicViewButton:SetTexture( "assets/UI/Art/Icons/MainWorldButton.dds" );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0045}}<syntaxhighlight lang="lua">Controls.StrategicMO:SetTexture( "assets/UI/Art/Icons/MainStrategicButton.dds" );</syntaxhighlight>
{{CodeLine5|0046}}<syntaxhighlight lang="lua">Controls.StrategicHL:SetTexture( "assets/UI/Art/Icons/MainStrategicButtonHL.dds" );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|NewEraPopup.lua}}
:<code>UI/InGame/Popups/NewEraPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0037}}<syntaxhighlight lang="lua">Controls.EraImage:SetTexture(lastBackgroundImage);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|SelectCivilization.lua}}
:<code>UI/FrontEnd/GameSetup/SelectCivilization.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0127}}<syntaxhighlight lang="lua">controlTable.CivIcon:SetTexture( textureAtlas );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|SocialPolicyPopup.lua}}
:<code>UI/InGame/Popups/SocialPolicyPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0761}}<syntaxhighlight lang="lua">pipe.ConnectorImage:SetTexture(bottomRightTexture);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0813}}<syntaxhighlight lang="lua">pipe.ConnectorImage:SetTexture(topRightTexture);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TechButtonInclude.lua}}
:<code>UI/InGame/TechTree/TechButtonInclude.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0352}}<syntaxhighlight lang="lua">thisButton:SetTexture( textureSheet );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TechTree.lua}}
:<code>UI/InGame/TechTree/TechTree.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0203}}<syntaxhighlight lang="lua">startPipe.TechPipeIcon:SetTexture(right1Texture);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0209}}<syntaxhighlight lang="lua">pipe.TechPipeIcon:SetTexture(right1Texture);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0226}}<syntaxhighlight lang="lua">pipe.TechPipeIcon:SetTexture(topRightTexture);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0279}}<syntaxhighlight lang="lua">pipe.TechPipeIcon:SetTexture(bottomLeftTexture);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|UnitFlagManager.lua}}
:<code>UI/InGame/UnitFlagManager.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0546}}<syntaxhighlight lang="lua">self.m_Instance.FlagShadow:SetTexture( textureName );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|UnitPanel.lua}}
:<code>UI/InGame/WorldView/UnitPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0443}}<syntaxhighlight lang="lua">Controls.UnitIconShadow:SetTexture(textureAtlas);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|VoteResultsPopup.lua}}
:<code>UI/InGame/Popups/VoteResultsPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0058}}<syntaxhighlight lang="lua">controlTable.Portrait:SetTexture( questionTextureSheet );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|YieldIconManager.lua}}
:<code>UI/InGame/YieldIconManager.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0125}}<syntaxhighlight lang="lua">imageInstance.Image:SetTexture(defaultTexture);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|SetTexture]]