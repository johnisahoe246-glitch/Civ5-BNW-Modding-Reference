{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This method is declared by {{Type5|Context}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''void''' UIElement:SetUpdate<b>(</b>('''void''' func<b>(</b>'''float''' fTimeDelta<b>)</b>) UpdateHandler<b>)</b></code>


'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|UpdateHandler:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Too many occurences. Only 50 out of 25 are listed.''

{{PseudoH4|CivsAlive.lua - DLC_01 DLC}}
:<code>DLC/DLC_01/Scenarios/Mongol Scenario/CivsAlive.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0031}}<syntaxhighlight lang="lua">ContextPtr:SetUpdate(function()</syntaxhighlight>
{{CodeLine5|0032}}<syntaxhighlight lang="lua">if (Game.GetGameState() == GameplayGameStateTypes.GAMESTATE_ON) then</syntaxhighlight>
{{CodeLine5|0033}}<syntaxhighlight lang="lua">-- Display victory information</syntaxhighlight>
{{CodeLine5|0034}}<syntaxhighlight lang="lua">local iRemainingToDestroy, iTurnsRemaining = GetVictoryValues();</syntaxhighlight>
{{CodeLine5|0035}}<syntaxhighlight lang="lua">Controls.CivsAliveLabel:LocalizeAndSetText("TXT_KEY_MONGOL_SCENARIO_CIVSALIVE", iRemainingToDestroy, iTurnsRemaining);</syntaxhighlight>
{{CodeLine5|0036}}<syntaxhighlight lang="lua">Controls.Grid:DoAutoSize();</syntaxhighlight>
{{CodeLine5|0037}}<syntaxhighlight lang="lua">else</syntaxhighlight>
{{CodeLine5|0038}}<syntaxhighlight lang="lua">-- Game over, hide the UI</syntaxhighlight>
{{CodeLine5|0039}}<syntaxhighlight lang="lua">ContextPtr:ClearUpdate();</syntaxhighlight>
{{CodeLine5|0040}}<syntaxhighlight lang="lua">ContextPtr:SetHide( true );</syntaxhighlight>
{{CodeLine5|0041}}<syntaxhighlight lang="lua">end</syntaxhighlight>
{{CodeLine5|0042}}<syntaxhighlight lang="lua">end);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CustomMod.lua}}
:<code>UI/FrontEnd/Modding/CustomMod.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0058}}<syntaxhighlight lang="lua">ContextPtr:SetUpdate( function()</syntaxhighlight>
{{CodeLine5|0059}}<syntaxhighlight lang="lua">if(g_ModList == nil) then</syntaxhighlight>
{{CodeLine5|0060}}<syntaxhighlight lang="lua">SetupFileButtonList();</syntaxhighlight>
{{CodeLine5|0061}}<syntaxhighlight lang="lua">end</syntaxhighlight>
{{CodeLine5|0062}}<syntaxhighlight lang="lua">end);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DebugMenu.lua}}
:<code>UI/InGame/DebugMenu.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0293}}<syntaxhighlight lang="lua">ContextPtr:SetUpdate( UpdateHandler );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|EndGameMenu.lua}}
:<code>UI/InGame/Popups/EndGameMenu.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0108}}<syntaxhighlight lang="lua">ContextPtr:SetUpdate( OnUpdate );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|InstalledPanel.lua}}
:<code>UI/FrontEnd/Modding/InstalledPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0489}}<syntaxhighlight lang="lua">ContextPtr:SetUpdate(OnUpdate);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|NetworkDebug.lua}}
:<code>UI/InGame/NetworkDebug.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0050}}<syntaxhighlight lang="lua">ContextPtr:SetUpdate(UpdateNetworkDisplay);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TurnsRemaining.lua - DLC_02 DLC}}
:<code>DLC/DLC_02/Scenarios/NewWorldScenario/TurnsRemaining.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0004}}<syntaxhighlight lang="lua">ContextPtr:SetUpdate(function()</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0006}}<syntaxhighlight lang="lua">local iTurnsRemaining = 100 - Game.GetGameTurn();</syntaxhighlight>
{{CodeLine5|0007}}<syntaxhighlight lang="lua">if (iTurnsRemaining < 1) then</syntaxhighlight>
{{CodeLine5|0008}}<syntaxhighlight lang="lua">Game.SetGameState(GameplayGameStateTypes.GAMESTATE_OVER);</syntaxhighlight>
{{CodeLine5|0009}}<syntaxhighlight lang="lua">ContextPtr:ClearUpdate();</syntaxhighlight>
{{CodeLine5|0010}}<syntaxhighlight lang="lua">ContextPtr:SetHide( true );</syntaxhighlight>
{{CodeLine5|0011}}<syntaxhighlight lang="lua">end</syntaxhighlight>
{{CodeLine5|0012}}<syntaxhighlight lang="lua">-- Loop through all the Majors</syntaxhighlight>
{{CodeLine5|0013}}<syntaxhighlight lang="lua">for iPlayerLoop = 0, GameDefines.MAX_MAJOR_CIVS-1, 1 do</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0015}}<syntaxhighlight lang="lua">   local player = Players[iPlayerLoop];</syntaxhighlight>
{{CodeLine5|0016}}<syntaxhighlight lang="lua">   if (player:IsAlive()) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0018}}<syntaxhighlight lang="lua">   if (player:GetScore() >= 1000) then</syntaxhighlight>
{{CodeLine5|0019}}<syntaxhighlight lang="lua">   print(string.format("Player %i has won w/ a score of %i", iPlayerLoop, player:GetScore()));</syntaxhighlight>
{{CodeLine5|0020}}<syntaxhighlight lang="lua">   Game.SetWinner(player:GetTeam(), GameInfo.Victories["VICTORY_DOMINATION"].ID);</syntaxhighlight>
{{CodeLine5|0021}}<syntaxhighlight lang="lua">   ContextPtr:ClearUpdate();</syntaxhighlight>
{{CodeLine5|0022}}<syntaxhighlight lang="lua">   ContextPtr:SetHide( true );</syntaxhighlight>
{{CodeLine5|0023}}<syntaxhighlight lang="lua">   end</syntaxhighlight>
{{CodeLine5|0024}}<syntaxhighlight lang="lua">   end</syntaxhighlight>
{{CodeLine5|0025}}<syntaxhighlight lang="lua">   end</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0027}}<syntaxhighlight lang="lua">   Controls.TurnsRemainingLabel:LocalizeAndSetText("TXT_KEY_NEWWORLD_SCENARIO_TURNSREMAINING", iTurnsRemaining);</syntaxhighlight>
{{CodeLine5|0028}}<syntaxhighlight lang="lua">   Controls.Grid:DoAutoSize();</syntaxhighlight>
{{CodeLine5|0029}}<syntaxhighlight lang="lua">   end);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TurnsRemaining.lua - DLC_04 DLC}}
:<code>DLC/DLC_04/Scenarios/1066Scenario/TurnsRemaining.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0004}}<syntaxhighlight lang="lua">ContextPtr:SetUpdate(function()</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0006}}<syntaxhighlight lang="lua">local iTurnsRemaining = 70 - Game.GetGameTurn();</syntaxhighlight>
{{CodeLine5|0007}}<syntaxhighlight lang="lua">local iOtherLeadersAlive = 0;</syntaxhighlight>
{{CodeLine5|0008}}<syntaxhighlight lang="lua">local iLondonPlayer = -1;</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0010}}<syntaxhighlight lang="lua">-- Loop through all the Majors checking for victory</syntaxhighlight>
{{CodeLine5|0011}}<syntaxhighlight lang="lua">for iPlayerLoop = 0, GameDefines.MAX_MAJOR_CIVS-1, 1 do</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0013}}<syntaxhighlight lang="lua">   local player = Players[iPlayerLoop];</syntaxhighlight>
{{CodeLine5|0014}}<syntaxhighlight lang="lua">   if (player:IsAlive()) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0016}}<syntaxhighlight lang="lua">   iOtherLeadersAlive = iOtherLeadersAlive + 1;</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0018}}<syntaxhighlight lang="lua">   -- Controls London?</syntaxhighlight>
{{CodeLine5|0019}}<syntaxhighlight lang="lua">   local pLondon = Map.GetPlot(43,17):GetPlotCity();</syntaxhighlight>
{{CodeLine5|0020}}<syntaxhighlight lang="lua">   if (pLondon:GetOwner() == iPlayerLoop) then</syntaxhighlight>
{{CodeLine5|0021}}<syntaxhighlight lang="lua">   iLondonPlayer = iPlayerLoop;</syntaxhighlight>
{{CodeLine5|0022}}<syntaxhighlight lang="lua">   if (pLondon:GetNumBuilding(GameInfo.Buildings["BUILDING_NATIONAL_COLLEGE"].ID) > 0) then</syntaxhighlight>
{{CodeLine5|0023}}<syntaxhighlight lang="lua">   Game.SetWinner(player:GetTeam(), GameInfo.Victories["VICTORY_DOMINATION"].ID);</syntaxhighlight>
{{CodeLine5|0024}}<syntaxhighlight lang="lua">   ContextPtr:ClearUpdate();</syntaxhighlight>
{{CodeLine5|0025}}<syntaxhighlight lang="lua">   ContextPtr:SetHide( true );</syntaxhighlight>
{{CodeLine5|0026}}<syntaxhighlight lang="lua">   end</syntaxhighlight>
{{CodeLine5|0027}}<syntaxhighlight lang="lua">   end</syntaxhighlight>
{{CodeLine5|0028}}<syntaxhighlight lang="lua">   end</syntaxhighlight>
{{CodeLine5|0029}}<syntaxhighlight lang="lua">   end</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0032}}<syntaxhighlight lang="lua">   if (iTurnsRemaining < 1 or Game.GetGameState() == GameplayGameStateTypes.GAMESTATE_EXTENDED) then</syntaxhighlight>
{{CodeLine5|0033}}<syntaxhighlight lang="lua">   Game.SetGameState(GameplayGameStateTypes.GAMESTATE_OVER);</syntaxhighlight>
{{CodeLine5|0034}}<syntaxhighlight lang="lua">   ContextPtr:ClearUpdate();</syntaxhighlight>
{{CodeLine5|0035}}<syntaxhighlight lang="lua">   ContextPtr:SetHide( true );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0037}}<syntaxhighlight lang="lua">   elseif (iOtherLeadersAlive == 0) then</syntaxhighlight>
{{CodeLine5|0038}}<syntaxhighlight lang="lua">   Game.SetWinner(Players[Game.GetActivePlayer()]:GetTeam(), GameInfo.Victories["VICTORY_DOMINATION"].ID);</syntaxhighlight>
{{CodeLine5|0039}}<syntaxhighlight lang="lua">   ContextPtr:SetHide( true );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0041}}<syntaxhighlight lang="lua">   else</syntaxhighlight>
{{CodeLine5|0042}}<syntaxhighlight lang="lua">   local londonText;</syntaxhighlight>
{{CodeLine5|0043}}<syntaxhighlight lang="lua">   local shireCourtText;</syntaxhighlight>
{{CodeLine5|0044}}<syntaxhighlight lang="lua">   local turnsRemainingText = Locale.ConvertTextKey("TXT_KEY_1066_SCENARIO_TURNSREMAINING", iTurnsRemaining);</syntaxhighlight>
{{CodeLine5|0045}}<syntaxhighlight lang="lua">   if (iLondonPlayer ~= -1) then</syntaxhighlight>
{{CodeLine5|0046}}<syntaxhighlight lang="lua">   local londonText = Locale.ConvertTextKey("TXT_KEY_1066_SCENARIO_LONDON_STATUS", Players[iLondonPlayer]:GetCivilizationShortDescriptionKey());</syntaxhighlight>
{{CodeLine5|0047}}<syntaxhighlight lang="lua">   local shireCourtText = Locale.ConvertTextKey("TXT_KEY_1066_SCENARIO_SHIRE_COURT_STATUS", Players[iLondonPlayer]:CountNumBuildings(GameInfo.Buildings["BUILDING_COURTHOUSE"].ID));</syntaxhighlight>
{{CodeLine5|0048}}<syntaxhighlight lang="lua">   turnsRemainingText = turnsRemainingText .. "[NEWLINE]" .. londonText .. "[NEWLINE]" .. shireCourtText;</syntaxhighlight>
{{CodeLine5|0049}}<syntaxhighlight lang="lua">   end</syntaxhighlight>
{{CodeLine5|0050}}<syntaxhighlight lang="lua">   Controls.TurnsRemainingLabel:LocalizeAndSetText(turnsRemainingText);</syntaxhighlight>
{{CodeLine5|0051}}<syntaxhighlight lang="lua">   Controls.Grid:DoAutoSize();</syntaxhighlight>
{{CodeLine5|0052}}<syntaxhighlight lang="lua">   end</syntaxhighlight>
{{CodeLine5|0053}}<syntaxhighlight lang="lua">   end);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TurnsRemaining.lua (G&K)}}
:<code>DLC/Expansion/Scenarios/MedievalScenario/TurnsRemaining.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0074}}<syntaxhighlight lang="lua">ContextPtr:SetUpdate(function()</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0076}}<syntaxhighlight lang="lua">if (g_ScenarioDone) then</syntaxhighlight>
{{CodeLine5|0077}}<syntaxhighlight lang="lua">ContextPtr:ClearUpdate();</syntaxhighlight>
{{CodeLine5|0078}}<syntaxhighlight lang="lua">ContextPtr:SetHide( true );</syntaxhighlight>
{{CodeLine5|0079}}<syntaxhighlight lang="lua">end</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0081}}<syntaxhighlight lang="lua">local iTurnsRemaining = 200 - Game.GetGameTurn();</syntaxhighlight>
{{CodeLine5|0082}}<syntaxhighlight lang="lua">local turnsRemainingText = Locale.ConvertTextKey("TXT_KEY_MEDIEVAL_SCENARIO_TURNSREMAINING", iTurnsRemaining);</syntaxhighlight>
{{CodeLine5|0083}}<syntaxhighlight lang="lua">Controls.TurnsRemainingLabel:LocalizeAndSetText(turnsRemainingText);</syntaxhighlight>
{{CodeLine5|0084}}<syntaxhighlight lang="lua">Controls.Grid:DoAutoSize();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0086}}<syntaxhighlight lang="lua">end);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TurnsRemaining.lua (G&K)}}
:<code>DLC/Expansion/Scenarios/FallOfRomeScenario/TurnsRemaining.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0007}}<syntaxhighlight lang="lua">ContextPtr:SetUpdate(function()</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0009}}<syntaxhighlight lang="lua">if (g_ScenarioDone) then</syntaxhighlight>
{{CodeLine5|0010}}<syntaxhighlight lang="lua">ContextPtr:ClearUpdate();</syntaxhighlight>
{{CodeLine5|0011}}<syntaxhighlight lang="lua">ContextPtr:SetHide( true );</syntaxhighlight>
{{CodeLine5|0012}}<syntaxhighlight lang="lua">end</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0014}}<syntaxhighlight lang="lua">local iTurnsRemaining = g_iGameTurnLength - Game.GetGameTurn();</syntaxhighlight>
{{CodeLine5|0015}}<syntaxhighlight lang="lua">local turnsRemainingText = Locale.ConvertTextKey("TXT_KEY_FOR_SCENARIO_TURNS_REMAINING", iTurnsRemaining);</syntaxhighlight>
{{CodeLine5|0016}}<syntaxhighlight lang="lua">Controls.TurnsRemainingLabel:LocalizeAndSetText(turnsRemainingText);</syntaxhighlight>
{{CodeLine5|0017}}<syntaxhighlight lang="lua">Controls.Grid:DoAutoSize();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0019}}<syntaxhighlight lang="lua">end);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TurnsRemaining.lua (G&K)}}
:<code>DLC/Expansion/Scenarios/SteampunkScenario/TurnsRemaining.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0082}}<syntaxhighlight lang="lua">ContextPtr:SetUpdate(function()</syntaxhighlight>
{{CodeLine5|0083}}<syntaxhighlight lang="lua">if (gbScenarioDone) then</syntaxhighlight>
{{CodeLine5|0084}}<syntaxhighlight lang="lua">ContextPtr:ClearUpdate();</syntaxhighlight>
{{CodeLine5|0085}}<syntaxhighlight lang="lua">end</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0087}}<syntaxhighlight lang="lua">if (not gbUpdated) then</syntaxhighlight>
{{CodeLine5|0088}}<syntaxhighlight lang="lua">local iActivePlayer = Game.GetActivePlayer();</syntaxhighlight>
{{CodeLine5|0089}}<syntaxhighlight lang="lua">local strStatus = Locale.Lookup("TXT_KEY_STEAMPUNK_SCENARIO_TURNS_REMAINING", GetNumTokensOwned(iActivePlayer), GetNumTokensUnlocked(Game.GetGameTurn() - 1)); --antonjs: consider: keep var for last turn updated</syntaxhighlight>
{{CodeLine5|0090}}<syntaxhighlight lang="lua">if (giPlayerAboutToWin == iActivePlayer) then</syntaxhighlight>
{{CodeLine5|0091}}<syntaxhighlight lang="lua">strStatus = "[COLOR_POSITIVE_TEXT]" .. strStatus .. "[ENDCOLOR]";</syntaxhighlight>
{{CodeLine5|0092}}<syntaxhighlight lang="lua">elseif (giPlayerAboutToWin ~= -1) then</syntaxhighlight>
{{CodeLine5|0093}}<syntaxhighlight lang="lua">strStatus = "[COLOR_WARNING_TEXT]" .. strStatus .. "[ENDCOLOR]";</syntaxhighlight>
{{CodeLine5|0094}}<syntaxhighlight lang="lua">end</syntaxhighlight>
{{CodeLine5|0095}}<syntaxhighlight lang="lua">Controls.QuickStatusLabel:SetText(strStatus);</syntaxhighlight>
{{CodeLine5|0096}}<syntaxhighlight lang="lua">gbUpdated = true;</syntaxhighlight>
{{CodeLine5|0097}}<syntaxhighlight lang="lua">end</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0099}}<syntaxhighlight lang="lua">Controls.Grid:DoAutoSize();</syntaxhighlight>
{{CodeLine5|0100}}<syntaxhighlight lang="lua">end);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|VictoryStatus.lua (G&K)}}
:<code>DLC/Expansion/Scenarios/SteampunkScenario/VictoryStatus.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0072}}<syntaxhighlight lang="lua">ContextPtr:SetUpdate(function()</syntaxhighlight>
{{CodeLine5|0073}}<syntaxhighlight lang="lua">if (not gbUpdated) then</syntaxhighlight>
{{CodeLine5|0074}}<syntaxhighlight lang="lua">local iActivePlayer = Game:GetActivePlayer();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0076}}<syntaxhighlight lang="lua">local iTokensNeededForVictory = GetTokensNeededForVictory();</syntaxhighlight>
{{CodeLine5|0077}}<syntaxhighlight lang="lua">local sHelpText = Locale.Lookup("TXT_KEY_STEAMPUNK_SCENARIO_VICTORY_HELP", iTokensNeededForVictory, GetTurnsMustHoldForVictory());</syntaxhighlight>
{{CodeLine5|0078}}<syntaxhighlight lang="lua">sHelpText = sHelpText .. "[NEWLINE][NEWLINE]";</syntaxhighlight>
{{CodeLine5|0079}}<syntaxhighlight lang="lua">if (not IsVictoryPossible(giYearUpdated)) then</syntaxhighlight>
{{CodeLine5|0080}}<syntaxhighlight lang="lua">sHelpText = sHelpText .. Locale.Lookup("TXT_KEY_STEAMPUNK_SCENARIO_VICTORY_LOCKED") .. "  ";</syntaxhighlight>
{{CodeLine5|0081}}<syntaxhighlight lang="lua">elseif (giPlayerAboutToWin ~= -1) then</syntaxhighlight>
{{CodeLine5|0082}}<syntaxhighlight lang="lua">local iTurnsUntilWin = GetTurnsMustHoldForVictory() - giTurnsControlHeld;</syntaxhighlight>
{{CodeLine5|0083}}<syntaxhighlight lang="lua">if (iTurnsUntilWin < 0) then</syntaxhighlight>
{{CodeLine5|0084}}<syntaxhighlight lang="lua">iTurnsUntilWin = 0;</syntaxhighlight>
{{CodeLine5|0085}}<syntaxhighlight lang="lua">end</syntaxhighlight>
{{CodeLine5|0086}}<syntaxhighlight lang="lua">local sCivAboutToWinKey = Players[giPlayerAboutToWin]:GetCivilizationShortDescriptionKey();</syntaxhighlight>
{{CodeLine5|0087}}<syntaxhighlight lang="lua">local sCountdownText = Locale.Lookup("TXT_KEY_STEAMPUNK_SCENARIO_VICTORY_COUNTDOWN", iTurnsUntilWin, sCivAboutToWinKey) .. "  ";</syntaxhighlight>
{{CodeLine5|0088}}<syntaxhighlight lang="lua">if (giPlayerAboutToWin == iActivePlayer) then</syntaxhighlight>
{{CodeLine5|0089}}<syntaxhighlight lang="lua">sCountdownText = "[COLOR_POSITIVE_TEXT]" .. sCountdownText .. "[ENDCOLOR]";</syntaxhighlight>
{{CodeLine5|0090}}<syntaxhighlight lang="lua">else</syntaxhighlight>
{{CodeLine5|0091}}<syntaxhighlight lang="lua">sCountdownText = "[COLOR_WARNING_TEXT]" .. sCountdownText .. "[ENDCOLOR]";</syntaxhighlight>
{{CodeLine5|0092}}<syntaxhighlight lang="lua">end</syntaxhighlight>
{{CodeLine5|0093}}<syntaxhighlight lang="lua">sHelpText = sHelpText .. sCountdownText;</syntaxhighlight>
{{CodeLine5|0094}}<syntaxhighlight lang="lua">end</syntaxhighlight>
{{CodeLine5|0095}}<syntaxhighlight lang="lua">sHelpText = sHelpText .. Locale.Lookup("TXT_KEY_STEAMPUNK_SCENARIO_VICTORY_POSSIBLE", giYearUpdated); --antonjs: todo: separate line, general UI stuff</syntaxhighlight>
{{CodeLine5|0096}}<syntaxhighlight lang="lua">Controls.HelpLabel:SetText(sHelpText);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0098}}<syntaxhighlight lang="lua">for s,t in pairs(ktTokens) do</syntaxhighlight>
{{CodeLine5|0099}}<syntaxhighlight lang="lua">   local bUnlocked = IsTokenUnlocked(s, giTurnUpdated);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0101}}<syntaxhighlight lang="lua">   gtTokenUI[s].TitleLabel:SetText(t.Title .. "  ");</syntaxhighlight>
{{CodeLine5|0102}}<syntaxhighlight lang="lua">   gtTokenUI[s].PortraitFrame:SetHide(true);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0104}}<syntaxhighlight lang="lua">   local sLabelText = "[ICON_LOCKED]  ";</syntaxhighlight>
{{CodeLine5|0105}}<syntaxhighlight lang="lua">   if (bUnlocked) then</syntaxhighlight>
{{CodeLine5|0106}}<syntaxhighlight lang="lua">   sLabelText = "[ICON_BULLET]  ";</syntaxhighlight>
{{CodeLine5|0107}}<syntaxhighlight lang="lua">   end</syntaxhighlight>
{{CodeLine5|0108}}<syntaxhighlight lang="lua">   sLabelText = sLabelText .. t.Help .. "[NEWLINE]      ";</syntaxhighlight>
{{CodeLine5|0109}}<syntaxhighlight lang="lua">   local iNumInList = 0;</syntaxhighlight>
{{CodeLine5|0110}}<syntaxhighlight lang="lua">   for iPlayer = 0, GameDefines.MAX_MAJOR_CIVS - 1, 1 do</syntaxhighlight>
{{CodeLine5|0111}}<syntaxhighlight lang="lua">   if (Players[iPlayer]:IsAlive()) then</syntaxhighlight>
{{CodeLine5|0112}}<syntaxhighlight lang="lua">   if (iNumInList ~= 0) then</syntaxhighlight>
{{CodeLine5|0113}}<syntaxhighlight lang="lua">   sLabelText = sLabelText .. ", ";</syntaxhighlight>
{{CodeLine5|0114}}<syntaxhighlight lang="lua">   end</syntaxhighlight>
{{CodeLine5|0115}}<syntaxhighlight lang="lua">   iNumInList = iNumInList + 1;</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0117}}<syntaxhighlight lang="lua">   local sCivDesc = Locale.Lookup(Players[iPlayer]:GetCivilizationShortDescriptionKey());</syntaxhighlight>
{{CodeLine5|0118}}<syntaxhighlight lang="lua">   if (iPlayer == iActivePlayer) then</syntaxhighlight>
{{CodeLine5|0119}}<syntaxhighlight lang="lua">   sCivDesc = Locale.Lookup("TXT_KEY_YOU");</syntaxhighlight>
{{CodeLine5|0120}}<syntaxhighlight lang="lua">   end</syntaxhighlight>
{{CodeLine5|0121}}<syntaxhighlight lang="lua">   sCivDesc = sCivDesc .. ": " .. gtPlayerStatus[iPlayer][s].Value;</syntaxhighlight>
{{CodeLine5|0122}}<syntaxhighlight lang="lua">   if (gtPlayerStatus[iPlayer][s].Owned) then</syntaxhighlight>
{{CodeLine5|0123}}<syntaxhighlight lang="lua">   sCivDesc = "[COLOR_POSITIVE_TEXT]" .. sCivDesc .. "[ENDCOLOR]";</syntaxhighlight>
{{CodeLine5|0124}}<syntaxhighlight lang="lua">   local pPlayer = Players[iPlayer];</syntaxhighlight>
{{CodeLine5|0125}}<syntaxhighlight lang="lua">   if (pPlayer ~= nil) then</syntaxhighlight>
{{CodeLine5|0126}}<syntaxhighlight lang="lua">   local tLeader = GameInfo.Leaders[pPlayer:GetLeaderType()];</syntaxhighlight>
{{CodeLine5|0127}}<syntaxhighlight lang="lua">   IconHookup( tLeader.PortraitIndex, 64, tLeader.IconAtlas, gtTokenUI[s].Portrait );</syntaxhighlight>
{{CodeLine5|0128}}<syntaxhighlight lang="lua">   gtTokenUI[s].PortraitFrame:SetHide(false);</syntaxhighlight>
{{CodeLine5|0129}}<syntaxhighlight lang="lua">   else</syntaxhighlight>
{{CodeLine5|0130}}<syntaxhighlight lang="lua">   print("SCRIPTING ERROR: Got nil when looking for player that owns a Title");</syntaxhighlight>
{{CodeLine5|0131}}<syntaxhighlight lang="lua">   end</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0133}}<syntaxhighlight lang="lua">   end</syntaxhighlight>
{{CodeLine5|0134}}<syntaxhighlight lang="lua">   sLabelText = sLabelText .. sCivDesc;</syntaxhighlight>
{{CodeLine5|0135}}<syntaxhighlight lang="lua">   end</syntaxhighlight>
{{CodeLine5|0136}}<syntaxhighlight lang="lua">   end</syntaxhighlight>
{{CodeLine5|0137}}<syntaxhighlight lang="lua">   local sLabelTT = GetTokenTooltip(s, iActivePlayer);</syntaxhighlight>
{{CodeLine5|0138}}<syntaxhighlight lang="lua">   gtTokenUI[s].TokenLabel:SetText(sLabelText);</syntaxhighlight>
{{CodeLine5|0139}}<syntaxhighlight lang="lua">   gtTokenUI[s].TokenLabel:SetToolTipString(sLabelTT);</syntaxhighlight>
{{CodeLine5|0140}}<syntaxhighlight lang="lua">   end</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0142}}<syntaxhighlight lang="lua">   gbUpdated = true;</syntaxhighlight>
{{CodeLine5|0143}}<syntaxhighlight lang="lua">   end</syntaxhighlight>
{{CodeLine5|0144}}<syntaxhighlight lang="lua">   end);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|SetUpdate]]