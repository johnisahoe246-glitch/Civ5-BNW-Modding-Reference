{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Player}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''string''' Player:GetCivilizationShortDescriptionKey<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|CityBannerManager.lua}}
:<code>UI/InGame/CityBannerManager.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0466}}<syntaxhighlight lang="lua">local strShortDescKey = player:GetCivilizationShortDescriptionKey();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CityStateDiploPopup.lua}}
:<code>UI/InGame/Popups/CityStateDiploPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0087}}<syntaxhighlight lang="lua">strTitle = Locale.ConvertTextKey("{"..pPlayer:GetCivilizationShortDescriptionKey()..":upper}");</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0266}}<syntaxhighlight lang="lua">Controls.AllyInfo:SetText("[COLOR_POSITIVE_TEXT]" .. Locale.ConvertTextKey(Players[iAlly]:GetCivilizationShortDescriptionKey()) .. "[ENDCOLOR]");</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0435}}<syntaxhighlight lang="lua">local strPlayerKey = Players[iQuestData1]:GetCivilizationShortDescriptionKey();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0636}}<syntaxhighlight lang="lua">local warConfirmString = Locale.ConvertTextKey("TXT_KEY_CONFIRM_WAR_PROTECTED_CITY_STATE", Players[g_iMinorCivID]:GetCivilizationShortDescriptionKey());</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0647}}<syntaxhighlight lang="lua">warConfirmString = warConfirmString .. ", " .. Locale.ConvertTextKey(Players[iPlayerLoop]:GetCivilizationShortDescriptionKey());</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0649}}<syntaxhighlight lang="lua">warConfirmString = warConfirmString .. " " .. Locale.ConvertTextKey(Players[iPlayerLoop]:GetCivilizationShortDescriptionKey());</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CityStateDiploPopup.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/Popups/CityStateDiploPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0257}}<syntaxhighlight lang="lua">strAllyTT = Locale.ConvertTextKey("TXT_KEY_CITY_STATE_ALLY_TT", Players[iAlly]:GetCivilizationShortDescriptionKey(), iInfUntilAllied);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1019}}<syntaxhighlight lang="lua">table.insert(listofProtectingCivs, Players[iPlayerLoop]:GetCivilizationShortDescriptionKey());</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1026}}<syntaxhighlight lang="lua">local cityStateName = Locale.Lookup(pMinor:GetCivilizationShortDescriptionKey());</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CityStateGreetingPopup.lua}}
:<code>UI/InGame/Popups/CityStateGreetingPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0025}}<syntaxhighlight lang="lua">local strNameKey = pPlayer:GetCivilizationShortDescriptionKey();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CityStateStatusHelper.lua (G&K)}}
:<code>DLC/Expansion/UI/CityStateStatusHelper.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0226}}<syntaxhighlight lang="lua">local strShortDescKey = pMinor:GetCivilizationShortDescriptionKey();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0492}}<syntaxhighlight lang="lua">sToolTipText = sToolTipText .. Locale.Lookup( "TXT_KEY_CITY_STATE_QUEST_FIND_PLAYER_FORMAL", Players[iQuestData1]:GetCivilizationShortDescriptionKey() );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0496}}<syntaxhighlight lang="lua">sToolTipText = sToolTipText .. Locale.Lookup( "TXT_KEY_CITY_STATE_QUEST_GIVE_GOLD_FORMAL", Players[iQuestData1]:GetCivilizationShortDescriptionKey() );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0498}}<syntaxhighlight lang="lua">sToolTipText = sToolTipText .. Locale.Lookup( "TXT_KEY_CITY_STATE_QUEST_PLEDGE_TO_PROTECT_FORMAL", Players[iQuestData1]:GetCivilizationShortDescriptionKey() );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0526}}<syntaxhighlight lang="lua">sToolTipText = sToolTipText .. Locale.Lookup( "TXT_KEY_CITY_STATE_QUEST_BULLY_CITY_STATE_FORMAL", Players[iQuestData1]:GetCivilizationShortDescriptionKey() );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0528}}<syntaxhighlight lang="lua">sToolTipText = sToolTipText .. Locale.Lookup( "TXT_KEY_CITY_STATE_QUEST_DENOUNCE_MAJOR_FORMAL", Players[iQuestData1]:GetCivilizationShortDescriptionKey() );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0546}}<syntaxhighlight lang="lua">sToolTipText = sToolTipText .. Locale.Lookup( "TXT_KEY_NOTIFICATION_MINOR_BARBS_QUEST", Players[iMinor]:GetCivilizationShortDescriptionKey() );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ConfirmGiftPopup.lua}}
:<code>UI/InGame/PopupsGeneric/ConfirmGiftPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0021}}<syntaxhighlight lang="lua">strCivName = Locale.ConvertTextKey(pGiftedPlayer:GetCivilizationShortDescriptionKey());</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DeclareWarMovePopup.lua}}
:<code>UI/InGame/PopupsGeneric/DeclareWarMovePopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0049}}<syntaxhighlight lang="lua">popupText = popupText .. ", " .. Locale.ConvertTextKey(Players[iPlayerLoop]:GetCivilizationShortDescriptionKey());</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0051}}<syntaxhighlight lang="lua">popupText = popupText .. " " .. Locale.ConvertTextKey(Players[iPlayerLoop]:GetCivilizationShortDescriptionKey());</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DiploList.lua}}
:<code>UI/InGame/DiploList.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0526}}<syntaxhighlight lang="lua">controlTable.QuestIcon:LocalizeAndSetToolTip( "TXT_KEY_CITY_STATE_QUEST_FIND_PLAYER_FORMAL", Players[iQuestData1]:GetCivilizationShortDescriptionKey() );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DiploRelationships.lua}}
:<code>UI/InGame/Popups/DiploRelationships.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0537}}<syntaxhighlight lang="lua">pStack.AllyInfo:SetText("[COLOR_POSITIVE_TEXT]" .. Locale.ConvertTextKey(Players[iAlly]:GetCivilizationShortDescriptionKey()) .. "[ENDCOLOR]");</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DiscussionDialog.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/LeaderHead/DiscussionDialog.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0308}}<syntaxhighlight lang="lua">strButton1Tooltip = Locale.ConvertTextKey("TXT_KEY_DIPLO_DISCUSS_PROTECTED_MINOR_FORGIVE_TT", pAIPlayer:GetCivilizationShortDescriptionKey(), pMinor:GetCivilizationShortDescriptionKey(), iInfLoss);</syntaxhighlight>
{{CodeLine5|0309}}<syntaxhighlight lang="lua">strButton2Tooltip = Locale.ConvertTextKey("TXT_KEY_DIPLO_DISCUSS_PROTECTED_MINOR_DISPUTE_TT", pAIPlayer:GetCivilizationShortDescriptionKey(), pMinor:GetCivilizationShortDescriptionKey());</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|InfoTooltipInclude.lua}}
:<code>UI/InGame/InfoTooltipInclude.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0334}}<syntaxhighlight lang="lua">local strShortDescKey = pPlayer:GetCivilizationShortDescriptionKey();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|MinorCivGoldPopup.lua}}
:<code>UI/InGame/PopupsGeneric/MinorCivGoldPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0063}}<syntaxhighlight lang="lua">popupText = Locale.ConvertTextKey("TXT_KEY_POPUP_MINOR_GOLD_GIFT", pPlayer:GetCivilizationShortDescriptionKey());</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0066}}<syntaxhighlight lang="lua">popupText = Locale.ConvertTextKey("TXT_KEY_POPUP_MINOR_GOLD_GIFT_CANT", iLowestGold, pPlayer:GetCivilizationShortDescriptionKey());</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|PlotMouseoverInclude.lua}}
:<code>UI/InGame/PlotMouseoverInclude.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0025}}<syntaxhighlight lang="lua">resultStr = resultStr .. "[COLOR_POSITIVE_TEXT]" .. Locale.ConvertTextKey("TXT_KEY_CITY_STATE_BARB_QUEST_LONG",  pOtherPlayer:GetCivilizationShortDescriptionKey()) .. "[ENDCOLOR]";</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0356}}<syntaxhighlight lang="lua">strOwner = Locale.ConvertTextKey("TXT_KEY_PLOTROLL_OWNED_CIV", pPlayer:GetCivilizationShortDescriptionKey());</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|SocialPolicyPopup.lua}}
:<code>UI/InGame/Popups/SocialPolicyPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0260}}<syntaxhighlight lang="lua">local strText = Locale.ConvertTextKey(strTextKey, player:GetNameKey(), player:GetCivilizationShortDescriptionKey());</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TurnsRemaining.lua - DLC_04 DLC}}
:<code>DLC/DLC_04/Scenarios/1066Scenario/TurnsRemaining.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0046}}<syntaxhighlight lang="lua">local londonText = Locale.ConvertTextKey("TXT_KEY_1066_SCENARIO_LONDON_STATUS", Players[iLondonPlayer]:GetCivilizationShortDescriptionKey());</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0160}}<syntaxhighlight lang="lua">local strPlayerKey = Players[iCSPlayer]:GetCivilizationShortDescriptionKey();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0214}}<syntaxhighlight lang="lua">local playerName = Locale.ConvertTextKey(Players[iPlayerForName]:GetCivilizationShortDescriptionKey());</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TurnsRemaining.lua (G&K)}}
:<code>DLC/Expansion/Scenarios/SteampunkScenario/TurnsRemaining.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0363}}<syntaxhighlight lang="lua">local sMessage = Locale.ConvertTextKey("TXT_KEY_STEAMPUNK_SCENARIO_VICTORY_CATEGORY_NOTIF_TT", pNewOwner:GetCivilizationShortDescriptionKey(), sTitle);</syntaxhighlight>
{{CodeLine5|0364}}<syntaxhighlight lang="lua">local sSummary = Locale.ConvertTextKey("TXT_KEY_STEAMPUNK_SCENARIO_VICTORY_CATEGORY_NOTIF_SUMMARY", pNewOwner:GetCivilizationShortDescriptionKey(), sTitle);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|VictoryProgress.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/Popups/VictoryProgress.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0703}}<syntaxhighlight lang="lua">local strLeaderShortDesc = pLeader:GetCivilizationShortDescriptionKey();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0717}}<syntaxhighlight lang="lua">local strLeaderLoopShortDesc = Locale.ConvertTextKey(pLeaderLoop:GetCivilizationShortDescriptionKey());</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0789}}<syntaxhighlight lang="lua">local strLastVoteLeader = pLastVoteLeader:GetCivilizationShortDescriptionKey();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|VictoryProgress.lua (G&K)}}
:<code>DLC/Expansion/Scenarios/SteampunkScenario/VictoryProgress.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0713}}<syntaxhighlight lang="lua">local strLeaderLoopShortDesc = pLeaderLoop:GetCivilizationShortDescriptionKey();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|VictoryStatus.lua (G&K)}}
:<code>DLC/Expansion/Scenarios/SteampunkScenario/VictoryStatus.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0086}}<syntaxhighlight lang="lua">local sCivAboutToWinKey = Players[giPlayerAboutToWin]:GetCivilizationShortDescriptionKey();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0117}}<syntaxhighlight lang="lua">local sCivDesc = Locale.Lookup(Players[iPlayer]:GetCivilizationShortDescriptionKey());</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|VoteResultsPopup.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/Popups/VoteResultsPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0131}}<syntaxhighlight lang="lua">strVoteCastTT = Locale.ConvertTextKey("TXT_KEY_POP_UN_ELEC_VOTE_TT_CITYSTATE_ALT", pPlayer:GetCivilizationShortDescriptionKey(), pVoteCastPlayer:GetCivilizationShortDescriptionKey());</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0133}}<syntaxhighlight lang="lua">strVoteCastTT = Locale.ConvertTextKey("TXT_KEY_POP_UN_ELEC_VOTE_TT_CIV_ALT", pPlayer:GetCivilizationShortDescriptionKey(), pVoteCastPlayer:GetCivilizationShortDescriptionKey());</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetCivilizationShortDescriptionKey]]
[[Category:Civ5 Players API|GetCivilizationShortDescriptionKey]]