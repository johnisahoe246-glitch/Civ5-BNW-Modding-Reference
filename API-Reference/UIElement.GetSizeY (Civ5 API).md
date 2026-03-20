{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This method is declared by '''ControlBase'''.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''int''' UIElement:GetSizeY<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|AdvancedSetup.lua}}
:<code>UI/FrontEnd/GameSetup/AdvancedSetup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0226}}<syntaxhighlight lang="lua">sizeY = sizeY + gameOption.GameOptionRoot:GetSizeY();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CityStateDiploPopup.lua}}
:<code>UI/InGame/Popups/CityStateDiploPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0774}}<syntaxhighlight lang="lua">local sizeY = textControl:GetSizeY() + WordWrapOffset;</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CityView.lua}}
:<code>UI/InGame/CityView/CityView.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1475}}<syntaxhighlight lang="lua">local size = math.min( screenSizeY + 30, Controls.RightStack:GetSizeY() + 85 );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1479}}<syntaxhighlight lang="lua">size = math.min( screenSizeY - 65, Controls.RightStack:GetSizeY() + 85 );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DiploCorner.lua}}
:<code>UI/InGame/WorldView/DiploCorner.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0171}}<syntaxhighlight lang="lua">controlTable.Box:SetSizeY( controlTable.String:GetSizeY() + 8 );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DiploGlobalRelationships.lua}}
:<code>UI/InGame/Popups/DiploGlobalRelationships.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0284}}<syntaxhighlight lang="lua">print("controlTable.OuterStack:GetSizeY()" .. controlTable.OuterStack:GetSizeY());</syntaxhighlight>
{{CodeLine5|0285}}<syntaxhighlight lang="lua">print("controlTable.PoliciesStack:GetSizeY()" .. controlTable.PoliciesStack:GetSizeY());</syntaxhighlight>
{{CodeLine5|0286}}<syntaxhighlight lang="lua">print("controlTable.WondersStack:GetSizeY()" .. controlTable.WondersStack:GetSizeY());</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0288}}<syntaxhighlight lang="lua">local sizeY = math.max(controlTable.OuterStack:GetSizeY(), controlTable.PoliciesStack:GetSizeY());</syntaxhighlight>
{{CodeLine5|0289}}<syntaxhighlight lang="lua">local sizeY = math.max(sizeY, controlTable.WondersStack:GetSizeY());</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DiploList.lua}}
:<code>UI/InGame/DiploList.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0584}}<syntaxhighlight lang="lua">local size = math.min( MAX_SIZE, Controls.OuterStack:GetSizeY() + 250 );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DiploRelationships.lua}}
:<code>UI/InGame/Popups/DiploRelationships.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0094}}<syntaxhighlight lang="lua">local buttonY = controlTable.CityStack:GetSizeY();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0214}}<syntaxhighlight lang="lua">local buttonY = controlTable.TradeStack:GetSizeY();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0220}}<syntaxhighlight lang="lua">buttonY = controlTable.LeaderButton:GetSizeY();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0605}}<syntaxhighlight lang="lua">local resourceY = pStack.ResourcesInfo:GetSizeY();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|EndGameMenu.lua}}
:<code>UI/InGame/Popups/EndGameMenu.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0209}}<syntaxhighlight lang="lua">local sizeY = Controls.EndGameText:GetSizeY();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|EnemyUnitPanel.lua}}
:<code>UI/InGame/WorldView/EnemyUnitPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0556}}<syntaxhighlight lang="lua">Controls.DetailsSeperator:SetSizeY( Controls.DetailsGrid:GetSizeY() );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|HallOfFame.lua}}
:<code>UI/InGame/Popups/HallOfFame.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0173}}<syntaxhighlight lang="lua">local itemY = controlTable.SettingStack:GetSizeY();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|InstalledPanel.lua}}
:<code>UI/FrontEnd/Modding/InstalledPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0256}}<syntaxhighlight lang="lua">local ph = listing.ProgressBar:GetSizeY();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|MPList.lua}}
:<code>UI/InGame/WorldView/MPList.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0246}}<syntaxhighlight lang="lua">teamEntry.Root:SetSizeY( teamEntry.TeamStack:GetSizeY() + teamEntry.TeamName:GetSizeY() );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|NotificationLogPopup.lua}}
:<code>UI/InGame/Popups/NotificationLogPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0066}}<syntaxhighlight lang="lua">local sizeY = controlTable.TextStack:GetSizeY()</syntaxhighlight>
{{CodeLine5|0067}}<syntaxhighlight lang="lua">controlTable.Button:SetSizeY(sizeY);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|NotificationPanel.lua}}
:<code>UI/InGame/WorldView/NotificationPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0363}}<syntaxhighlight lang="lua">local bigY = Controls.BigStack:GetSizeY();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|Ranking.lua}}
:<code>UI/InGame/Popups/Ranking.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0044}}<syntaxhighlight lang="lua">local buttonY = controlTable.MyStack:GetSizeY();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ReplayViewer.lua}}
:<code>UI/InGame/Popups/ReplayViewer.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0327}}<syntaxhighlight lang="lua">local yAbsoluteOffset = (screenY * 0.5) - (Controls.MainPanel:GetSizeY() * 0.5);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0333}}<syntaxhighlight lang="lua">local graphDisplayHeight = Controls.GraphDisplay:GetSizeY();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|StagingRoom.lua}}
:<code>UI/FrontEnd/Multiplayer/StagingRoom.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0793}}<syntaxhighlight lang="lua">Controls.OptionsScrollPanel:SetSizeY( Controls.VerticalTrim:GetSizeY() - 2);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1191}}<syntaxhighlight lang="lua">controlTable.Box:SetSizeY( controlTable.String:GetSizeY() + 15 );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|UnitList.lua}}
:<code>UI/InGame/UnitList.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0204}}<syntaxhighlight lang="lua">local statusY = instance.Status:GetSizeY();</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetSizeY]]