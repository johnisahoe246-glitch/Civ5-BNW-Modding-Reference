{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Player}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''int''' Player:IsMinorCiv<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|CityBannerManager.lua}}
:<code>UI/InGame/CityBannerManager.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0150}}<syntaxhighlight lang="lua">local isCapital = city:IsCapital() or Players[city:GetOriginalOwner()]:IsMinorCiv();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0152}}<syntaxhighlight lang="lua">if (city:IsCapital() and not player:IsMinorCiv()) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0156}}<syntaxhighlight lang="lua">DoResizeBanner(controls, convertedKey, isCapital, player:IsMinorCiv(), isActiveTeamCity);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0409}}<syntaxhighlight lang="lua">if( player:IsMinorCiv() ) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0425}}<syntaxhighlight lang="lua">if( pOriginalOwner:IsMinorCiv() ) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0465}}<syntaxhighlight lang="lua">elseif (player:IsMinorCiv()) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1115}}<syntaxhighlight lang="lua">if player:IsMinorCiv() then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CityStateStatusHelper.lua (G&K)}}
:<code>DLC/Expansion/UI/CityStateStatusHelper.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0417}}<syntaxhighlight lang="lua">if (Players[iQuestData1]:IsMinorCiv()) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CivsAlive.lua - DLC_01 DLC}}
:<code>DLC/DLC_01/Scenarios/Mongol Scenario/CivsAlive.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0076}}<syntaxhighlight lang="lua">if (Players[playerID]:IsMinorCiv()) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ConfirmGiftPopup.lua}}
:<code>UI/InGame/PopupsGeneric/ConfirmGiftPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0020}}<syntaxhighlight lang="lua">if (pGiftedPlayer:IsMinorCiv()) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DeclareWarMovePopup.lua}}
:<code>UI/InGame/PopupsGeneric/DeclareWarMovePopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0019}}<syntaxhighlight lang="lua">if (not owner:IsMinorCiv() and Teams[Game.GetActiveTeam()]:IsOpenBordersTradingAllowed()) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0025}}<syntaxhighlight lang="lua">if (owner:IsMinorCiv()) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DeclareWarMovePopup.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/PopupsGeneric/DeclareWarMovePopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0019}}<syntaxhighlight lang="lua">if (not owner:IsMinorCiv() and Teams[Game.GetActiveTeam()]:IsOpenBordersTradingAllowedWithTeam(plot:GetTeam())) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|Demographics.lua}}
:<code>UI/InGame/Popups/Demographics.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0047}}<syntaxhighlight lang="lua">if(pPlayer:IsAlive() and not pPlayer:IsMinorCiv()) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DiploList.lua}}
:<code>UI/InGame/DiploList.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0421}}<syntaxhighlight lang="lua">if( pOtherPlayer:IsMinorCiv() and</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0521}}<syntaxhighlight lang="lua">if( Players[iQuestData1]:IsMinorCiv() ) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DiploRelationships.lua}}
:<code>UI/InGame/Popups/DiploRelationships.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0057}}<syntaxhighlight lang="lua">if (pOtherPlayer:IsMinorCiv()) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DiploVotePopup.lua}}
:<code>UI/InGame/Popups/DiploVotePopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0060}}<syntaxhighlight lang="lua">if (not pOtherPlayer:IsMinorCiv()) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|EnemyUnitPanel.lua}}
:<code>UI/InGame/WorldView/EnemyUnitPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0105}}<syntaxhighlight lang="lua">if pPlayer:IsMinorCiv() then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1073}}<syntaxhighlight lang="lua">if (iModifier ~= 0 and pTheirPlayer:IsMinorCiv()) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|PlotMouseoverInclude.lua}}
:<code>UI/InGame/PlotMouseoverInclude.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0012}}<syntaxhighlight lang="lua">if( pOtherPlayer:IsMinorCiv() and iActiveTeam ~= iOtherTeam and pOtherPlayer:IsAlive() and pTeam:IsHasMet( iOtherTeam ) ) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TradeLogic.lua}}
:<code>UI/InGame/WorldView/TradeLogic.lua</code>
:{{CodeBegin5}}
{{CodeLine5|2578}}<syntaxhighlight lang="lua">elseif (pLoopPlayer:IsMinorCiv()) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|2616}}<syntaxhighlight lang="lua">elseif (pLoopPlayer:IsMinorCiv() and pLoopPlayer:GetAlly() == iFromPlayer) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TradeLogic.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/WorldView/TradeLogic.lua</code>
:{{CodeBegin5}}
{{CodeLine5|2985}}<syntaxhighlight lang="lua">if (Players[iOtherPlayer]:IsMinorCiv()) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TurnsRemaining.lua - DLC_02 DLC}}
:<code>DLC/DLC_02/Scenarios/NewWorldScenario/TurnsRemaining.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0099}}<syntaxhighlight lang="lua">if( pPlayer1:IsMinorCiv() ) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0145}}<syntaxhighlight lang="lua">if (bAdjacentChina and not player:IsMinorCiv() and not player:IsBarbarian()) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0408}}<syntaxhighlight lang="lua">if (pPlayer:IsAlive() and not pPlayer:IsMinorCiv() and (iPlayer == iNWOwner or iNWOwner == -1 or iNWOwner > 7)) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0452}}<syntaxhighlight lang="lua">if( newPlayer:IsMinorCiv() ) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0457}}<syntaxhighlight lang="lua">if (not oldPlayer:IsMinorCiv()) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TurnsRemaining.lua (G&K)}}
:<code>DLC/Expansion/Scenarios/MedievalScenario/TurnsRemaining.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0651}}<syntaxhighlight lang="lua">if (bAdjacentChina and not player:IsMinorCiv() and not player:IsBarbarian() and iNumConquistadors < 3) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TurnsRemaining.lua (G&K)}}
:<code>DLC/Expansion/Scenarios/SteampunkScenario/TurnsRemaining.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0516}}<syntaxhighlight lang="lua">if (not pPlayer:IsMinorCiv() and pPlayer:GetNumCities() == 1) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TutorialChecks.lua}}
:<code>Tutorial/TutorialChecks.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1125}}<syntaxhighlight lang="lua">if (pOtherPlayer:IsMinorCiv() and pOtherPlayer:IsAlive() and not pTeam:IsAtWar(iOtherTeam)) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|2464}}<syntaxhighlight lang="lua">if (iPlotOwner >= 0 and Players[iPlotOwner]:IsMinorCiv() and not pTeam:IsAtWar(iPlotTeam)) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|UnitPanel.lua}}
:<code>UI/InGame/WorldView/UnitPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0451}}<syntaxhighlight lang="lua">if( pPlayer:IsMinorCiv() ) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|VictoryProgress.lua}}
:<code>UI/InGame/Popups/VictoryProgress.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0217}}<syntaxhighlight lang="lua">if(not pPlayer:IsMinorCiv() and pPlayer:IsEverAlive()) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0447}}<syntaxhighlight lang="lua">if(not v:IsMinorCiv() and v:IsAlive() and (leadAI == nil or v:GetNumPolicyBranchesFinished() > maxPolicies) and i ~= Game.GetActivePlayer()) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|VictoryProgress.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/Popups/VictoryProgress.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0720}}<syntaxhighlight lang="lua">if (pLeaderLoop:IsMinorCiv() and pTeamLoop:GetTeamVotingForInDiplo() == iTeam) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0735}}<syntaxhighlight lang="lua">elseif (not pLeaderLoop:IsMinorCiv() and Game.GetPreviousVoteCast(iTeamLoop) == iTeam) then</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|IsMinorCiv]]
[[Category:Civ5 City States API|IsMinorCiv]]