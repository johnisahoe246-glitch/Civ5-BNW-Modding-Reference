{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This method is declared by '''ControlBase'''.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''void''' UIElement:SetOffsetVal<b>(</b>'''int''' xOffset, '''int''' yOffset<b>)</b></code>


'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|xOffset:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|yOffset:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Too many occurences. Only 50 out of 233 are listed.''

{{PseudoH4|ChooseReligionPopup.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/Popups/ChooseReligionPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0383}}<syntaxhighlight lang="lua">Controls.FollowerBelief2Description:SetOffsetVal(24,25);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0388}}<syntaxhighlight lang="lua">Controls.EnhancerBeliefDescription:SetOffsetVal(24,25);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0407}}<syntaxhighlight lang="lua">Controls.FollowerBelief2Description:SetOffsetVal(52,30);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0412}}<syntaxhighlight lang="lua">Controls.EnhancerBeliefDescription:SetOffsetVal(52,30);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0440}}<syntaxhighlight lang="lua">Controls.BonusBeliefDescription:SetOffsetVal(24,25);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0452}}<syntaxhighlight lang="lua">Controls.BonusBeliefDescription:SetOffsetVal(52,30);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CityBannerManager.lua}}
:<code>UI/InGame/CityBannerManager.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0754}}<syntaxhighlight lang="lua">BannerInstance.CityName:SetOffsetVal(-3,0);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CityView.lua}}
:<code>UI/InGame/CityView/CityView.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1082}}<syntaxhighlight lang="lua">controlTable.SlackerButton:SetOffsetVal( (slackerAdded % numberOfSlackersPerRow) * slackerSize + slackerPadding, math.floor(slackerAdded / numberOfSlackersPerRow) * slackerSize + slackerPadding );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CivilopediaScreen.lua}}
:<code>UI/Civilopedia/CivilopediaScreen.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0115}}<syntaxhighlight lang="lua">Controls.ScrollBar:SetOffsetVal( 0, 18 );</syntaxhighlight>
{{CodeLine5|0116}}<syntaxhighlight lang="lua">Controls.LeftScrollBar:SetOffsetVal( 0, 18 );</syntaxhighlight>
{{CodeLine5|0117}}<syntaxhighlight lang="lua">Controls.DownButton:SetOffsetVal( 0, screenSizeY - 126 - 18 );</syntaxhighlight>
{{CodeLine5|0118}}<syntaxhighlight lang="lua">Controls.LeftDownButton:SetOffsetVal( 0, screenSizeY - 126 - 18 );</syntaxhighlight>
{{CodeLine5|0119}}<syntaxhighlight lang="lua">Controls.LeftUpButton:SetOffsetVal( 0, 0 );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0133}}<syntaxhighlight lang="lua">Controls.SelectedCategoryTab:SetOffsetVal(50 * (selectedCategory - 1), -10);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1806}}<syntaxhighlight lang="lua">button:SetOffsetVal( (buttonAdded % numberOfButtonsPerRow) * buttonSize + buttonPadding, math.floor(buttonAdded / numberOfButtonsPerRow) * buttonSize + buttonPadding );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|2085}}<syntaxhighlight lang="lua">thisBuildingInstance.UnlockedBuildingButton:SetOffsetVal( (buttonAdded % numberOfButtonsPerRow) * buttonSize + buttonPadding, math.floor(buttonAdded / numberOfButtonsPerRow) * buttonSize + buttonPadding );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|2943}}<syntaxhighlight lang="lua">thisBuildingInstance.RequiredBuildingButton:SetOffsetVal( (buttonAdded % numberOfButtonsPerRow) * buttonSize + buttonPadding, math.floor(buttonAdded / numberOfButtonsPerRow) * buttonSize + buttonPadding );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|3550}}<syntaxhighlight lang="lua">thisBuildingInstance.UniqueBuildingButton:SetOffsetVal( (buttonAdded % numberOfButtonsPerRow) * buttonSize + buttonPadding, math.floor(buttonAdded / numberOfButtonsPerRow) * buttonSize + buttonPadding );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|3581}}<syntaxhighlight lang="lua">thisImprovementInstance.UniqueImprovementButton:SetOffsetVal( (buttonAdded % numberOfButtonsPerRow) * buttonSize + buttonPadding, math.floor(buttonAdded / numberOfButtonsPerRow) * buttonSize + buttonPadding );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|EnemyUnitPanel.lua}}
:<code>UI/InGame/WorldView/EnemyUnitPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1705}}<syntaxhighlight lang="lua">Controls.MyDeltaBar:SetOffsetVal( 0, healthBarSize.y + 4 );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1707}}<syntaxhighlight lang="lua">Controls.MyDeltaBar:SetOffsetVal( 0, 2 );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1750}}<syntaxhighlight lang="lua">Controls.TheirDeltaBar:SetOffsetVal( 0, healthBarSize.y + 4 );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1752}}<syntaxhighlight lang="lua">Controls.TheirDeltaBar:SetOffsetVal( 0, 2 );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|InstalledPanel.lua}}
:<code>UI/FrontEnd/Modding/InstalledPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0735}}<syntaxhighlight lang="lua">Controls.DetailValuesStack:SetOffsetVal(details_size.x - max_detail_value_width, 0);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0737}}<syntaxhighlight lang="lua">Controls.DetailLabelsStack:SetOffsetVal(details_size.x - max_detail_value_width - spacer -  max_detail_label_width, 0);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|MPGameSetupScreen.lua}}
:<code>UI/FrontEnd/Multiplayer/GameSetup/MPGameSetupScreen.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0162}}<syntaxhighlight lang="lua">Controls.OptionsScrollPanel:SetOffsetVal( 40, 44 );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|NotificationPanel.lua}}
:<code>UI/InGame/WorldView/NotificationPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0371}}<syntaxhighlight lang="lua">Controls.SmallScrollPanel:SetOffsetVal( 20, 0 );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0373}}<syntaxhighlight lang="lua">Controls.SmallScrollPanel:SetOffsetVal( 0, 0 );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ProductionPopup.lua}}
:<code>UI/InGame/Popups/ProductionPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0035}}<syntaxhighlight lang="lua">Controls.ScrollBar:SetOffsetVal( 15, 18 );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0037}}<syntaxhighlight lang="lua">Controls.DownButton:SetOffsetVal( 15, screenSizeY - 414 );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|SocialPolicyPopup.lua}}
:<code>UI/InGame/Popups/SocialPolicyPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0703}}<syntaxhighlight lang="lua">pipe.ConnectorImage:SetOffsetVal( xOffset, (prereq.GridY-1)*g_PolicyPipeYOffset + 58 );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0712}}<syntaxhighlight lang="lua">pipe.ConnectorImage:SetOffsetVal( xOffset + 16, (prereq.GridY-1 + thisPipe.yOffset)*g_PolicyPipeYOffset + 58 );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0752}}<syntaxhighlight lang="lua">startPipe.ConnectorImage:SetOffsetVal( xOffset, (policy.GridY-1)*g_PolicyPipeYOffset + 48 );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0757}}<syntaxhighlight lang="lua">pipe.ConnectorImage:SetOffsetVal( xOffset, (policy.GridY-1)*g_PolicyPipeYOffset + 58 );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0760}}<syntaxhighlight lang="lua">pipe.ConnectorImage:SetOffsetVal( xOffset, (policy.GridY-1 + thisPipe.yOffset)*g_PolicyPipeYOffset + 58 );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0804}}<syntaxhighlight lang="lua">startPipe.ConnectorImage:SetOffsetVal( xOffset, (policy.GridY-1)*g_PolicyPipeYOffset + 0 );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0809}}<syntaxhighlight lang="lua">pipe.ConnectorImage:SetOffsetVal( xOffset, (policy.GridY-1)*g_PolicyPipeYOffset - 10 );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0886}}<syntaxhighlight lang="lua">controlTable.PolicyIcon:SetOffsetVal((policyInfo.GridX-1)*g_PolicyXOffset+16,(policyInfo.GridY-1)*g_PolicyYOffset+12);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TechTree.lua}}
:<code>UI/InGame/TechTree/TechTree.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0152}}<syntaxhighlight lang="lua">hConnection.TechPipeIcon:SetOffsetVal(prereq.GridX*blockSpacingX + blockSizeX + 96, (prereq.GridY-5)*blockSpacingY + 12 + extraYOffset);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0160}}<syntaxhighlight lang="lua">vConnection.TechPipeIcon:SetOffsetVal((tech.GridX-1)*blockSpacingX + blockSizeX + 96, ((tech.GridY-5)*blockSpacingY) - (((tech.GridY-prereq.GridY) * blockSpacingY) / 2) + extraYOffset);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0202}}<syntaxhighlight lang="lua">startPipe.TechPipeIcon:SetOffsetVal( tech.GridX*blockSpacingX + blockSizeX + 64, yOffset );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0208}}<syntaxhighlight lang="lua">pipe.TechPipeIcon:SetOffsetVal( (tech.GridX)*blockSpacingX + blockSizeX + 96, yOffset );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0211}}<syntaxhighlight lang="lua">pipe.TechPipeIcon:SetOffsetVal( (tech.GridX+thisPipe.xOffset)*blockSpacingX + blockSizeX + 96 - 12, yOffset - 15 );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0225}}<syntaxhighlight lang="lua">pipe.TechPipeIcon:SetOffsetVal( (tech.GridX+thisPipe.xOffset)*blockSpacingX + blockSizeX + 96 - 12, yOffset );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0235}}<syntaxhighlight lang="lua">pipe.TechPipeIcon:SetOffsetVal( (tech.GridX)*blockSpacingX + blockSizeX + 96 - 12, yOffset );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0269}}<syntaxhighlight lang="lua">startPipe.TechPipeIcon:SetOffsetVal( tech.GridX*blockSpacingX + 26, yOffset );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0275}}<syntaxhighlight lang="lua">pipe.TechPipeIcon:SetOffsetVal( (tech.GridX)*blockSpacingX, yOffset );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0278}}<syntaxhighlight lang="lua">pipe.TechPipeIcon:SetOffsetVal( (tech.GridX)*blockSpacingX, yOffset - 15);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0458}}<syntaxhighlight lang="lua">thisTechButtonInstance.TechButton:SetOffsetVal( tech.GridX*blockSpacingX + 64, (tech.GridY-5)*blockSpacingY + extraYOffset);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|UnitPanel.lua}}
:<code>UI/InGame/WorldView/UnitPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0225}}<syntaxhighlight lang="lua">instance.UnitActionButton:SetOffsetVal( (numBuildActions % numberOfButtonsPerRow) * buttonSize + buttonPadding + buttonOffsetX, math.floor(numBuildActions / numberOfButtonsPerRow) * buttonSize + buttonPadding + buttonOffsetY );</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|SetOffsetVal]]