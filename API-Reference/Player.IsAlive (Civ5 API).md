{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Player}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''int''' Player:IsAlive<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
''Too many occurences. Only 50 out of 160 are listed.''

{{PseudoH4|CityBannerManager.lua}}
:<code>UI/InGame/CityBannerManager.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1245}}<syntaxhighlight lang="lua">if( player:IsAlive() )</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CityStateDiploPopup.lua}}
:<code>UI/InGame/Popups/CityStateDiploPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0381}}<syntaxhighlight lang="lua">if (pOtherPlayer:IsAlive()) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CivsAlive.lua - DLC_01 DLC}}
:<code>DLC/DLC_01/Scenarios/Mongol Scenario/CivsAlive.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0012}}<syntaxhighlight lang="lua">if (Players[iPlayerLoop]:IsAlive()) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|Demographics.lua}}
:<code>UI/InGame/Popups/Demographics.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0047}}<syntaxhighlight lang="lua">if(pPlayer:IsAlive() and not pPlayer:IsMinorCiv()) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DiploGlobalRelationships.lua}}
:<code>UI/InGame/Popups/DiploGlobalRelationships.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0038}}<syntaxhighlight lang="lua">if (iOtherPlayer ~= g_iUs and pOtherPlayer:IsAlive()) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0150}}<syntaxhighlight lang="lua">if (pThirdPlayer ~= nil and pThirdPlayer:IsAlive()) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DiploList.lua}}
:<code>UI/InGame/DiploList.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0251}}<syntaxhighlight lang="lua">if (iPlayerLoop ~= g_iPlayer and pOtherPlayer:IsAlive()) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0423}}<syntaxhighlight lang="lua">pOtherPlayer:IsAlive()    and</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DiploRelationships.lua}}
:<code>UI/InGame/Popups/DiploRelationships.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0054}}<syntaxhighlight lang="lua">if (pPlayer:GetTeam() ~= iOtherTeam and pOtherPlayer:IsAlive()) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0136}}<syntaxhighlight lang="lua">if (iPlayerLoop ~= iPlayer and pOtherPlayer:IsAlive()) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DiploVotePopup.lua}}
:<code>UI/InGame/Popups/DiploVotePopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0056}}<syntaxhighlight lang="lua">if (pOtherPlayer ~= nil and pOtherPlayer:IsAlive()) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DiscussionDialog.lua}}
:<code>UI/InGame/LeaderHead/DiscussionDialog.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0425}}<syntaxhighlight lang="lua">if (pPlayer:GetTeam() ~= iThirdPartyTeam and pThirdPartyPlayer:IsAlive()) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0855}}<syntaxhighlight lang="lua">if (not pThirdPartyPlayer:IsAlive()) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|EndGameMenu.lua}}
:<code>UI/InGame/Popups/EndGameMenu.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0018}}<syntaxhighlight lang="lua">if (not pPlayer:IsAlive()) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0027}}<syntaxhighlight lang="lua">if (iActivePlayer ~= iNextPlayer and pPlayer:IsAlive() and pPlayer:IsHuman()) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0180}}<syntaxhighlight lang="lua">if (not Game:IsNetworkMultiPlayer() and player:IsAlive() and PreGame.GetGameOption("GAMEOPTION_NO_EXTENDED_PLAY") ~= 1) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0291}}<syntaxhighlight lang="lua">if (Game.IsHotSeat() and Game.CountHumanPlayersAlive() > 0 and not pPlayer:IsAlive()) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|GameplayUtils.lua (G&K)}}
:<code>DLC/Expansion/Scenarios/SteampunkScenario/GameplayUtils.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0196}}<syntaxhighlight lang="lua">if (Players[iPlayer] ~= nil and Players[iPlayer]:IsAlive()) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|MPList.lua}}
:<code>UI/InGame/WorldView/MPList.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0038}}<syntaxhighlight lang="lua">if( pPlayer:IsAlive() ) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0086}}<syntaxhighlight lang="lua">if (pPlayer:IsAlive() and pPlayer:IsHuman()) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0179}}<syntaxhighlight lang="lua">if( pPlayer:HasReceivedNetTurnComplete() or not pPlayer:IsAlive() ) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ReligionOverview.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/Popups/ReligionOverview.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0490}}<syntaxhighlight lang="lua">if (pPlayer:IsAlive()) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TradeLogic.lua}}
:<code>UI/InGame/WorldView/TradeLogic.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0472}}<syntaxhighlight lang="lua">pLoopPlayer:IsAlive()) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|2554}}<syntaxhighlight lang="lua">if( pLoopPlayer:IsAlive() ) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TradeLogic.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/WorldView/TradeLogic.lua</code>
:{{CodeBegin5}}
{{CodeLine5|2005}}<syntaxhighlight lang="lua">if (player:GetTeam() == iOtherTeam and player:IsAlive()) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|2806}}<syntaxhighlight lang="lua">if(pLoopPlayer:IsAlive() and otherPlayerButton ~= nil) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TurnsRemaining.lua - DLC_02 DLC}}
:<code>DLC/DLC_02/Scenarios/NewWorldScenario/TurnsRemaining.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0016}}<syntaxhighlight lang="lua">if (player:IsAlive()) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0335}}<syntaxhighlight lang="lua">if (pLoopPlayer:IsAlive() and pLoopPlayer:GetStartingPlot():GetX() > 50) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0408}}<syntaxhighlight lang="lua">if (pPlayer:IsAlive() and not pPlayer:IsMinorCiv() and (iPlayer == iNWOwner or iNWOwner == -1 or iNWOwner > 7)) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TurnsRemaining.lua (G&K)}}
:<code>DLC/Expansion/Scenarios/SteampunkScenario/TurnsRemaining.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0170}}<syntaxhighlight lang="lua">if (pPlayer ~= nil and pPlayer:IsAlive()) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0198}}<syntaxhighlight lang="lua">if (pPlayer and pPlayer:IsAlive()) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0682}}<syntaxhighlight lang="lua">if (Players[iPlayer]:IsAlive() and gbLogSaveData) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TurnsRemaining.lua (G&K)}}
:<code>DLC/Expansion/Scenarios/FallOfRomeScenario/TurnsRemaining.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0288}}<syntaxhighlight lang="lua">if (pPlayer:IsAlive() and IsEmpire(iPlayerLoop)) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TurnsRemaining.lua (G&K)}}
:<code>DLC/Expansion/Scenarios/MedievalScenario/TurnsRemaining.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1123}}<syntaxhighlight lang="lua">if (pPlayer:IsAlive() and pPlayer:GetNumCities() == 0) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TutorialChecks.lua}}
:<code>Tutorial/TutorialChecks.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1064}}<syntaxhighlight lang="lua">if (player:GetTeam() ~= iOtherTeam and pOtherPlayer:IsAlive()) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1125}}<syntaxhighlight lang="lua">if (pOtherPlayer:IsMinorCiv() and pOtherPlayer:IsAlive() and not pTeam:IsAtWar(iOtherTeam)) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|2809}}<syntaxhighlight lang="lua">if (team ~= iOtherTeam and pOtherPlayer:IsAlive()) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|3002}}<syntaxhighlight lang="lua">if (pPlayer:GetTeam() ~= iOtherTeam and pOtherPlayer:IsAlive() and pOtherPlayer:IsFriends()) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|UnitFlagManager.lua}}
:<code>UI/InGame/UnitFlagManager.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0908}}<syntaxhighlight lang="lua">not Players[ playerID ]:IsAlive() )</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0934}}<syntaxhighlight lang="lua">not Players[ playerID ]:IsAlive() or</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|VictoryProgress.lua}}
:<code>UI/InGame/Popups/VictoryProgress.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0267}}<syntaxhighlight lang="lua">pPlayer:IsHasLostCapital() or not pPlayer:IsAlive(),</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0374}}<syntaxhighlight lang="lua">not pPlayer:IsAlive() or Teams[pPlayer:GetTeam()]:GetLiberatedByTeam() ~= -1,</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0447}}<syntaxhighlight lang="lua">if(not v:IsMinorCiv() and v:IsAlive() and (leadAI == nil or v:GetNumPolicyBranchesFinished() > maxPolicies) and i ~= Game.GetActivePlayer()) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0580}}<syntaxhighlight lang="lua">SetCivIcon(pPlayer, 45, controlTable.Icon, nil, controlTable.IconOut, not pPlayer:IsAlive(),</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0685}}<syntaxhighlight lang="lua">not pPlayer:IsAlive() or Teams[pTeam]:GetLiberatedByTeam() ~= -1,</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0711}}<syntaxhighlight lang="lua">if(curPlayer:IsAlive()) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0797}}<syntaxhighlight lang="lua">SetCivIcon(pPlayer, 45, controlTable.Icon, nil, controlTable.IconOut,  not pPlayer:IsAlive(),</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|VictoryProgress.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/Popups/VictoryProgress.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0690}}<syntaxhighlight lang="lua">not pPlayer:IsAlive() or Teams[iTeam]:GetLiberatedByTeam() ~= -1,</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|VictoryStatus.lua (G&K)}}
:<code>DLC/Expansion/Scenarios/SteampunkScenario/VictoryStatus.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0111}}<syntaxhighlight lang="lua">if (Players[iPlayer]:IsAlive()) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|WhosWinningPopup.lua}}
:<code>UI/InGame/Popups/WhosWinningPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0153}}<syntaxhighlight lang="lua">if (pLoopPlayer:IsAlive()) then</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|IsAlive]]
[[Category:Civ5 Players API|IsAlive]]