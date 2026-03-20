{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This method is declared by '''ControlBase'''.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''void''' UIElement:SetColor<b>(</b>'''table''' fadeColor, '''int''' arg1<b>)</b></code>


'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|fadeColor:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|arg1:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Too many occurences. Only 50 out of 145 are listed.''

{{PseudoH4|CityBannerManager.lua}}
:<code>UI/InGame/CityBannerManager.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0112}}<syntaxhighlight lang="lua">controls.CityBannerBackground:SetColor(backgroundColor);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0114}}<syntaxhighlight lang="lua">controls.CityBannerBGLeftHL:SetColor( backgroundColor );</syntaxhighlight>
{{CodeLine5|0115}}<syntaxhighlight lang="lua">controls.CityBannerBGRightHL:SetColor( backgroundColor );</syntaxhighlight>
{{CodeLine5|0116}}<syntaxhighlight lang="lua">controls.CityBannerRightBackground:SetColor( backgroundColor );</syntaxhighlight>
{{CodeLine5|0117}}<syntaxhighlight lang="lua">controls.CityBannerLeftBackground:SetColor( backgroundColor );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0134}}<syntaxhighlight lang="lua">controls.CityProductionName:SetColor(textColor200, 0);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0137}}<syntaxhighlight lang="lua">controls.CityName:SetColor(textColor, 0);</syntaxhighlight>
{{CodeLine5|0138}}<syntaxhighlight lang="lua">controls.CityName:SetColor(textColorShadow, 1);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CityStateDiploPopup.lua}}
:<code>UI/InGame/Popups/CityStateDiploPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0089}}<syntaxhighlight lang="lua">Controls.TitleLabel:SetColor(textColor, 0);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0103}}<syntaxhighlight lang="lua">Controls.CivIcon:SetColor(iconColor);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DiploList.lua}}
:<code>UI/InGame/DiploList.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0438}}<syntaxhighlight lang="lua">controlTable.MinorName:SetColor( color, 0 );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0463}}<syntaxhighlight lang="lua">controlTable.LeaderPortrait:SetColor( color );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0551}}<syntaxhighlight lang="lua">controls.StatusIcon:SetColor( {x=1, y=1, z=1, w=1 } );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0560}}<syntaxhighlight lang="lua">controls.StatusIcon:SetColor(color);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DiploList.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/DiploList.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0485}}<syntaxhighlight lang="lua">controlTable.StatusIcon:SetColor( {x=1, y=1, z=1, w=1 } );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DiploRelationships.lua}}
:<code>UI/InGame/Popups/DiploRelationships.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0083}}<syntaxhighlight lang="lua">controlTable.LeaderPortrait:SetColor(iconColor);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|EndGameMenu.lua}}
:<code>UI/InGame/Popups/EndGameMenu.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0225}}<syntaxhighlight lang="lua">Controls.BackgroundImage:SetColor({x=1,y=1,z=1,w=1});</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0237}}<syntaxhighlight lang="lua">Controls.BackgroundImage:SetColor({x=1,y=1,z=1,w=0.125});</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|EnemyUnitPanel.lua}}
:<code>UI/InGame/WorldView/EnemyUnitPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0076}}<syntaxhighlight lang="lua">Controls.UnitBackColor:SetColor( flagColor );</syntaxhighlight>
{{CodeLine5|0077}}<syntaxhighlight lang="lua">Controls.UnitIcon:SetColor( iconColor );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|EspionageOverview.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/Popups/EspionageOverview.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1018}}<syntaxhighlight lang="lua">entry.CivilizationName:SetColor(textColor, 0);</syntaxhighlight>
{{CodeLine5|1019}}<syntaxhighlight lang="lua">entry.CityName:SetColor(textColor, 0);</syntaxhighlight>
{{CodeLine5|1020}}<syntaxhighlight lang="lua">entry.CityPopulation:SetColor(textColor, 0);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1140}}<syntaxhighlight lang="lua">entry.CivIcon:SetColor(cityInfo.CivilizationIconColor);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|FoRScenarioLoadScreen.lua (G&K)}}
:<code>DLC/Expansion/Scenarios/FallOfRomeScenario/FoRScenarioLoadScreen.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0165}}<syntaxhighlight lang="lua">controlTable.Icon:SetColor( primaryColorVector );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0169}}<syntaxhighlight lang="lua">controlTable.TeamColor:SetColor( secondaryColorVector );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|HallOfFame.lua}}
:<code>UI/InGame/Popups/HallOfFame.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0085}}<syntaxhighlight lang="lua">controlTable.CivIconBG:SetColor( white );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0104}}<syntaxhighlight lang="lua">controlTable.WinCivIcon:SetColor( primaryColorVector );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0110}}<syntaxhighlight lang="lua">controlTable.CivIconBG:SetColor( secondaryColorVector );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|IconSupport.lua}}
:<code>UI/IconSupport.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0191}}<syntaxhighlight lang="lua">iconControl:SetColor( primaryColorVector );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0210}}<syntaxhighlight lang="lua">teamColorControl:SetColor( primaryColorVector );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0212}}<syntaxhighlight lang="lua">teamColorControl:SetColor( secondaryColorVector );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0229}}<syntaxhighlight lang="lua">teamColorControl:SetColor( white );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|InstalledPanel.lua}}
:<code>UI/FrontEnd/Modding/InstalledPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0823}}<syntaxhighlight lang="lua">listing:SetColor(ListingBoxHighlightColor);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0827}}<syntaxhighlight lang="lua">listing:SetColor(ListingBoxDefaultColor);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|MiniMapPanel.lua}}
:<code>UI/InGame/WorldView/MiniMapPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0238}}<syntaxhighlight lang="lua">controlTable.KeyColor:SetColor(keyColor);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ReplayViewer.lua}}
:<code>UI/InGame/Popups/ReplayViewer.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0263}}<syntaxhighlight lang="lua">messageInstance.MessageText:SetColor(colorVector, 0);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0265}}<syntaxhighlight lang="lua">messageInstance.MessageText:SetColor(defaultColorVector, 0);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|SocialPolicyPopup.lua}}
:<code>UI/InGame/Popups/SocialPolicyPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0379}}<syntaxhighlight lang="lua">thisBack:SetColor( fadeColor );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0397}}<syntaxhighlight lang="lua">thisBack:SetColor( fullColor );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0471}}<syntaxhighlight lang="lua">thisPolicyIcon.PolicyImage:SetColor( fadeColorRV );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|UnitPanel.lua}}
:<code>UI/InGame/WorldView/UnitPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0456}}<syntaxhighlight lang="lua">Controls.UnitIconBackground:SetColor( flagColor );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|VictoryProgress.lua}}
:<code>UI/InGame/Popups/VictoryProgress.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0294}}<syntaxhighlight lang="lua">Controls.ApolloIcon:SetColor(white);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0347}}<syntaxhighlight lang="lua">controlTable[ control ]:SetColor( white );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0441}}<syntaxhighlight lang="lua">Controls.Utopia:SetColor( {x=1, y=1, z=1, w=1 } );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0585}}<syntaxhighlight lang="lua">controlTable.ApolloIcon:SetColor(white);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0793}}<syntaxhighlight lang="lua">controlTable.Utopia:SetColor( {x=1, y=1, z=1, w=1 } );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0923}}<syntaxhighlight lang="lua">controlTable:SetColor(darken);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|VoteResultsPopup.lua}}
:<code>UI/InGame/Popups/VoteResultsPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0093}}<syntaxhighlight lang="lua">controlTable.Portrait:SetColor(textColor);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0161}}<syntaxhighlight lang="lua">controlTable.PlayerNameText:SetColor(backgroundColor, 0);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|SetColor]]
[[Category:Civ5 Players API|SetColor]]