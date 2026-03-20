{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This method is declared by {{Type5|AlphaAnim}}, {{Type5|Context}}, {{Type5|Grid}}, {{Type5|Image}}, {{Type5|ScrollAnim}} and {{Type5|Stack}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''void''' UIElement:SetTextureOffset<b>(</b>{{Type5|Vector2}} questionOffset<b>)</b></code>


'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|questionOffset:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|CivilopediaScreen.lua}}
:<code>UI/Civilopedia/CivilopediaScreen.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1805}}<syntaxhighlight lang="lua">image:SetTextureOffset( textureOffset );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|2081}}<syntaxhighlight lang="lua">thisBuildingInstance.UnlockedBuildingImage:SetTextureOffset( nullOffset );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|2939}}<syntaxhighlight lang="lua">thisBuildingInstance.RequiredBuildingImage:SetTextureOffset( nullOffset );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|3546}}<syntaxhighlight lang="lua">thisBuildingInstance.UniqueBuildingImage:SetTextureOffset( nullOffset );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|3577}}<syntaxhighlight lang="lua">thisImprovementInstance.UniqueImprovementImage:SetTextureOffset( nullOffset );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|EnemyUnitPanel.lua}}
:<code>UI/InGame/WorldView/EnemyUnitPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0069}}<syntaxhighlight lang="lua">Controls.UnitIcon:SetTextureOffset( textureOffset );</syntaxhighlight>
{{CodeLine5|0070}}<syntaxhighlight lang="lua">Controls.UnitIconShadow:SetTextureOffset( textureOffset );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0117}}<syntaxhighlight lang="lua">Controls.UnitPortrait:SetTextureOffset(textureOffset);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|EspionageOverview.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/Popups/EspionageOverview.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0368}}<syntaxhighlight lang="lua">Controls.AgentRank:SetTextureOffset(rankOffsets[agent.Rank]);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0464}}<syntaxhighlight lang="lua">Controls.AgentActivityIcon:SetTextureOffset(progressBarState.IconOffset);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0544}}<syntaxhighlight lang="lua">agentEntry.AgentRank:SetTextureOffset(rankOffsets[v.Rank]);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0651}}<syntaxhighlight lang="lua">agentEntry.AgentActivityIcon:SetTextureOffset(progressBarState.IconOffset);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|FoRScenarioLoadScreen.lua (G&K)}}
:<code>DLC/Expansion/Scenarios/FallOfRomeScenario/FoRScenarioLoadScreen.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0158}}<syntaxhighlight lang="lua">controlTable.Icon:SetTextureOffset( questionOffset );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0160}}<syntaxhighlight lang="lua">controlTable.IconShadow:SetTextureOffset( questionOffset );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0216}}<syntaxhighlight lang="lua">controlTable.Icon:SetTextureOffset( textureOffset );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0218}}<syntaxhighlight lang="lua">controlTable.IconShadow:SetTextureOffset( textureOffset );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0289}}<syntaxhighlight lang="lua">Controls.IconShadow:SetTextureOffset( questionOffset );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|GameSetupScreen.lua}}
:<code>UI/FrontEnd/GameSetup/GameSetupScreen.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0512}}<syntaxhighlight lang="lua">Controls[buttonName]:SetTextureOffset( questionOffset );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|HallOfFame.lua}}
:<code>UI/InGame/Popups/HallOfFame.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0096}}<syntaxhighlight lang="lua">controlTable.WinCivIcon:SetTextureOffset( textureOffset );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0098}}<syntaxhighlight lang="lua">controlTable.CivIconShadow:SetTextureOffset( textureOffset );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|IconSupport.lua}}
:<code>UI/IconSupport.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0172}}<syntaxhighlight lang="lua">iconControl:SetTextureOffset( textureOffset );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|LoadMenu.lua}}
:<code>UI/FrontEnd/LoadMenu.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0274}}<syntaxhighlight lang="lua">Controls.CivIcon:SetTextureOffset(questionOffset);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0286}}<syntaxhighlight lang="lua">Controls.CivIcon:SetTextureOffset( textureOffset );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0369}}<syntaxhighlight lang="lua">Controls.MapSize:SetTextureOffset( questionOffset );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0382}}<syntaxhighlight lang="lua">Controls.Handicap:SetTextureOffset( questionOffset );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0395}}<syntaxhighlight lang="lua">Controls.SpeedIcon:SetTextureOffset( questionOffset );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0478}}<syntaxhighlight lang="lua">Controls.CivIcon:SetTextureOffset( questionOffset );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0483}}<syntaxhighlight lang="lua">Controls.MapType:SetTextureOffset( questionOffset );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ProductionPopup.lua}}
:<code>UI/InGame/Popups/ProductionPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0916}}<syntaxhighlight lang="lua">controlTable.ProductionButtonImage:SetTextureOffset(textureOffset);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|SelectCivilization.lua}}
:<code>UI/FrontEnd/GameSetup/SelectCivilization.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0096}}<syntaxhighlight lang="lua">controlTable.CivIcon:SetTextureOffset( questionOffset );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0128}}<syntaxhighlight lang="lua">controlTable.CivIcon:SetTextureOffset( textureOffset );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TechButtonInclude.lua}}
:<code>UI/InGame/TechTree/TechButtonInclude.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0353}}<syntaxhighlight lang="lua">thisButton:SetTextureOffset( textureOffset );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TechTree.lua}}
:<code>UI/InGame/TechTree/TechTree.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0213}}<syntaxhighlight lang="lua">pipe.TechPipeIcon:SetTextureOffset(Vector2(72,72));</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0227}}<syntaxhighlight lang="lua">pipe.TechPipeIcon:SetTextureOffset(Vector2(72,0));</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0280}}<syntaxhighlight lang="lua">pipe.TechPipeIcon:SetTextureOffset(Vector2(0,72));</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0294}}<syntaxhighlight lang="lua">pipe.TechPipeIcon:SetTextureOffset(Vector2(0,0));</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|UnitPanel.lua}}
:<code>UI/InGame/WorldView/UnitPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0444}}<syntaxhighlight lang="lua">Controls.UnitIcon:SetTextureOffset(textureOffset);</syntaxhighlight>
{{CodeLine5|0445}}<syntaxhighlight lang="lua">Controls.UnitIconShadow:SetTextureOffset(textureOffset);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|VoteResultsPopup.lua}}
:<code>UI/InGame/Popups/VoteResultsPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0059}}<syntaxhighlight lang="lua">controlTable.Portrait:SetTextureOffset( questionOffset );</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|SetTextureOffset]]