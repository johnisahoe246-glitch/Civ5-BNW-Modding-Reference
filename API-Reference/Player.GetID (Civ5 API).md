{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Player}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>{{Type5|PlayerID}} Player:GetID<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|ChoosePantheonPopup.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/Popups/ChoosePantheonPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0082}}<syntaxhighlight lang="lua">CivIconHookup( pPlayer:GetID(), 64, Controls.CivIcon, Controls.CivIconBG, Controls.CivIconShadow, false, true );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ChooseReligionPopup.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/Popups/ChooseReligionPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0279}}<syntaxhighlight lang="lua">if (pActivePlayer:GetID() == pPlayer:GetID()) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CityBannerManager.lua}}
:<code>UI/InGame/CityBannerManager.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0992}}<syntaxhighlight lang="lua">if (player:GetID() ~= Game.GetActivePlayer()) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1252}}<syntaxhighlight lang="lua">OnCityCreated( ToHexFromGrid( Vector2( city:GetX(), city:GetY() ) ), player:GetID(), city:GetID() );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|Demographics.lua}}
:<code>UI/InGame/Popups/Demographics.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0332}}<syntaxhighlight lang="lua">if (pPlayer:GetID() == Game.GetActivePlayer()) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DiscussionDialog.lua}}
:<code>UI/InGame/LeaderHead/DiscussionDialog.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0908}}<syntaxhighlight lang="lua">local iCoopState = Players[g_iAIPlayer]:GetCoopWarAcceptedState(pActivePlayer:GetID(), iThirdPartyPlayer);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|GameplayUtilities.lua}}
:<code>Gameplay/Lua/GameplayUtilities.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0014}}<syntaxhighlight lang="lua">local playerID = player:GetID();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|MPList.lua}}
:<code>UI/InGame/WorldView/MPList.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0106}}<syntaxhighlight lang="lua">local bIsLocalPlayer = pPlayer:GetID() == Game.GetActivePlayer();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0144}}<syntaxhighlight lang="lua">CivIconHookup( pPlayer:GetID(), 32, controlTable.Icon, controlTable.CivIconBG, controlTable.CivIconShadow, false, true );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0147}}<syntaxhighlight lang="lua">UpdatePingTimeLabel( controlTable.Ping, pPlayer:GetID() );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0219}}<syntaxhighlight lang="lua">g_PlayerEntries[ pPlayer:GetID() ] = controlTable;</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TutorialChecks.lua}}
:<code>Tutorial/TutorialChecks.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1127}}<syntaxhighlight lang="lua">local iQuest = pOtherPlayer:GetActiveQuestForPlayer(player:GetID());</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1438}}<syntaxhighlight lang="lua">if (not pTargetPlot:IsWater() and pTargetPlot:IsVisibleEnemyUnit(player:GetID())) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|2465}}<syntaxhighlight lang="lua">if (Players[iPlotOwner]:GetMinorCivFriendshipLevelWithMajor(pPlayer:GetID()) < 1) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TutorialChecks.lua (G&K)}}
:<code>DLC/Expansion/Tutorial/TutorialChecks.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1127}}<syntaxhighlight lang="lua">if (pOtherPlayer:GetMinorCivNumActiveQuestsForPlayer(player:GetID()) >= 0) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|UnitFlagManager.lua}}
:<code>UI/InGame/UnitFlagManager.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1412}}<syntaxhighlight lang="lua">OnUnitCreated( player:GetID(), unit:GetID(), 0, 0, 0, 0, 0, 0, 0, WhiteFog, 0, 0, true );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|VictoryProgress.lua}}
:<code>UI/InGame/Popups/VictoryProgress.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0264}}<syntaxhighlight lang="lua">local iPlayer = pPlayer:GetID();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0384}}<syntaxhighlight lang="lua">elseif(pPlayer:GetID() == Game.GetActivePlayer()) then</syntaxhighlight>
{{CodeLine5|0385}}<syntaxhighlight lang="lua">if(PreGame.GetCivilizationShortDescription(pPlayer:GetID()) ~= "") then</syntaxhighlight>
{{CodeLine5|0386}}<syntaxhighlight lang="lua">strPlayer = PreGame.GetCivilizationShortDescription(pPlayer:GetID());</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0673}}<syntaxhighlight lang="lua">local iPlayerLoop = pPlayer:GetID();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0865}}<syntaxhighlight lang="lua">strCiv = PreGame.GetCivilizationShortDescription(pPlayer:GetID());</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|VoteResultsPopup.lua}}
:<code>UI/InGame/Popups/VoteResultsPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0043}}<syntaxhighlight lang="lua">if ((pPlayer:GetID() == activePlayer:GetID()) or (activePlayer:GetTeam() == pTeam:GetID())) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0047}}<syntaxhighlight lang="lua">CivIconHookup( pPlayer:GetID(), 32, controlTable.Icon, controlTable.IconBG, controlTable.IconShadow, false, true );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0082}}<syntaxhighlight lang="lua">CivIconHookup( pPlayer:GetID(), 32, controlTable.Icon, controlTable.IconBG, controlTable.IconShadow, false, true);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0121}}<syntaxhighlight lang="lua">elseif (pVoteCastPlayer:GetID() == Game.GetActivePlayer()) then</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetID]]