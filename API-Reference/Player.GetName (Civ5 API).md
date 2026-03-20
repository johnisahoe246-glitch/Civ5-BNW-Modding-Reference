{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Player}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''string''' Player:GetName<b>(</b>'''string''' form<b>)</b></code>


'''Returned Value'''
:No description available.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|form:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|ActionInfoPanel.lua}}
:<code>UI/InGame/WorldView/ActionInfoPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0243}}<syntaxhighlight lang="lua">local playerName = otherPlayer:GetName();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ChooseReligionPopup.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/Popups/ChooseReligionPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0276}}<syntaxhighlight lang="lua">takenReligions[eReligion] = pPlayer:GetName();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DiploCurrentDeals.lua}}
:<code>UI/InGame/Popups/DiploCurrentDeals.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0102}}<syntaxhighlight lang="lua">controlTable.PlayerLabel:SetText( pOtherPlayer:GetName() );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DiploGlobalRelationships.lua}}
:<code>UI/InGame/Popups/DiploGlobalRelationships.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0063}}<syntaxhighlight lang="lua">otherName = pOtherPlayer:GetName();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DiploList.lua}}
:<code>UI/InGame/DiploList.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0265}}<syntaxhighlight lang="lua">controlTable.LeaderName:SetText( pOtherPlayer:GetName() );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DiscussionDialog.lua}}
:<code>UI/InGame/LeaderHead/DiscussionDialog.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0201}}<syntaxhighlight lang="lua">strLeaderName = pAIPlayer:GetName();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0596}}<syntaxhighlight lang="lua">AddLeaderButton( iPlayerLoop, pThirdPartyPlayer:GetName() );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0816}}<syntaxhighlight lang="lua">AddLeaderButton( iPlayerLoop, Players[iPlayerLoop]:GetName() );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|EspionageOverview.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/Popups/EspionageOverview.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0881}}<syntaxhighlight lang="lua">strLeaderName = pPlayer:GetName();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|MPList.lua}}
:<code>UI/InGame/WorldView/MPList.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0153}}<syntaxhighlight lang="lua">TruncateString( controlTable.Name, textSize, pPlayer:GetName() );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ReplayViewer.lua}}
:<code>UI/InGame/Popups/ReplayViewer.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1287}}<syntaxhighlight lang="lua">LeaderName = player:GetName(),</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TradeLogic.lua}}
:<code>UI/InGame/WorldView/TradeLogic.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0934}}<syntaxhighlight lang="lua">Controls.ThemText:SetText( Locale.ConvertTextKey( "TXT_KEY_DIPLO_ITEMS_LABEL", Locale.ConvertTextKey( g_pThem:GetName() ) ) );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0944}}<syntaxhighlight lang="lua">local strString = Locale.ConvertTextKey("TXT_KEY_DIPLO_LEADER_SAYS", g_pThem:GetName());</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|2776}}<syntaxhighlight lang="lua">szName = pLoopPlayer:GetName();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TurnsRemaining.lua - DLC_02 DLC}}
:<code>DLC/DLC_02/Scenarios/NewWorldScenario/TurnsRemaining.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0194}}<syntaxhighlight lang="lua">popupInfo.Text = Locale.ConvertTextKey("TXT_KEY_NEWWORLD_SCENARIO_OTHER_CIRCUMNAVIGATION", player:GetName(), iRemaining);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TurnsRemaining.lua (G&K)}}
:<code>DLC/Expansion/Scenarios/MedievalScenario/TurnsRemaining.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0636}}<syntaxhighlight lang="lua">popupInfo.Text = Locale.ConvertTextKey("TXT_KEY_MEDIEVAL_SCENARIO_OTHER_CARAVEL", player:GetName(), iVPReceived, (5 - iNumCaravels));</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0773}}<syntaxhighlight lang="lua">popupInfo.Text = Locale.ConvertTextKey("TXT_KEY_MEDIEVAL_SCENARIO_OTHER_ADOPTED_PROTESTANTISM", pPlayer:GetName());</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|VoteResultsPopup.lua (G&K)}}
:<code>DLC/Expansion/Scenarios/MedievalScenario/VoteResultsPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0296}}<syntaxhighlight lang="lua">strVotesToWinString = Locale.ConvertTextKey("TXT_KEY_MEDIEVAL_SCENARIO_HRE_WINNER", Players[iBestVotePlayer]:GetName());</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetName]]