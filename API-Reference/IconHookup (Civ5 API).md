{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a global function. Use: <code>include("IconSupport.lua")</code>
}}


=Usage=
<code>'''bool''' IconHookup<b>(</b>'''int''' offset, '''float''' iconSize, '''string''' atlas, {{Type5|Image}} imageControl, '''unknown''' debugPrint = nil<b>)</b></code>


'''Returned Value'''
:No description available.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|offset:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|iconSize:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|atlas:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|imageControl:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|debugPrint:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Too many occurences. Only 50 out of 457 are listed.''

{{PseudoH4|AdvancedSetup.lua}}
:<code>UI/FrontEnd/GameSetup/AdvancedSetup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0315}}<syntaxhighlight lang="lua">IconHookup( 22, 64, "LEADER_ATLAS", controlTable.Portrait );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ChangePassword.lua}}
:<code>UI/InGame/ChangePassword.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0116}}<syntaxhighlight lang="lua">IconHookup( civ.PortraitIndex, 128, civ.IconAtlas, Controls.Icon );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ChooseFaithGreatPerson.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/Popups/ChooseFaithGreatPerson.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0033}}<syntaxhighlight lang="lua">IconHookup( info.PortraitIndex, 64, info.IconAtlas, controlTable.Icon64 );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ChooseReligionPopup.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/Popups/ChooseReligionPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0466}}<syntaxhighlight lang="lua">IconHookup(portraitIndex, 80, iconAtlas, Controls.ReligionIcon);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CityBannerManager.lua}}
:<code>UI/InGame/CityBannerManager.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0360}}<syntaxhighlight lang="lua">if IconHookup( thisUnitInfo.PortraitIndex, 45, thisUnitInfo.IconAtlas, controls.CityBannerProductionImage ) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0367}}<syntaxhighlight lang="lua">if IconHookup( thisBuildingInfo.PortraitIndex, 45, thisBuildingInfo.IconAtlas, controls.CityBannerProductionImage ) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0418}}<syntaxhighlight lang="lua">IconHookup( civInfo.PortraitIndex, 32, civInfo.AlphaIconAtlas, controls.StatusIcon );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CityBannerManager.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/CityBannerManager.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0203}}<syntaxhighlight lang="lua">IconHookup( religion.PortraitIndex, 32, religion.IconAtlas, controls.ReligiousIcon );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CityList.lua}}
:<code>UI/InGame/CityList.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0403}}<syntaxhighlight lang="lua">if IconHookup( thisProjectInfo.PortraitIndex, g_iPortraitSize, thisProjectInfo.IconAtlas, instance.ProdImage ) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CityStateStatusHelper.lua (G&K)}}
:<code>DLC/Expansion/UI/CityStateStatusHelper.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0134}}<syntaxhighlight lang="lua">IconHookup(kBarIconNeutralIndex, size, kBarIconAtlas, barMarkerCtrl);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CityView.lua}}
:<code>UI/InGame/CityView/CityView.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0325}}<syntaxhighlight lang="lua">if IconHookup( building.PortraitIndex, 64, building.IconAtlas, controlTable.BuildingImage ) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0588}}<syntaxhighlight lang="lua">IconHookup( thisBuildingInfo.PortraitIndex, 45, thisBuildingInfo.IconAtlas, Controls[controlImage] );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0607}}<syntaxhighlight lang="lua">IconHookup( thisProcessInfo.PortraitIndex, 45, thisProcessInfo.IconAtlas, Controls[controlImage] );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0885}}<syntaxhighlight lang="lua">if IconHookup( thisProcessInfo.PortraitIndex, g_iPortraitSize, thisProcessInfo.IconAtlas, Controls.ProductionPortrait ) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1760}}<syntaxhighlight lang="lua">IconHookup(   0, 45, "CITIZEN_ATLAS", controlTable.PlotButtonImage);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1772}}<syntaxhighlight lang="lua">IconHookup(   12, 45, "CITIZEN_ATLAS", controlTable.PlotButtonImage);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CivilopediaScreen.lua}}
:<code>UI/Civilopedia/CivilopediaScreen.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1375}}<syntaxhighlight lang="lua">if IconHookup( portraitIndex, portraitSize, portraitAtlas, Controls.Portrait ) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1618}}<syntaxhighlight lang="lua">if IconHookup( 44, portraitSize, "UNIT_ATLAS_2", Controls.Portrait ) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|2937}}<syntaxhighlight lang="lua">if not IconHookup( thisBuildingInfo.PortraitIndex, buttonSize, thisBuildingInfo.IconAtlas, thisBuildingInstance.RequiredBuildingImage ) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|3264}}<syntaxhighlight lang="lua">if IconHookup( thisPolicy.PortraitIndex, portraitSize, thisPolicy.IconAtlas, Controls.Portrait ) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|3467}}<syntaxhighlight lang="lua">if IconHookup( thisCiv.PortraitIndex, portraitSize, thisCiv.IconAtlas, Controls.Portrait ) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|3575}}<syntaxhighlight lang="lua">if not IconHookup( thisImprovement.PortraitIndex, buttonSize, thisImprovement.IconAtlas, thisImprovementInstance.UniqueImprovementImage ) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|3867}}<syntaxhighlight lang="lua">if IconHookup( thisTerrain.PortraitIndex, portraitSize, thisTerrain.IconAtlas, Controls.Portrait ) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DiploList.lua}}
:<code>UI/InGame/DiploList.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0278}}<syntaxhighlight lang="lua">IconHookup( otherLeaderInfo.PortraitIndex, 64, otherLeaderInfo.IconAtlas, controlTable.LeaderPortrait );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|EnemyUnitPanel.lua}}
:<code>UI/InGame/WorldView/EnemyUnitPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0079}}<syntaxhighlight lang="lua">IconHookup( 0, g_iPortraitSize, "ENEMY_CITY_ATLAS", Controls.UnitPortrait );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|FoRScenarioLoadScreen.lua (G&K)}}
:<code>DLC/Expansion/Scenarios/FallOfRomeScenario/FoRScenarioLoadScreen.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0259}}<syntaxhighlight lang="lua">IconHookup( civ.PortraitIndex, 64, civ.IconAtlas, Controls.IconShadow );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|GameMenu.lua}}
:<code>UI/InGame/Menus/GameMenu.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0271}}<syntaxhighlight lang="lua">IconHookup( 4, 64, "WORLDTYPE_ATLAS", Controls.TypeIcon);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0278}}<syntaxhighlight lang="lua">IconHookup( info.PortraitIndex, 64, info.IconAtlas, Controls.SizeIcon );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0281}}<syntaxhighlight lang="lua">IconHookup( 6, 64, "WORLDSIZE_ATLAS", Controls.SizeIcon );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0288}}<syntaxhighlight lang="lua">IconHookup( info.PortraitIndex, 64, info.IconAtlas, Controls.DifficultyIcon );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|GameSetupScreen.lua}}
:<code>UI/FrontEnd/GameSetup/GameSetupScreen.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0274}}<syntaxhighlight lang="lua">IconHookup( mapScript.IconIndex or 0, 128, mapScript.IconAtlas, Controls.TypeIcon );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0387}}<syntaxhighlight lang="lua">IconHookup(3, 128, "WORLDTYPE_ATLAS", Controls.TypeIcon);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0493}}<syntaxhighlight lang="lua">IconHookup( 22, 128, "LEADER_ATLAS", Controls.Portrait );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|HallOfFame.lua}}
:<code>UI/InGame/Popups/HallOfFame.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0049}}<syntaxhighlight lang="lua">IconHookup( leader.PortraitIndex, 64, leader.IconAtlas, controlTable.LeaderPortrait );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0063}}<syntaxhighlight lang="lua">IconHookup( info.PortraitIndex, 32, info.IconAtlas, controlTable.Difficulty );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|IconSupport.lua}}
:<code>UI/IconSupport.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0245}}<syntaxhighlight lang="lua">IconHookup( 23, iconSize, "CIV_COLOR_ATLAS", iconControl );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|LoadMenu.lua}}
:<code>UI/FrontEnd/LoadMenu.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0356}}<syntaxhighlight lang="lua">IconHookup(4, 64, "WORLDTYPE_ATLAS", Controls.MapType);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|MongolScenarioLoadScreen.lua - DLC_01 DLC}}
:<code>DLC/DLC_01/Scenarios/Mongol Scenario/MongolScenarioLoadScreen.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0115}}<syntaxhighlight lang="lua">IconHookup( civ.PortraitIndex, 80, civ.IconAtlas, Controls.IconShadow );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|NotificationPanel.lua}}
:<code>UI/InGame/WorldView/NotificationPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0196}}<syntaxhighlight lang="lua">IconHookup( portraitIndex, 80, GameInfo.Buildings[iGameValue].IconAtlas, instance.WonderConstructedAlphaAnim );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0227}}<syntaxhighlight lang="lua">IconHookup( portraitIndex, 80, thisResourceInfo.IconAtlas, instance.ResourceImage );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ProductionPopup.lua}}
:<code>UI/InGame/Popups/ProductionPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0571}}<syntaxhighlight lang="lua">if IconHookup( thisProjectInfo.PortraitIndex, 128, thisProjectInfo.IconAtlas, Controls.ProductionPortrait ) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ReligionOverview.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/Popups/ReligionOverview.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0541}}<syntaxhighlight lang="lua">IconHookup(v.FounderIconIndex, 45, v.FounderIconAtlas, entry.FounderIcon);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0629}}<syntaxhighlight lang="lua">IconHookup(v.ReligionIconIndex, 48, v.ReligionIconAtlas, beliefEntry.BeliefReligionIcon);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|SocialPolicyPopup.lua}}
:<code>UI/InGame/Popups/SocialPolicyPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0472}}<syntaxhighlight lang="lua">IconHookup( policyInfo.PortraitIndex, 64, policyInfo.IconAtlas, thisPolicyIcon.PolicyImage );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TechButtonInclude.lua}}
:<code>UI/InGame/TechTree/TechButtonInclude.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0161}}<syntaxhighlight lang="lua">IconHookup( row.PortraitIndex, textureSize, row.IconAtlas, thisButton );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TechPopup.lua}}
:<code>UI/InGame/TechPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0231}}<syntaxhighlight lang="lua">if IconHookup( tech.PortraitIndex, 64, tech.IconAtlas, thisTechButtonInstance.TechPortrait ) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|UnitPanel.lua}}
:<code>UI/InGame/WorldView/UnitPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0122}}<syntaxhighlight lang="lua">IconHookup(iconIndex, actionIconSize, iconAtlas, icon);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0584}}<syntaxhighlight lang="lua">IconHookup( civPortraitIndex, 128, civInfo.IconAtlas, Controls.BackgroundCivSymbol );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|VictoryProgress.lua}}
:<code>UI/InGame/Popups/VictoryProgress.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0841}}<syntaxhighlight lang="lua">IconHookup( leader.PortraitIndex, iconSize, leader.IconAtlas, controlTable );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|VictoryStatus.lua (G&K)}}
:<code>DLC/Expansion/Scenarios/SteampunkScenario/VictoryStatus.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0127}}<syntaxhighlight lang="lua">IconHookup( tLeader.PortraitIndex, 64, tLeader.IconAtlas, gtTokenUI[s].Portrait );</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|IconHookup]]