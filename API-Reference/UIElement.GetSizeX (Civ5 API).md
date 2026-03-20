{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This method is declared by '''ControlBase'''.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''int''' UIElement:GetSizeX<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|CityBannerManager.lua}}
:<code>UI/InGame/CityBannerManager.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0750}}<syntaxhighlight lang="lua">local iWidth = BannerInstance.CityName:GetSizeX();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CityBannerManager.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/CityBannerManager.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0736}}<syntaxhighlight lang="lua">local iWidth = BannerInstance.NameStack:GetSizeX();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CityView.lua}}
:<code>UI/InGame/CityView/CityView.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0721}}<syntaxhighlight lang="lua">local cityNameSize = (math.abs(Controls.NextCityButton:GetOffsetX()) * 2) - (Controls.PrevCityButton:GetSizeX());</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0724}}<syntaxhighlight lang="lua">cityNameSize = cityNameSize - Controls.CityCapitalIcon:GetSizeX();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1300}}<syntaxhighlight lang="lua">Controls.ResourceDemandedBox:SetSizeX(Controls.ResourceDemandedString:GetSizeX() + 10);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DiploCorner.lua}}
:<code>UI/InGame/WorldView/DiploCorner.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0296}}<syntaxhighlight lang="lua">TruncateString( Controls.LengthTest, Controls.ChatPull:GetSizeX(), Locale.ConvertTextKey("TXT_KEY_DIPLO_TO_TEAM"));</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0300}}<syntaxhighlight lang="lua">TruncateString( Controls.LengthTest, Controls.ChatPull:GetSizeX(), Locale.ConvertTextKey("TXT_KEY_DIPLO_TO_PLAYER", Players[ iPlayer ]:GetNickName()));</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0356}}<syntaxhighlight lang="lua">TruncateString( textControl, Controls.ChatPull:GetSizeX()-20, Locale.ConvertTextKey("TXT_KEY_DIPLO_TO_PLAYER", pPlayer:GetNickName()));</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DiploList.lua}}
:<code>UI/InGame/DiploList.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0213}}<syntaxhighlight lang="lua">local textBoxSize = Controls.NameBox:GetSizeX() - Controls.LeaderName:GetOffsetX();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0229}}<syntaxhighlight lang="lua">local textBoxSize = Controls.NameBox:GetSizeX() - Controls.CivName:GetOffsetX() - 120;</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0260}}<syntaxhighlight lang="lua">local textBoxSize = controlTable.NameBox:GetSizeX() - controlTable.LeaderName:GetOffsetX();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0334}}<syntaxhighlight lang="lua">TruncateString( controlTable.DiploState, controlTable.StatusBox:GetSizeX(), statusString );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DiploRelationships.lua}}
:<code>UI/InGame/Popups/DiploRelationships.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0197}}<syntaxhighlight lang="lua">local textBoxSize = controlTable.LeaderNameStack:GetSizeX() - controlTable.DiploState:GetSizeX() -</syntaxhighlight>
{{CodeLine5|0198}}<syntaxhighlight lang="lua">controlTable.Score:GetSizeX() - controlTable.CivIconBG:GetSizeX()- 74;</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DiploVotePopup.lua}}
:<code>UI/InGame/Popups/DiploVotePopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0067}}<syntaxhighlight lang="lua">local textBoxSize = controlTable.Button:GetSizeX() - controlTable.ButtonText:GetOffsetX();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|EnemyUnitPanel.lua}}
:<code>UI/InGame/WorldView/EnemyUnitPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0553}}<syntaxhighlight lang="lua">local sizeX = Controls.DetailsGrid:GetSizeX();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|GameMenu.lua}}
:<code>UI/InGame/Menus/GameMenu.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0320}}<syntaxhighlight lang="lua">local availableTextExtent = Controls.ScrollPanel:GetSizeX();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|LoadMenu.lua}}
:<code>UI/FrontEnd/LoadMenu.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0231}}<syntaxhighlight lang="lua">TruncateString(Controls.SaveFileName, Controls.DetailsBox:GetSizeX(), name);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0558}}<syntaxhighlight lang="lua">TruncateString(controlTable.ButtonText, controlTable.Button:GetSizeX(), entryName);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0576}}<syntaxhighlight lang="lua">TruncateString(controlTable.ButtonText, controlTable.Button:GetSizeX(), displayName);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|Lobby.lua}}
:<code>UI/FrontEnd/Multiplayer/Lobby.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0228}}<syntaxhighlight lang="lua">TruncateString(controlTable.ServerNameLabel, controlTable.ServerNameBox:GetSizeX(), serverEntry.serverName);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|MPList.lua}}
:<code>UI/InGame/WorldView/MPList.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0126}}<syntaxhighlight lang="lua">local textSize = controlTable.Root:GetSizeX() - controlTable.Name:GetOffsetX() - controlTable.CivIconBG:GetSizeX() + (controlTable.IconBox:GetOffsetX() /2);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0245}}<syntaxhighlight lang="lua">teamEntry.Root:SetSizeX( teamEntry.TeamStack:GetSizeX() );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ReplayViewer.lua}}
:<code>UI/InGame/Popups/ReplayViewer.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0324}}<syntaxhighlight lang="lua">local xAbsoluteOffset = (screenX * 0.5) - (Controls.MainPanel:GetSizeX() * 0.5);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0332}}<syntaxhighlight lang="lua">local graphDisplayWidth = Controls.GraphDisplay:GetSizeX();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|SaveMenu.lua}}
:<code>UI/InGame/Menus/SaveMenu.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0569}}<syntaxhighlight lang="lua">TruncateString(instance.ButtonText, instance.Button:GetSizeX(), displayName);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|StagingRoom.lua}}
:<code>UI/FrontEnd/Multiplayer/StagingRoom.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0385}}<syntaxhighlight lang="lua">TruncateString(slotInstance.PlayerNameLabel, slotInstance.PlayerNameBox:GetSizeX() -</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0559}}<syntaxhighlight lang="lua">TruncateString(Controls.PlayerNameLabel, Controls.PlayerNameBox:GetSizeX() -</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|SupportFunctions.lua}}
:<code>UI/SupportFunctions.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0016}}<syntaxhighlight lang="lua">local fullStrExtent = control:GetSizeX();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0023}}<syntaxhighlight lang="lua">local trailingExtent = control:GetSizeX();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0037}}<syntaxhighlight lang="lua">local ellipsisExtent = control:GetSizeX();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0043}}<syntaxhighlight lang="lua">truncatedSize = control:GetSizeX();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TradeLogic.lua}}
:<code>UI/InGame/WorldView/TradeLogic.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0985}}<syntaxhighlight lang="lua">TruncateString(Controls.ThemName, Controls.ThemTablePanel:GetSizeX() - Controls.ThemTablePanel:GetOffsetX(),</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|2784}}<syntaxhighlight lang="lua">TruncateString(controlTable.Name, controlTable.ButtonSize:GetSizeX() - controlTable.Name:GetOffsetX(), szName);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|VictoryProgress.lua}}
:<code>UI/InGame/Popups/VictoryProgress.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0577}}<syntaxhighlight lang="lua">SetCivName(pPlayer, i, controlTable.Name, true, controlTable.Civ:GetSizeX() - controlTable.CivIconBG:GetSizeX());</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|VoteResultsPopup.lua}}
:<code>UI/InGame/Popups/VoteResultsPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0155}}<syntaxhighlight lang="lua">unSize = controlTable.UNIcon:GetSizeX();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0168}}<syntaxhighlight lang="lua">TruncateString(controlTable.PlayerNameText, controlTable.PlayerNameBox:GetSizeX(), strName);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0176}}<syntaxhighlight lang="lua">TruncateString(controlTable.VoteCastText, controlTable.VoteCastBox:GetSizeX() - unSize, strVote);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|VoteResultsPopup.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/Popups/VoteResultsPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0199}}<syntaxhighlight lang="lua">TruncateString(controlTable.VoteCastText, controlTable.VoteCastBox:GetSizeX(), strVote);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetSizeX]]