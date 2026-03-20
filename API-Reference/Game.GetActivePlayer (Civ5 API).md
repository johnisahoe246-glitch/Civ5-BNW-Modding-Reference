{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Game}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>{{Type5|PlayerID}} Game.GetActivePlayer<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
''Too many occurences. Only 50 out of 513 are listed.''

{{PseudoH4|ActionInfoPanel.lua}}
:<code>UI/InGame/WorldView/ActionInfoPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0074}}<syntaxhighlight lang="lua">local player = Players[Game.GetActivePlayer()];</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0233}}<syntaxhighlight lang="lua">local iActivePlayer = Game.GetActivePlayer();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0414}}<syntaxhighlight lang="lua">local pPlayer = Players[Game.GetActivePlayer()];</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|AdvisorCounselPopup.lua}}
:<code>UI/InGame/Popups/AdvisorCounselPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0195}}<syntaxhighlight lang="lua">CivIconHookup( Game.GetActivePlayer(), 64, Controls.Icon, Controls.CivIconBG, Controls.CivIconShadow, false, true );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ChangePassword.lua}}
:<code>UI/InGame/ChangePassword.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0008}}<syntaxhighlight lang="lua">local ePlayer = Game.GetActivePlayer();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0015}}<syntaxhighlight lang="lua">LuaEvents.PasswordChanged( Game.GetActivePlayer() );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CityBannerManager.lua}}
:<code>UI/InGame/CityBannerManager.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0814}}<syntaxhighlight lang="lua">local active_team = Players[Game.GetActivePlayer()]:GetTeam();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0992}}<syntaxhighlight lang="lua">if (player:GetID() ~= Game.GetActivePlayer()) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CityStateDiploPopup.lua}}
:<code>UI/InGame/Popups/CityStateDiploPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0643}}<syntaxhighlight lang="lua">if (iPlayerLoop ~= Game.GetActivePlayer()) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CityStateDiploPopup.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/Popups/CityStateDiploPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0637}}<syntaxhighlight lang="lua">Game.DoMinorPledgeProtection(Game.GetActivePlayer(), g_iMinorCivID, true);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CityStateGreetingPopup.lua}}
:<code>UI/InGame/Popups/CityStateGreetingPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0227}}<syntaxhighlight lang="lua">if (iAlly ~= Game.GetActivePlayer()) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CivilopediaScreen.lua}}
:<code>UI/Civilopedia/CivilopediaScreen.lua</code>
:{{CodeBegin5}}
{{CodeLine5|2348}}<syntaxhighlight lang="lua">cost = Players[Game.GetActivePlayer()]:GetUnitProductionNeeded( unitID );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|2733}}<syntaxhighlight lang="lua">cost = Players[Game.GetActivePlayer()]:GetBuildingProductionNeeded( buildingID );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|Demographics.lua}}
:<code>UI/InGame/Popups/Demographics.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0464}}<syntaxhighlight lang="lua">BuildList( Game.GetActivePlayer() );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DiploCorner.lua}}
:<code>UI/InGame/WorldView/DiploCorner.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0041}}<syntaxhighlight lang="lua">{ text = Locale.Lookup("TXT_KEY_POP_NOTIFICATION_LOG"),            call=function() Popup(ButtonPopupTypes.BUTTONPOPUP_NOTIFICATION_LOG,Game.GetActivePlayer()); end };</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0404}}<syntaxhighlight lang="lua">if( which == 1 ) then Events.EndGameShow( EndGameTypes.Technology, Game.GetActivePlayer() );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0406}}<syntaxhighlight lang="lua">elseif( which == 3 ) then Events.EndGameShow( EndGameTypes.Culture, Game.GetActivePlayer() );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0408}}<syntaxhighlight lang="lua">elseif( which == 5 ) then Events.EndGameShow( EndGameTypes.Time, Game.GetActivePlayer() );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DiploCorner.lua - DLC_01 DLC}}
:<code>DLC/DLC_01/Scenarios/Mongol Scenario/DiploCorner.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0030}}<syntaxhighlight lang="lua">g_MultiPullInfo[5] = { text="TXT_KEY_POP_NOTIFICATION_LOG",      call=function() Events.SerialEventGameMessagePopup( { Type = ButtonPopupTypes.BUTTONPOPUP_NOTIFICATION_LOG, Data1 = Game.GetActivePlayer() } ); end };</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DiploCorner.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/WorldView/DiploCorner.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0393}}<syntaxhighlight lang="lua">local iLocalPlayer = Game.GetActivePlayer();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DiploCurrentDeals.lua}}
:<code>UI/InGame/Popups/DiploCurrentDeals.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0138}}<syntaxhighlight lang="lua">local iPlayer = Game.GetActivePlayer();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DiploList.lua}}
:<code>UI/InGame/DiploList.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0017}}<syntaxhighlight lang="lua">local g_iPlayer = Game.GetActivePlayer();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|EspionageOverview.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/Popups/EspionageOverview.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0282}}<syntaxhighlight lang="lua">local activePlayer = Players[Game.GetActivePlayer()];</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0328}}<syntaxhighlight lang="lua">Network.SendMoveSpy(Game.GetActivePlayer(), g_SelectedAgentID, -1, -1);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0717}}<syntaxhighlight lang="lua">Network.SendStageCoup(Game.GetActivePlayer(), v.AgentID);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0975}}<syntaxhighlight lang="lua">CivIconHookup( Game.GetActivePlayer(), 32, entry.CivIcon, entry.CivIconBG, entry.CivIconShadow, false, true);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1237}}<syntaxhighlight lang="lua">if (cityInfo.PlayerID == Game.GetActivePlayer()) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|GameMenu.lua}}
:<code>UI/InGame/Menus/GameMenu.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0286}}<syntaxhighlight lang="lua">info = GameInfo.HandicapInfos[ Players[Game.GetActivePlayer()]:GetHandicapType() ];</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|GenericWorldAnchor.lua}}
:<code>UI/InGame/GenericWorldAnchor.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0102}}<syntaxhighlight lang="lua">if (bShow and not Players[Game.GetActivePlayer()]:CanFound(iPlotX, iPlotY)) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|HappinessInfo.lua}}
:<code>UI/InGame/Popups/HappinessInfo.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0167}}<syntaxhighlight lang="lua">local iPlayerID = Game.GetActivePlayer();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|InGame.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/InGame.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0257}}<syntaxhighlight lang="lua">local iFromPlayer = Game.GetActivePlayer();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|LiberateMinorPopup.lua}}
:<code>UI/InGame/PopupsGeneric/LiberateMinorPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0008}}<syntaxhighlight lang="lua">local pActivePlayer   = Players[Game.GetActivePlayer()];</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|MilitaryOverview.lua}}
:<code>UI/InGame/Popups/MilitaryOverview.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0073}}<syntaxhighlight lang="lua">Events.SerialEventUnitFlagSelected( Game:GetActivePlayer(), unitID );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|PlayerChange.lua}}
:<code>UI/InGame/PlayerChange.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0009}}<syntaxhighlight lang="lua">if (PreGame.TestPassword( Game.GetActivePlayer(), Controls.EnterPasswordEditBox:GetText() )) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0075}}<syntaxhighlight lang="lua">local bValid = PreGame.TestPassword( Game.GetActivePlayer(), Controls.EnterPasswordEditBox:GetText());</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ProductionPopup.lua}}
:<code>UI/InGame/Popups/ProductionPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0808}}<syntaxhighlight lang="lua">if playerID == Game.GetActivePlayer() and cityID == currentCityID then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ReligionOverview.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/Popups/ReligionOverview.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0471}}<syntaxhighlight lang="lua">Network.SendFaithPurchase(Game.GetActivePlayer(), v1, v2);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TradeLogic.lua}}
:<code>UI/InGame/WorldView/TradeLogic.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0095}}<syntaxhighlight lang="lua">g_iUs = Game.GetActivePlayer();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0648}}<syntaxhighlight lang="lua">if( fromPlayer == Game.GetActivePlayer() ) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TurnsRemaining.lua - DLC_04 DLC}}
:<code>DLC/DLC_04/Scenarios/1066Scenario/TurnsRemaining.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0038}}<syntaxhighlight lang="lua">Game.SetWinner(Players[Game.GetActivePlayer()]:GetTeam(), GameInfo.Victories["VICTORY_DOMINATION"].ID);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0158}}<syntaxhighlight lang="lua">if (iOldAlly == Game.GetActivePlayer())   then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0407}}<syntaxhighlight lang="lua">if (iHandicap > 4 and Game.GetActivePlayer() ~= iPlayer) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0421}}<syntaxhighlight lang="lua">if (iHandicap > 6 and Game.GetActivePlayer() ~= iPlayer) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TurnsRemaining.lua (G&K)}}
:<code>DLC/Expansion/Scenarios/MedievalScenario/TurnsRemaining.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0769}}<syntaxhighlight lang="lua">if (Game.GetActivePlayer() == iOwner) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TurnsRemaining.lua (G&K)}}
:<code>DLC/Expansion/Scenarios/FallOfRomeScenario/TurnsRemaining.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0501}}<syntaxhighlight lang="lua">if (IsWesternRoman(Game.GetActivePlayer())) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0966}}<syntaxhighlight lang="lua">local bIsPlayerBarbarian = not IsEmpire(Game.GetActivePlayer());</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|VictoryProgress.lua}}
:<code>UI/InGame/Popups/VictoryProgress.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0447}}<syntaxhighlight lang="lua">if(not v:IsMinorCiv() and v:IsAlive() and (leadAI == nil or v:GetNumPolicyBranchesFinished() > maxPolicies) and i ~= Game.GetActivePlayer()) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0479}}<syntaxhighlight lang="lua">SimpleCivIconHookup( Game.GetActivePlayer(), 64, Controls.Icon );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0904}}<syntaxhighlight lang="lua">elseif(iPlayer == Game.GetActivePlayer()) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|VoteResultsPopup.lua}}
:<code>UI/InGame/Popups/VoteResultsPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0121}}<syntaxhighlight lang="lua">elseif (pVoteCastPlayer:GetID() == Game.GetActivePlayer()) then</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetActivePlayer]]
[[Category:Civ5 Players API|GetActivePlayer]]