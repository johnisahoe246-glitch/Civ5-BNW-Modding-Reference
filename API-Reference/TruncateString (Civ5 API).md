{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a global function. Use: <code>include("SupportFunctions.lua")</code>
}}


=Usage=
<code>'''void''' TruncateString<b>(</b>{{Type5|Label}} control, '''int''' resultSize, '''string''' longStr, '''string''' trailingText = nil<b>)</b></code>


'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|control:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|resultSize:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|longStr:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|trailingText:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|CityView.lua}}
:<code>UI/InGame/CityView/CityView.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0726}}<syntaxhighlight lang="lua">TruncateString(Controls.CityNameTitleBarLabel, cityNameSize, convertedKey);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DiploCorner.lua}}
:<code>UI/InGame/WorldView/DiploCorner.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0144}}<syntaxhighlight lang="lua">TruncateString( controlTable.String, 200, Players[fromPlayer]:GetNickName() );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0157}}<syntaxhighlight lang="lua">TruncateString( controlTable.String, 200, Players[toPlayer]:GetNickName() );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0296}}<syntaxhighlight lang="lua">TruncateString( Controls.LengthTest, Controls.ChatPull:GetSizeX(), Locale.ConvertTextKey("TXT_KEY_DIPLO_TO_TEAM"));</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0300}}<syntaxhighlight lang="lua">TruncateString( Controls.LengthTest, Controls.ChatPull:GetSizeX(), Locale.ConvertTextKey("TXT_KEY_DIPLO_TO_PLAYER", Players[ iPlayer ]:GetNickName()));</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0356}}<syntaxhighlight lang="lua">TruncateString( textControl, Controls.ChatPull:GetSizeX()-20, Locale.ConvertTextKey("TXT_KEY_DIPLO_TO_PLAYER", pPlayer:GetNickName()));</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DiploList.lua}}
:<code>UI/InGame/DiploList.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0216}}<syntaxhighlight lang="lua">TruncateString(Controls.LeaderName, textBoxSize, g_pPlayer:GetNickName());</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0218}}<syntaxhighlight lang="lua">TruncateString(Controls.LeaderName, textBoxSize, Locale.ConvertTextKey( PreGame.GetLeaderName( g_iPlayer ) ), "  (" .. Locale.ConvertTextKey( "TXT_KEY_YOU" ) .. ")");</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0220}}<syntaxhighlight lang="lua">TruncateString(Controls.LeaderName, textBoxSize, Locale.ConvertTextKey( leaderDescription ), "  (" .. Locale.ConvertTextKey( "TXT_KEY_YOU" ) .. ")");</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0231}}<syntaxhighlight lang="lua">TruncateString(Controls.CivName, textBoxSize, Locale.ConvertTextKey(PreGame.GetCivilizationShortDescription(g_iPlayer)));</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0233}}<syntaxhighlight lang="lua">TruncateString(Controls.CivName, textBoxSize, Locale.ConvertTextKey(myCivInfo.ShortDescription));</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0263}}<syntaxhighlight lang="lua">TruncateString(controlTable.LeaderName, textBoxSize, pOtherPlayer:GetNickName());</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0334}}<syntaxhighlight lang="lua">TruncateString( controlTable.DiploState, controlTable.StatusBox:GetSizeX(), statusString );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DiploVotePopup.lua}}
:<code>UI/InGame/Popups/DiploVotePopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0070}}<syntaxhighlight lang="lua">TruncateString(controlTable.ButtonText, textBoxSize, pOtherPlayer:GetNickName());</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0076}}<syntaxhighlight lang="lua">TruncateString(controlTable.ButtonText, textBoxSize, Locale.ConvertTextKey( PreGame.GetLeaderName( Game.GetActivePlayer() ) ), "  (" .. Locale.ConvertTextKey( "TXT_KEY_YOU" ) .. ")");</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0078}}<syntaxhighlight lang="lua">TruncateString(controlTable.ButtonText, textBoxSize, Locale.ConvertTextKey( leaderDescription ), "  (" .. Locale.ConvertTextKey( "TXT_KEY_YOU" ) .. ")");</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0081}}<syntaxhighlight lang="lua">TruncateString(controlTable.ButtonText, textBoxSize, Locale.ConvertTextKey("TXT_KEY_POP_UN_TEAM_LABEL", pOtherTeam:GetID() + 1) , " (" .. Locale.ConvertTextKey("TXT_KEY_POP_VOTE_RESULTS_YOUR_TEAM") .. ")");</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0087}}<syntaxhighlight lang="lua">TruncateString(controlTable.ButtonText, textBoxSize, Locale.ConvertTextKey( leaderDescription ));</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0089}}<syntaxhighlight lang="lua">TruncateString(controlTable.ButtonText, textBoxSize, Locale.ConvertTextKey("TXT_KEY_POP_UN_TEAM_LABEL", pOtherTeam:GetID() + 1));</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|GameMenu.lua}}
:<code>UI/InGame/Menus/GameMenu.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0325}}<syntaxhighlight lang="lua">TruncateString(Controls.DetailsCiv, availableTextExtent, Locale.ConvertTextKey(myCivInfo.ShortDescription));</syntaxhighlight>
{{CodeLine5|0326}}<syntaxhighlight lang="lua">TruncateString(Controls.DetailsLeader, availableTextExtent, pPlayer:GetNickName());</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0328}}<syntaxhighlight lang="lua">TruncateString(Controls.DetailsCiv, availableTextExtent, PreGame.GetCivilizationShortDescription(0));</syntaxhighlight>
{{CodeLine5|0329}}<syntaxhighlight lang="lua">TruncateString(Controls.DetailsLeader, availableTextExtent, PreGame.GetLeaderName(0));</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0334}}<syntaxhighlight lang="lua">TruncateString(Controls.DetailsLeader, availableTextExtent, Locale.ConvertTextKey(leaderDescription));</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|GPList.lua}}
:<code>UI/InGame/GPList.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0117}}<syntaxhighlight lang="lua">TruncateString( instance.CityName, 74, sortEntry.name );</syntaxhighlight>
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
{{CodeLine5|0140}}<syntaxhighlight lang="lua">TruncateString( controlTable.Name, textSize, pPlayer:GetNickName() );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0153}}<syntaxhighlight lang="lua">TruncateString( controlTable.Name, textSize, pPlayer:GetName() );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ResourceList.lua}}
:<code>UI/InGame/ResourceList.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0116}}<syntaxhighlight lang="lua">TruncateString( instance.ResourceName, 140, resource.IconString .. " " .. sortEntry.name );</syntaxhighlight>
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
{{CodeLine5|0386}}<syntaxhighlight lang="lua">slotInstance.PlayerNameLabel:GetOffsetX(), playerName);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0403}}<syntaxhighlight lang="lua">TruncateString(slotInstance.PlayerNameLabel, slotInstance.PlayerNameBox:GetSizeX() -</syntaxhighlight>
{{CodeLine5|0404}}<syntaxhighlight lang="lua">slotInstance.PlayerNameLabel:GetOffsetX(), Locale.ConvertTextKey("TXT_KEY_AI_NICKNAME"));</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0559}}<syntaxhighlight lang="lua">TruncateString(Controls.PlayerNameLabel, Controls.PlayerNameBox:GetSizeX() -</syntaxhighlight>
{{CodeLine5|0560}}<syntaxhighlight lang="lua">Controls.PlayerNameLabel:GetOffsetX(), playerName);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TradeLogic.lua}}
:<code>UI/InGame/WorldView/TradeLogic.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0985}}<syntaxhighlight lang="lua">TruncateString(Controls.ThemName, Controls.ThemTablePanel:GetSizeX() - Controls.ThemTablePanel:GetOffsetX(),</syntaxhighlight>
{{CodeLine5|0986}}<syntaxhighlight lang="lua">Locale.ConvertTextKey( "TXT_KEY_DIPLO_ITEMS_LABEL", g_pThem:GetNickName() ));</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|2784}}<syntaxhighlight lang="lua">TruncateString(controlTable.Name, controlTable.ButtonSize:GetSizeX() - controlTable.Name:GetOffsetX(), szName);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|UnitList.lua}}
:<code>UI/InGame/UnitList.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0132}}<syntaxhighlight lang="lua">TruncateString( instance.UnitName, 110, sortEntry.name );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|VictoryProgress.lua}}
:<code>UI/InGame/Popups/VictoryProgress.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0394}}<syntaxhighlight lang="lua">TruncateString(Controls.UNInfo, 200, strPlayer);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0467}}<syntaxhighlight lang="lua">TruncateString(Controls.CultureLabel, 200, strCiv);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0879}}<syntaxhighlight lang="lua">TruncateString(controlTable, controlSize, displayText);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|VoteResultsPopup.lua}}
:<code>UI/InGame/Popups/VoteResultsPopup.lua</code>
:{{CodeBegin5}}
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
[[Category:Civ5 Methods and Functions|TruncateString]]