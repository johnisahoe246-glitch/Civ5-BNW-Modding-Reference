{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a global function. Use: <code>include("IconSupport.lua")</code>
}}


=Usage=
<code>{{Type5|Vector2}}, '''string''' IconLookup<b>(</b>'''int''' offset, '''int''' iconSize, '''string''' atlas<b>)</b></code>


'''Returned Values'''
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
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|CivilopediaScreen.lua}}
:<code>UI/Civilopedia/CivilopediaScreen.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0402}}<syntaxhighlight lang="lua">article.tooltipTextureOffset, article.tooltipTexture = IconLookup( tech.PortraitIndex, buttonSize, tech.IconAtlas );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0447}}<syntaxhighlight lang="lua">article.tooltipTextureOffset, article.tooltipTexture = IconLookup( unit.PortraitIndex, buttonSize, unit.IconAtlas );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0706}}<syntaxhighlight lang="lua">article.tooltipTextureOffset, article.tooltipTexture = IconLookup( building.PortraitIndex, buttonSize, building.IconAtlas );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0882}}<syntaxhighlight lang="lua">article.tooltipTextureOffset, article.tooltipTexture = IconLookup( policy.PortraitIndex, buttonSize, policy.IconAtlas );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0904}}<syntaxhighlight lang="lua">article.tooltipTextureOffset, article.tooltipTexture = IconLookup( freePolicy.PortraitIndex, buttonSize, freePolicy.IconAtlas );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0940}}<syntaxhighlight lang="lua">article.tooltipTextureOffset, article.tooltipTexture = IconLookup( person.PortraitIndex, buttonSize, person.IconAtlas );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1006}}<syntaxhighlight lang="lua">article.tooltipTextureOffset, article.tooltipTexture = IconLookup( row.PortraitIndex, buttonSize, row.IconAtlas );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1037}}<syntaxhighlight lang="lua">article.tooltipTextureOffset, article.tooltipTexture = IconLookup( leader.PortraitIndex, buttonSize, leader.IconAtlas );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1202}}<syntaxhighlight lang="lua">article.tooltipTextureOffset, article.tooltipTexture = IconLookup( resource.PortraitIndex, buttonSize, resource.IconAtlas );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|2024}}<syntaxhighlight lang="lua">local textureOffset, textureSheet = IconLookup( prereq.PortraitIndex, buttonSize, prereq.IconAtlas );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|2042}}<syntaxhighlight lang="lua">local textureOffset, textureSheet = IconLookup( leadsTo.PortraitIndex, buttonSize, leadsTo.IconAtlas );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|2060}}<syntaxhighlight lang="lua">local textureOffset, textureSheet = IconLookup( thisUnitInfo.PortraitIndex, buttonSize, thisUnitInfo.IconAtlas );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|2109}}<syntaxhighlight lang="lua">local textureOffset, textureSheet = IconLookup( thisProjectInfo.PortraitIndex, buttonSize, thisProjectInfo.IconAtlas );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|2127}}<syntaxhighlight lang="lua">local textureOffset, textureSheet = IconLookup( revealedResource.PortraitIndex, buttonSize, revealedResource.IconAtlas );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|2144}}<syntaxhighlight lang="lua">local textureOffset, textureSheet = IconLookup( thisBuildInfo.IconIndex, buttonSize, thisBuildInfo.IconAtlas );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|2410}}<syntaxhighlight lang="lua">local textureOffset, textureSheet = IconLookup( promotion.PortraitIndex, buttonSize, promotion.IconAtlas );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|2434}}<syntaxhighlight lang="lua">local textureOffset, textureSheet = IconLookup( requiredResource.PortraitIndex, buttonSize, requiredResource.IconAtlas );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|2476}}<syntaxhighlight lang="lua">local textureOffset, textureSheet = IconLookup( obs.PortraitIndex, buttonSize, obs.IconAtlas );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|2516}}<syntaxhighlight lang="lua">local textureOffset, textureSheet = IconLookup( upgradeUnit.PortraitIndex, buttonSize, upgradeUnit.IconAtlas );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|2550}}<syntaxhighlight lang="lua">local textureOffset, textureSheet = IconLookup( defaultUnit.PortraitIndex, buttonSize, defaultUnit.IconAtlas );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|2566}}<syntaxhighlight lang="lua">local textureOffset, textureSheet = IconLookup( thisCiv.PortraitIndex, buttonSize, thisCiv.IconAtlas );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|2646}}<syntaxhighlight lang="lua">local textureOffset, textureSheet = IconLookup( thisReq.PortraitIndex, buttonSize, thisReq.IconAtlas );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|2913}}<syntaxhighlight lang="lua">local textureOffset, textureSheet = IconLookup( thisSpec.PortraitIndex, buttonSize, thisSpec.IconAtlas );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|3023}}<syntaxhighlight lang="lua">local textureOffset, textureSheet = IconLookup( defaultBuilding.PortraitIndex, buttonSize, defaultBuilding.IconAtlas );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|3304}}<syntaxhighlight lang="lua">local textureOffset, textureSheet = IconLookup( requiredPolicy.PortraitIndex, buttonSize, requiredPolicy.IconAtlas );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|3483}}<syntaxhighlight lang="lua">local textureOffset, textureSheet = IconLookup( leader.PortraitIndex, buttonSize, leader.IconAtlas );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|3945}}<syntaxhighlight lang="lua">local textureOffset, textureSheet = IconLookup( thisFeature.PortraitIndex, buttonSize, thisFeature.IconAtlas );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|3966}}<syntaxhighlight lang="lua">local textureOffset, textureSheet = IconLookup( thisResource.PortraitIndex, buttonSize, thisResource.IconAtlas );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|4084}}<syntaxhighlight lang="lua">local textureOffset, textureSheet = IconLookup( thisTerrain.PortraitIndex, buttonSize, thisTerrain.IconAtlas );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|4267}}<syntaxhighlight lang="lua">local textureOffset, textureSheet = IconLookup( thisImprovement.PortraitIndex, buttonSize, thisImprovement.IconAtlas );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|EnemyUnitPanel.lua}}
:<code>UI/InGame/WorldView/EnemyUnitPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0066}}<syntaxhighlight lang="lua">local textureOffset, textureAtlas = IconLookup( thisCiv.PortraitIndex, 32, thisCiv.AlphaIconAtlas );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0097}}<syntaxhighlight lang="lua">local textureOffset, textureSheet = IconLookup( thisUnitInfo.UnitFlagIconOffset, 32, thisUnitInfo.UnitFlagAtlas );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0111}}<syntaxhighlight lang="lua">textureOffset, textureSheet = IconLookup( thisUnitInfo.PortraitIndex, g_iPortraitSize, thisUnitInfo.IconAtlas );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|FoRScenarioLoadScreen.lua (G&K)}}
:<code>DLC/Expansion/Scenarios/FallOfRomeScenario/FoRScenarioLoadScreen.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0213}}<syntaxhighlight lang="lua">local textureOffset, textureAtlas = IconLookup( civ.PortraitIndex, 64, civ.IconAtlas );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|HallOfFame.lua}}
:<code>UI/InGame/Popups/HallOfFame.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0092}}<syntaxhighlight lang="lua">local textureOffset, textureAtlas = IconLookup( civ.PortraitIndex, 48, civ.AlphaIconAtlas );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|IconSupport.lua}}
:<code>UI/IconSupport.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0168}}<syntaxhighlight lang="lua">local textureOffset, textureAtlas = IconLookup( thisCiv.PortraitIndex, iconSize, thisCiv.AlphaIconAtlas );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ProductionPopup.lua}}
:<code>UI/InGame/Popups/ProductionPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0910}}<syntaxhighlight lang="lua">local textureOffset, textureSheet = IconLookup( thisUnitInfo.PortraitIndex, 45, thisUnitInfo.IconAtlas );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0964}}<syntaxhighlight lang="lua">local textureOffset, textureSheet = IconLookup( thisInfo.PortraitIndex, 45, thisInfo.IconAtlas );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TechButtonInclude.lua}}
:<code>UI/InGame/TechTree/TechButtonInclude.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0392}}<syntaxhighlight lang="lua">local textureOffset, textureSheet = IconLookup( thisProjectInfo.PortraitIndex, textureSize, thisProjectInfo.IconAtlas );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0410}}<syntaxhighlight lang="lua">local textureOffset, textureSheet = IconLookup( thisResourceInfo.PortraitIndex, textureSize, thisResourceInfo.IconAtlas );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0426}}<syntaxhighlight lang="lua">local textureOffset, textureSheet = IconLookup( thisBuildInfo.IconIndex, textureSize, thisBuildInfo.IconAtlas );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|UniqueBonuses.lua}}
:<code>UI/FrontEnd/GameSetup/UniqueBonuses.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0011}}<syntaxhighlight lang="lua">questionOffset, questionTextureSheet = IconLookup( 23, 64, "CIV_COLOR_ATLAS" );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0029}}<syntaxhighlight lang="lua">local textureOffset, textureSheet = IconLookup( thisUnitInfo.PortraitIndex, textureSize, thisUnitInfo.IconAtlas );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0057}}<syntaxhighlight lang="lua">local textureOffset, textureSheet = IconLookup( thisBuildingInfo.PortraitIndex, textureSize, thisBuildingInfo.IconAtlas );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0085}}<syntaxhighlight lang="lua">local textureOffset, textureSheet = IconLookup( thisImprovmentInfo.PortraitIndex, textureSize, thisImprovmentInfo.IconAtlas );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|UnitPanel.lua}}
:<code>UI/InGame/WorldView/UnitPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0441}}<syntaxhighlight lang="lua">local textureOffset, textureAtlas = IconLookup( thisUnitInfo.UnitFlagIconOffset, 32, thisUnitInfo.UnitFlagAtlas );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0459}}<syntaxhighlight lang="lua">textureOffset, textureAtlas = IconLookup( thisUnitInfo.PortraitIndex, unitPortraitSize, thisUnitInfo.IconAtlas );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0500}}<syntaxhighlight lang="lua">local textureOffset, textureAtlas = IconLookup( 0, unitPortraitSize, "CITY_ATLAS" );</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|IconLookup]]