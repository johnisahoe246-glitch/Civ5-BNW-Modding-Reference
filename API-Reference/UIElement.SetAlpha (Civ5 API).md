{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This method is declared by '''ControlBase'''.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''void''' UIElement:SetAlpha<b>(</b>'''float''' DimAlpha<b>)</b></code>


'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|DimAlpha:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Too many occurences. Only 50 out of 126 are listed.''

{{PseudoH4|EconomicGeneralInfo.lua}}
:<code>UI/InGame/Popups/EconomicGeneralInfo.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0218}}<syntaxhighlight lang="lua">Controls.CityToggle:SetAlpha( 1.0 );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0221}}<syntaxhighlight lang="lua">Controls.CityToggle:SetAlpha( 0.5 );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0269}}<syntaxhighlight lang="lua">Controls.TradeToggle:SetAlpha( 1.0 );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0272}}<syntaxhighlight lang="lua">Controls.TradeToggle:SetAlpha( 0.5 );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0339}}<syntaxhighlight lang="lua">Controls.BuildingsToggle:SetAlpha( 1.0 );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0342}}<syntaxhighlight lang="lua">Controls.BuildingsToggle:SetAlpha( 0.5 );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|EspionageOverview.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/Popups/EspionageOverview.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0978}}<syntaxhighlight lang="lua">entry.CivilizationName:SetAlpha(1.0);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0980}}<syntaxhighlight lang="lua">entry.CityName:SetAlpha(1.0);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1011}}<syntaxhighlight lang="lua">entry.CityPopulation:SetAlpha(1.0);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1067}}<syntaxhighlight lang="lua">cityEntry.CivilizationName:SetAlpha(0.4);</syntaxhighlight>
{{CodeLine5|1068}}<syntaxhighlight lang="lua">cityEntry.CityName:SetAlpha(0.4);</syntaxhighlight>
{{CodeLine5|1069}}<syntaxhighlight lang="lua">cityEntry.CityPopulation:SetAlpha(0.4);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|HappinessInfo.lua}}
:<code>UI/InGame/Popups/HappinessInfo.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0231}}<syntaxhighlight lang="lua">Controls.LuxuryHappinessToggle:SetAlpha( 1.0 );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0287}}<syntaxhighlight lang="lua">Controls.CityBuildingToggle:SetAlpha( 1.0 );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0589}}<syntaxhighlight lang="lua">Controls.CityUnhappinessToggle:SetAlpha( 1.0 );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0592}}<syntaxhighlight lang="lua">Controls.CityUnhappinessToggle:SetAlpha( 0.5 );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0640}}<syntaxhighlight lang="lua">Controls.ResourcesAvailableToggle:SetAlpha( 1.0 );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0643}}<syntaxhighlight lang="lua">Controls.ResourcesAvailableToggle:SetAlpha( 0.5 );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0684}}<syntaxhighlight lang="lua">Controls.ResourcesImportedToggle:SetAlpha( 0.5 );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0723}}<syntaxhighlight lang="lua">Controls.ResourcesExportedToggle:SetAlpha( 1.0 );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0726}}<syntaxhighlight lang="lua">Controls.ResourcesExportedToggle:SetAlpha( 0.5 );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0764}}<syntaxhighlight lang="lua">Controls.ResourcesLocalToggle:SetAlpha( 1.0 );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0767}}<syntaxhighlight lang="lua">Controls.ResourcesLocalToggle:SetAlpha( 0.5 );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|MilitaryOverview.lua}}
:<code>UI/InGame/Popups/MilitaryOverview.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0167}}<syntaxhighlight lang="lua">instance.Button:SetAlpha( 0.6 );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|MiniMapPanel.lua}}
:<code>UI/InGame/WorldView/MiniMapPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0036}}<syntaxhighlight lang="lua">Controls.ShowResources:SetAlpha( 0.5 );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0043}}<syntaxhighlight lang="lua">Controls.ShowResources:SetAlpha( 1.0 );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|MPList.lua}}
:<code>UI/InGame/WorldView/MPList.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0180}}<syntaxhighlight lang="lua">controlTable.Name:SetAlpha( 0.5 );</syntaxhighlight>
{{CodeLine5|0181}}<syntaxhighlight lang="lua">controlTable.IconBox:SetAlpha( 0.2 );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0184}}<syntaxhighlight lang="lua">controlTable.IconBox:SetAlpha( 1 );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|OptionsMenu.lua}}
:<code>UI/Options/OptionsMenu.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0307}}<syntaxhighlight lang="lua">Controls.TutorialPull:SetAlpha( 0.5 );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0312}}<syntaxhighlight lang="lua">Controls.TutorialPull:SetAlpha( 1.0 );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0314}}<syntaxhighlight lang="lua">Controls.ResetTutorialButton:SetAlpha( 1.0 );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0320}}<syntaxhighlight lang="lua">Controls.MPQuickCombatCheckbox:SetAlpha( 0.5 );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0322}}<syntaxhighlight lang="lua">Controls.MPQuickMovementCheckbox:SetAlpha( 0.5 );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0325}}<syntaxhighlight lang="lua">Controls.MPQuickCombatCheckbox:SetAlpha( 1.0 );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0327}}<syntaxhighlight lang="lua">Controls.MPQuickMovementCheckbox:SetAlpha( 1.0 );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0334}}<syntaxhighlight lang="lua">Controls.LanguagePull:SetAlpha( 0.5 );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0336}}<syntaxhighlight lang="lua">Controls.SpokenLanguagePull:SetAlpha( 0.5 );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0338}}<syntaxhighlight lang="lua">Controls.AutoUIAssetsCheck:SetAlpha( 0.5 );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0340}}<syntaxhighlight lang="lua">Controls.SmallUIAssetsCheck:SetAlpha( 0.5 );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1183}}<syntaxhighlight lang="lua">controlTable.Button:SetAlpha(.3);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ProductionPopup.lua}}
:<code>UI/InGame/Popups/ProductionPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1022}}<syntaxhighlight lang="lua">controlTable.Button:SetAlpha( 0.4 );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1024}}<syntaxhighlight lang="lua">controlTable.Button:SetAlpha( 1.0 );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TradeLogic.lua}}
:<code>UI/InGame/WorldView/TradeLogic.lua</code>
:{{CodeBegin5}}
{{CodeLine5|2564}}<syntaxhighlight lang="lua">g_OtherPlayersButtons[ iLoopPlayer ][ SubTableName ].Button:SetAlpha( 1 );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|2568}}<syntaxhighlight lang="lua">g_OtherPlayersButtons[ iLoopPlayer ][ SubTableName ].Button:SetAlpha( 0.5 );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|UnitFlagManager.lua}}
:<code>UI/InGame/UnitFlagManager.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0783}}<syntaxhighlight lang="lua">self.m_Instance.Anchor:SetAlpha( g_DimAlpha );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0796}}<syntaxhighlight lang="lua">self.m_Instance.Anchor:SetAlpha( 1.0 );</syntaxhighlight>
{{CodeLine5|0797}}<syntaxhighlight lang="lua">self.m_Instance.HealthBar:SetAlpha( 1.0 );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|UnitPanel.lua}}
:<code>UI/InGame/WorldView/UnitPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0263}}<syntaxhighlight lang="lua">instance.UnitActionButton:SetAlpha( 0.4 );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0266}}<syntaxhighlight lang="lua">instance.UnitActionButton:SetAlpha( 1.0 );</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|SetAlpha]]