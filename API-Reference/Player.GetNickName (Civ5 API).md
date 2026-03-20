{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Player}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''string''' Player:GetNickName<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|ActionInfoPanel.lua}}
:<code>UI/InGame/WorldView/ActionInfoPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0244}}<syntaxhighlight lang="lua">pleaseWait = pleaseWait .. "[NEWLINE]" .. "(" .. otherPlayer:GetNickName() .. ") " .. playerName;</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DiploCorner.lua}}
:<code>UI/InGame/WorldView/DiploCorner.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0144}}<syntaxhighlight lang="lua">TruncateString( controlTable.String, 200, Players[fromPlayer]:GetNickName() );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0157}}<syntaxhighlight lang="lua">TruncateString( controlTable.String, 200, Players[toPlayer]:GetNickName() );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0300}}<syntaxhighlight lang="lua">TruncateString( Controls.LengthTest, Controls.ChatPull:GetSizeX(), Locale.ConvertTextKey("TXT_KEY_DIPLO_TO_PLAYER", Players[ iPlayer ]:GetNickName()));</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0356}}<syntaxhighlight lang="lua">TruncateString( textControl, Controls.ChatPull:GetSizeX()-20, Locale.ConvertTextKey("TXT_KEY_DIPLO_TO_PLAYER", pPlayer:GetNickName()));</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DiploCurrentDeals.lua}}
:<code>UI/InGame/Popups/DiploCurrentDeals.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0096}}<syntaxhighlight lang="lua">if( pOtherPlayer:GetNickName() ~= "" and pOtherPlayer:IsHuman() ) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0098}}<syntaxhighlight lang="lua">controlTable.PlayerLabel:SetText( pOtherPlayer:GetNickName() );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DiploGlobalRelationships.lua}}
:<code>UI/InGame/Popups/DiploGlobalRelationships.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0061}}<syntaxhighlight lang="lua">otherName = pOtherPlayer:GetNickName();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0161}}<syntaxhighlight lang="lua">thirdName = pThirdPlayer:GetNickName();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DiploList.lua}}
:<code>UI/InGame/DiploList.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0215}}<syntaxhighlight lang="lua">if(g_pPlayer:GetNickName() ~= "" and Game.IsGameMultiPlayer()) then</syntaxhighlight>
{{CodeLine5|0216}}<syntaxhighlight lang="lua">TruncateString(Controls.LeaderName, textBoxSize, g_pPlayer:GetNickName());</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0262}}<syntaxhighlight lang="lua">if(pOtherPlayer:GetNickName() ~= "" and Game.IsGameMultiPlayer()) then</syntaxhighlight>
{{CodeLine5|0263}}<syntaxhighlight lang="lua">TruncateString(controlTable.LeaderName, textBoxSize, pOtherPlayer:GetNickName());</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DiploRelationships.lua}}
:<code>UI/InGame/Popups/DiploRelationships.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0202}}<syntaxhighlight lang="lua">if(pOtherPlayer:GetNickName() ~= "" and pOtherPlayer:IsHuman()) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DiploVotePopup.lua}}
:<code>UI/InGame/Popups/DiploVotePopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0069}}<syntaxhighlight lang="lua">if(pOtherPlayer:GetNickName() ~= "" and Game:IsNetworkMultiPlayer()) then</syntaxhighlight>
{{CodeLine5|0070}}<syntaxhighlight lang="lua">TruncateString(controlTable.ButtonText, textBoxSize, pOtherPlayer:GetNickName());</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DiscussionDialog.lua}}
:<code>UI/InGame/LeaderHead/DiscussionDialog.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0198}}<syntaxhighlight lang="lua">if(pAIPlayer:GetNickName() ~= "" and Game:IsNetworkMultiPlayer()) then</syntaxhighlight>
{{CodeLine5|0199}}<syntaxhighlight lang="lua">strLeaderName = pAIPlayer:GetNickName();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|EspionageOverview.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/Popups/EspionageOverview.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0878}}<syntaxhighlight lang="lua">if(pPlayer:GetNickName() ~= "" and Game:IsNetworkMultiPlayer()) then</syntaxhighlight>
{{CodeLine5|0879}}<syntaxhighlight lang="lua">strLeaderName = pPlayer:GetNickName();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|GameMenu.lua}}
:<code>UI/InGame/Menus/GameMenu.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0204}}<syntaxhighlight lang="lua">if(Game:IsNetworkMultiPlayer() and pPlayer:GetNickName() ~= "") then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0208}}<syntaxhighlight lang="lua">Controls.LeaderFrame:SetToolTipString( pPlayer:GetNickName() );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0326}}<syntaxhighlight lang="lua">TruncateString(Controls.DetailsLeader, availableTextExtent, pPlayer:GetNickName());</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|GameplayUtilities.lua}}
:<code>Gameplay/Lua/GameplayUtilities.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0020}}<syntaxhighlight lang="lua">local nickName = player:GetNickName();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|MPList.lua}}
:<code>UI/InGame/WorldView/MPList.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0140}}<syntaxhighlight lang="lua">TruncateString( controlTable.Name, textSize, pPlayer:GetNickName() );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|PlotMouseoverInclude.lua}}
:<code>UI/InGame/PlotMouseoverInclude.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0271}}<syntaxhighlight lang="lua">if (pPlayer:GetNickName() ~= nil and pPlayer:GetNickName() ~= "") then</syntaxhighlight>
{{CodeLine5|0272}}<syntaxhighlight lang="lua">strUnitText = strUnitText .. Locale.ConvertTextKey("TXT_KEY_MULTIPLAYER_UNIT_TT", pPlayer:GetNickName(), pPlayer:GetCivilizationAdjectiveKey(), unit:GetNameKey());</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0353}}<syntaxhighlight lang="lua">strOwner = Locale.ConvertTextKey("TXT_KEY_PLOTROLL_OWNED_PLAYER", pPlayer:GetNickName());</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TradeLogic.lua}}
:<code>UI/InGame/WorldView/TradeLogic.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0932}}<syntaxhighlight lang="lua">Controls.ThemText:SetText( Locale.ConvertTextKey( "TXT_KEY_DIPLO_ITEMS_LABEL", Locale.ConvertTextKey( g_pThem:GetNickName() ) ) );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0986}}<syntaxhighlight lang="lua">Locale.ConvertTextKey( "TXT_KEY_DIPLO_ITEMS_LABEL", g_pThem:GetNickName() ));</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|2774}}<syntaxhighlight lang="lua">szName = pLoopPlayer:GetNickName();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|UnitFlagManager.lua}}
:<code>UI/InGame/UnitFlagManager.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1582}}<syntaxhighlight lang="lua">toolTipString = Locale.ConvertTextKey("TXT_KEY_MULTIPLAYER_UNIT_TT", pPlayer:GetNickName(), pPlayer:GetCivilizationAdjectiveKey(), pUnit:GetNameKey());</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|VictoryProgress.lua}}
:<code>UI/InGame/Popups/VictoryProgress.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0383}}<syntaxhighlight lang="lua">strPlayer = pPlayer:GetNickName();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0458}}<syntaxhighlight lang="lua">if(leadAI:GetNickName() ~= "" and Game:IsNetworkMultiPlayer()) then</syntaxhighlight>
{{CodeLine5|0459}}<syntaxhighlight lang="lua">strCiv = Locale.Lookup(pPlayer:GetNickName());</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0903}}<syntaxhighlight lang="lua">controlTableTT:SetToolTipString(pPlayer:GetNickName());</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|VictoryProgress.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/Popups/VictoryProgress.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0459}}<syntaxhighlight lang="lua">strCiv = pPlayer:GetNickName();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|VoteResultsPopup.lua}}
:<code>UI/InGame/Popups/VoteResultsPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0072}}<syntaxhighlight lang="lua">strName = strName .. " " .. pPlayer:GetNickName();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0134}}<syntaxhighlight lang="lua">strVote = pVoteCastPlayer:GetNickName();</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetNickName]]