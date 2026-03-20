{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This method is declared by '''ControlBase'''.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''void''' UIElement:SetSizeY<b>(</b>'''int''' newSizeY<b>)</b></code>


'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|newSizeY:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Too many occurences. Only 50 out of 88 are listed.''

{{PseudoH4|AdvancedSetup.lua}}
:<code>UI/FrontEnd/GameSetup/AdvancedSetup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1300}}<syntaxhighlight lang="lua">Controls.MainGrid:SetSizeY( screenY - TOP_COMPENSATION );</syntaxhighlight>
{{CodeLine5|1301}}<syntaxhighlight lang="lua">Controls.ListingScrollPanel:SetSizeY( screenY - TOP_COMPENSATION - BOTTOM_COMPENSATION - LOCAL_SLOT_COMPENSATION );</syntaxhighlight>
{{CodeLine5|1302}}<syntaxhighlight lang="lua">Controls.OptionsScrollPanel:SetSizeY( screenY - TOP_COMPENSATION - BOTTOM_COMPENSATION );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CityStateDiploPopup.lua}}
:<code>UI/InGame/Popups/CityStateDiploPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0775}}<syntaxhighlight lang="lua">buttonControl:SetSizeY(sizeY);</syntaxhighlight>
{{CodeLine5|0776}}<syntaxhighlight lang="lua">animControl:SetSizeY(sizeY+WordWrapAnimOffset);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CityStateDiploPopup.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/Popups/CityStateDiploPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0042}}<syntaxhighlight lang="lua">buttonHL:SetSizeY(sizeY+WordWrapAnimOffset);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CityView.lua}}
:<code>UI/InGame/CityView/CityView.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1477}}<syntaxhighlight lang="lua">Controls.BuildingListBackground:SetSizeY( size );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1480}}<syntaxhighlight lang="lua">Controls.ScrollPanel:SetSizeY( size );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DiploCorner.lua}}
:<code>UI/InGame/WorldView/DiploCorner.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0171}}<syntaxhighlight lang="lua">controlTable.Box:SetSizeY( controlTable.String:GetSizeY() + 8 );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DiploGlobalRelationships.lua}}
:<code>UI/InGame/Popups/DiploGlobalRelationships.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0296}}<syntaxhighlight lang="lua">controlTable.Button:SetSizeY(newSizeY);</syntaxhighlight>
{{CodeLine5|0297}}<syntaxhighlight lang="lua">controlTable.ButtonAnim:SetSizeY(newSizeY);</syntaxhighlight>
{{CodeLine5|0298}}<syntaxhighlight lang="lua">controlTable.ButtonAnimGrid:SetSizeY(newSizeY+5);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DiploList.lua}}
:<code>UI/InGame/DiploList.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0037}}<syntaxhighlight lang="lua">Controls.OuterGrid:SetSizeY( MAX_SIZE );</syntaxhighlight>
{{CodeLine5|0038}}<syntaxhighlight lang="lua">Controls.ScrollPanel:SetSizeY( MAX_SIZE - PANEL_OFFSET );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0585}}<syntaxhighlight lang="lua">Controls.OuterGrid:SetSizeY( size );</syntaxhighlight>
{{CodeLine5|0586}}<syntaxhighlight lang="lua">Controls.ScrollPanel:SetSizeY( size - PANEL_OFFSET );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DiploRelationships.lua}}
:<code>UI/InGame/Popups/DiploRelationships.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0095}}<syntaxhighlight lang="lua">controlTable.LeaderButton:SetSizeY(buttonY);</syntaxhighlight>
{{CodeLine5|0096}}<syntaxhighlight lang="lua">controlTable.LeaderButtonHL:SetSizeY(buttonY);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0215}}<syntaxhighlight lang="lua">controlTable.LeaderNameStack:SetSizeY(buttonY);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0221}}<syntaxhighlight lang="lua">controlTable.DiploButton:SetSizeY(buttonY);</syntaxhighlight>
{{CodeLine5|0222}}<syntaxhighlight lang="lua">controlTable.DiploButtonHL:SetSizeY(buttonY);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0606}}<syntaxhighlight lang="lua">pStack.ResourcesLabel:SetSizeY(resourceY);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DiscussionDialog.lua}}
:<code>UI/InGame/LeaderHead/DiscussionDialog.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0154}}<syntaxhighlight lang="lua">Controls.LeaderSpeechBorderFrame:SetSizeY( contentSize );</syntaxhighlight>
{{CodeLine5|0155}}<syntaxhighlight lang="lua">Controls.LeaderSpeechFrame:SetSizeY( contentSize - offsetsBetweenFrames );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|EndGameMenu.lua}}
:<code>UI/InGame/Popups/EndGameMenu.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0210}}<syntaxhighlight lang="lua">Controls.GameOverContainer:SetSizeY(sizeY + 30);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|EnemyUnitPanel.lua}}
:<code>UI/InGame/WorldView/EnemyUnitPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0556}}<syntaxhighlight lang="lua">Controls.DetailsSeperator:SetSizeY( Controls.DetailsGrid:GetSizeY() );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|HallOfFame.lua}}
:<code>UI/InGame/Popups/HallOfFame.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0174}}<syntaxhighlight lang="lua">controlTable.GameItem:SetSizeY(itemY);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|Lobby.lua}}
:<code>UI/FrontEnd/Multiplayer/Lobby.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0545}}<syntaxhighlight lang="lua">Controls.ListingStack:SetSizeY( SIZE );</syntaxhighlight>
{{CodeLine5|0546}}<syntaxhighlight lang="lua">Controls.ListingScrollPanel:SetSizeY( SIZE );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|MPGameSetupScreen.lua}}
:<code>UI/FrontEnd/Multiplayer/GameSetup/MPGameSetupScreen.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0168}}<syntaxhighlight lang="lua">Controls.OptionsScrollPanel:SetSizeY( SIZE );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|MPList.lua}}
:<code>UI/InGame/WorldView/MPList.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0018}}<syntaxhighlight lang="lua">Controls.MPListScroll:SetSizeY( screenY - MINIMAP_GUESS - TOP_COMPENSATION - CHAT_COMPENSATION );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|NotificationLogPopup.lua}}
:<code>UI/InGame/Popups/NotificationLogPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0067}}<syntaxhighlight lang="lua">controlTable.Button:SetSizeY(sizeY);</syntaxhighlight>
{{CodeLine5|0068}}<syntaxhighlight lang="lua">controlTable.TextAnim:SetSizeY(sizeY);</syntaxhighlight>
{{CodeLine5|0069}}<syntaxhighlight lang="lua">controlTable.TextHL:SetSizeY(sizeY);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|NotificationPanel.lua}}
:<code>UI/InGame/WorldView/NotificationPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0364}}<syntaxhighlight lang="lua">Controls.SmallScrollPanel:SetSizeY( g_SmallScrollMax - bigY );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|Ranking.lua}}
:<code>UI/InGame/Popups/Ranking.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0045}}<syntaxhighlight lang="lua">controlTable.MainStack:SetSizeY(buttonY);</syntaxhighlight>
{{CodeLine5|0046}}<syntaxhighlight lang="lua">controlTable.SelectHighlight:SetSizeY(buttonY);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|StagingRoom.lua}}
:<code>UI/FrontEnd/Multiplayer/StagingRoom.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0793}}<syntaxhighlight lang="lua">Controls.OptionsScrollPanel:SetSizeY( Controls.VerticalTrim:GetSizeY() - 2);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1191}}<syntaxhighlight lang="lua">controlTable.Box:SetSizeY( controlTable.String:GetSizeY() + 15 );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1354}}<syntaxhighlight lang="lua">Controls.ListingScrollPanel:SetSizeY( screenY - TOP_COMPENSATION - LOCAL_SLOT_COMPENSATION - BOTTOM_COMPENSATION - TOP_FRAME );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1357}}<syntaxhighlight lang="lua">Controls.VerticalTrim:SetSizeY( screenY - TOP_COMPENSATION - BOTTOM_COMPENSATION - TOP_FRAME );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TechPopup.lua}}
:<code>UI/InGame/TechPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0106}}<syntaxhighlight lang="lua">Controls.ScrollPanelBlackFrame:SetSizeY( screenY );</syntaxhighlight>
{{CodeLine5|0107}}<syntaxhighlight lang="lua">Controls.ScrollPanelFrame:SetSizeY( screenY );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0109}}<syntaxhighlight lang="lua">Controls.ScrollPanel:SetSizeY( screenY - 244 );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0111}}<syntaxhighlight lang="lua">Controls.ScrollPanel:SetSizeY( screenY - 300 );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|UnitList.lua}}
:<code>UI/InGame/UnitList.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0208}}<syntaxhighlight lang="lua">instance.StatusBox:SetSizeY(statusY);</syntaxhighlight>
{{CodeLine5|0209}}<syntaxhighlight lang="lua">instance.SelectionFrame:SetSizeY(statusY);</syntaxhighlight>
{{CodeLine5|0210}}<syntaxhighlight lang="lua">instance.Root:SetSizeY(statusY);</syntaxhighlight>
{{CodeLine5|0211}}<syntaxhighlight lang="lua">instance.SelectHL:SetSizeY(statusY);</syntaxhighlight>
{{CodeLine5|0212}}<syntaxhighlight lang="lua">instance.SelectAnim:SetSizeY(statusY);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|SetSizeY]]