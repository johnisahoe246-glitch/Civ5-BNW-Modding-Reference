{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Player}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''string''' Player:GetNameKey<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|CityStateDiploPopup.lua}}
:<code>UI/InGame/Popups/CityStateDiploPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0387}}<syntaxhighlight lang="lua">strWarString = strWarString .. Locale.ConvertTextKey(pOtherPlayer:GetNameKey());</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0432}}<syntaxhighlight lang="lua">local strTargetPlayerKey = Players[iQuestData1]:GetNameKey();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CityStateStatusHelper.lua (G&K)}}
:<code>DLC/Expansion/UI/CityStateStatusHelper.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0490}}<syntaxhighlight lang="lua">sToolTipText = sToolTipText .. Locale.Lookup( "TXT_KEY_CITY_STATE_QUEST_KILL_CITY_STATE_FORMAL", Players[iQuestData1]:GetNameKey() );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DiploList.lua}}
:<code>UI/InGame/DiploList.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0518}}<syntaxhighlight lang="lua">controlTable.QuestIcon:LocalizeAndSetToolTip( "TXT_KEY_CITY_STATE_QUEST_KILL_CITY_STATE_FORMAL", Players[iQuestData1]:GetNameKey() );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DiploRelationships.lua}}
:<code>UI/InGame/Popups/DiploRelationships.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0205}}<syntaxhighlight lang="lua">controlTable.LeaderName:LocalizeAndSetText( pOtherPlayer:GetNameKey() );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|LiberateMinorPopup.lua}}
:<code>UI/InGame/PopupsGeneric/LiberateMinorPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0013}}<syntaxhighlight lang="lua">popupText = Locale.ConvertTextKey("TXT_KEY_POPUP_CITY_CAPTURE_LIBERATE_MINOR", cityNameKey, pMinor:GetNameKey());</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|PuppetCityPopup.lua}}
:<code>UI/InGame/PopupsGeneric/PuppetCityPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0050}}<syntaxhighlight lang="lua">local strToolTip = Locale.ConvertTextKey("TXT_KEY_POPUP_CITY_CAPTURE_INFO_LIBERATE", Players[iLiberatedPlayer]:GetNameKey());</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|SocialPolicyPopup.lua}}
:<code>UI/InGame/Popups/SocialPolicyPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0260}}<syntaxhighlight lang="lua">local strText = Locale.ConvertTextKey(strTextKey, player:GetNameKey(), player:GetCivilizationShortDescriptionKey());</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TradeLogic.lua}}
:<code>UI/InGame/WorldView/TradeLogic.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0929}}<syntaxhighlight lang="lua">Controls.UsText:SetText( Locale.ConvertTextKey( "TXT_KEY_DIPLO_ITEMS_LABEL", Locale.ConvertTextKey( g_pUs:GetNameKey() ) ) );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0954}}<syntaxhighlight lang="lua">Controls.LeaderNameItems:SetText(Locale.ConvertTextKey("TXT_KEY_DIPLO_ITEMS_LABEL",Locale.ConvertTextKey(g_pThem:GetNameKey())));</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|VictoryProgress.lua}}
:<code>UI/InGame/Popups/VictoryProgress.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0871}}<syntaxhighlight lang="lua">strPlayer = pPlayer:GetNameKey();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|VictoryProgress.lua (G&K)}}
:<code>DLC/Expansion/Scenarios/FallOfRomeScenario/VictoryProgress.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0873}}<syntaxhighlight lang="lua">strPlayer = Locale.ConvertTextKey(pPlayer:GetNameKey());</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|VoteResultsPopup.lua}}
:<code>UI/InGame/Popups/VoteResultsPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0074}}<syntaxhighlight lang="lua">strName = strName .. " " .. Locale.ConvertTextKey(pPlayer:GetNameKey());</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0136}}<syntaxhighlight lang="lua">strVote = Locale.ConvertTextKey(pVoteCastPlayer:GetNameKey());</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetNameKey]]