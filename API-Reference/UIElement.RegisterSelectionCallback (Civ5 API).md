{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of ControlBase.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''void''' UIElement:RegisterSelectionCallback<b>(</b>('''void''' func<b>(</b>{{Type5|FaithPurchaseType}} v1, '''int''' v2<b>)</b>) OnChatTarget<b>)</b></code>


'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|OnChatTarget:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Too many occurences. Only 50 out of 65 are listed.''

{{PseudoH4|AdvancedSetup.lua}}
:<code>UI/FrontEnd/GameSetup/AdvancedSetup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0436}}<syntaxhighlight lang="lua">pullDown:RegisterSelectionCallback(function(playerID, id)</syntaxhighlight>
{{CodeLine5|0437}}<syntaxhighlight lang="lua">local civID = playableCivs[id] and playableCivs[id].CivID or -1;</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0439}}<syntaxhighlight lang="lua">PreGame.SetCivilization( playerID, civID);</syntaxhighlight>
{{CodeLine5|0440}}<syntaxhighlight lang="lua">PerformPartialSync();</syntaxhighlight>
{{CodeLine5|0441}}<syntaxhighlight lang="lua">end);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0488}}<syntaxhighlight lang="lua">pullDown:RegisterSelectionCallback( function(id)</syntaxhighlight>
{{CodeLine5|0489}}<syntaxhighlight lang="lua">local era = GameInfo.Eras[id];</syntaxhighlight>
{{CodeLine5|0490}}<syntaxhighlight lang="lua">PreGame.SetEra( id );</syntaxhighlight>
{{CodeLine5|0491}}<syntaxhighlight lang="lua">pullDown:GetButton():LocalizeAndSetText(era.Description);</syntaxhighlight>
{{CodeLine5|0492}}<syntaxhighlight lang="lua">PerformPartialSync();</syntaxhighlight>
{{CodeLine5|0493}}<syntaxhighlight lang="lua">end);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0527}}<syntaxhighlight lang="lua">pullDown:RegisterSelectionCallback( function(id)</syntaxhighlight>
{{CodeLine5|0528}}<syntaxhighlight lang="lua">PreGame.SetGameSpeed( id );</syntaxhighlight>
{{CodeLine5|0529}}<syntaxhighlight lang="lua">local gameSpeed = GameInfo.GameSpeeds[id];</syntaxhighlight>
{{CodeLine5|0530}}<syntaxhighlight lang="lua">pullDown:GetButton():LocalizeAndSetText(gameSpeed.Description);</syntaxhighlight>
{{CodeLine5|0531}}<syntaxhighlight lang="lua">pullDown:GetButton():SetToolTipString( Locale.ConvertTextKey( gameSpeed.Help ) );</syntaxhighlight>
{{CodeLine5|0532}}<syntaxhighlight lang="lua">PerformPartialSync();</syntaxhighlight>
{{CodeLine5|0533}}<syntaxhighlight lang="lua">end);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0561}}<syntaxhighlight lang="lua">pullDown:RegisterSelectionCallback(function(id)</syntaxhighlight>
{{CodeLine5|0562}}<syntaxhighlight lang="lua">local handicap = GameInfo.HandicapInfos[id];</syntaxhighlight>
{{CodeLine5|0563}}<syntaxhighlight lang="lua">PreGame.SetHandicap( 0, id );</syntaxhighlight>
{{CodeLine5|0564}}<syntaxhighlight lang="lua">pullDown:GetButton():LocalizeAndSetText(handicap.Description);</syntaxhighlight>
{{CodeLine5|0565}}<syntaxhighlight lang="lua">pullDown:GetButton():LocalizeAndSetToolTip(handicap.Help);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0567}}<syntaxhighlight lang="lua">PerformPartialSync();</syntaxhighlight>
{{CodeLine5|0568}}<syntaxhighlight lang="lua">end);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0601}}<syntaxhighlight lang="lua">pullDown:RegisterSelectionCallback( function(id)</syntaxhighlight>
{{CodeLine5|0602}}<syntaxhighlight lang="lua">if( id == -1 ) then</syntaxhighlight>
{{CodeLine5|0603}}<syntaxhighlight lang="lua">PreGame.SetRandomWorldSize( true );</syntaxhighlight>
{{CodeLine5|0604}}<syntaxhighlight lang="lua">pullDown:GetButton():LocalizeAndSetText("TXT_KEY_RANDOM_MAP_SIZE");</syntaxhighlight>
{{CodeLine5|0605}}<syntaxhighlight lang="lua">pullDown:GetButton():LocalizeAndSetToolTip("TXT_KEY_RANDOM_MAP_SIZE_HELP");</syntaxhighlight>
{{CodeLine5|0606}}<syntaxhighlight lang="lua">else</syntaxhighlight>
{{CodeLine5|0607}}<syntaxhighlight lang="lua">local mapSize = GameInfo.Worlds[id];</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0609}}<syntaxhighlight lang="lua">PreGame.SetRandomWorldSize( false );</syntaxhighlight>
{{CodeLine5|0610}}<syntaxhighlight lang="lua">PreGame.SetWorldSize( id );</syntaxhighlight>
{{CodeLine5|0611}}<syntaxhighlight lang="lua">PreGame.SetNumMinorCivs( mapSize.DefaultMinorCivs );</syntaxhighlight>
{{CodeLine5|0612}}<syntaxhighlight lang="lua">pullDown:GetButton():LocalizeAndSetText(mapSize.Description);</syntaxhighlight>
{{CodeLine5|0613}}<syntaxhighlight lang="lua">pullDown:GetButton():LocalizeAndSetToolTip(mapSize.Help);</syntaxhighlight>
{{CodeLine5|0614}}<syntaxhighlight lang="lua">end</syntaxhighlight>
{{CodeLine5|0615}}<syntaxhighlight lang="lua">ScreenOptions["Teams"].FullSync();</syntaxhighlight>
{{CodeLine5|0616}}<syntaxhighlight lang="lua">PerformPartialSync();</syntaxhighlight>
{{CodeLine5|0617}}<syntaxhighlight lang="lua">end);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0769}}<syntaxhighlight lang="lua">pullDown:RegisterSelectionCallback( function(id)</syntaxhighlight>
{{CodeLine5|0770}}<syntaxhighlight lang="lua">local mapScript = mapScripts[id];</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0772}}<syntaxhighlight lang="lua">-- If this is an "error" entry (invalid WB file for example), do nothing.</syntaxhighlight>
{{CodeLine5|0773}}<syntaxhighlight lang="lua">if(mapScript.Error) then</syntaxhighlight>
{{CodeLine5|0774}}<syntaxhighlight lang="lua">return;</syntaxhighlight>
{{CodeLine5|0775}}<syntaxhighlight lang="lua">end</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0777}}<syntaxhighlight lang="lua">PreGame.SetLoadWBScenario(false);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0779}}<syntaxhighlight lang="lua">if( id == 0 or mapScript == nil) then</syntaxhighlight>
{{CodeLine5|0780}}<syntaxhighlight lang="lua">PreGame.SetRandomMapScript(true);</syntaxhighlight>
{{CodeLine5|0781}}<syntaxhighlight lang="lua">elseif(mapScript.IsEarthMap) then</syntaxhighlight>
{{CodeLine5|0782}}<syntaxhighlight lang="lua">PreGame.SetEarthMap(true);</syntaxhighlight>
{{CodeLine5|0783}}<syntaxhighlight lang="lua">else</syntaxhighlight>
{{CodeLine5|0784}}<syntaxhighlight lang="lua">PreGame.SetEarthMap(false);</syntaxhighlight>
{{CodeLine5|0785}}<syntaxhighlight lang="lua">PreGame.SetRandomMapScript(false);</syntaxhighlight>
{{CodeLine5|0786}}<syntaxhighlight lang="lua">PreGame.SetMapScript(mapScript.FileName);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0788}}<syntaxhighlight lang="lua">if(mapScript.DefaultCityStates ~= nil) then</syntaxhighlight>
{{CodeLine5|0789}}<syntaxhighlight lang="lua">PreGame.SetNumMinorCivs(mapScript.DefaultCityStates);</syntaxhighlight>
{{CodeLine5|0790}}<syntaxhighlight lang="lua">end</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0792}}<syntaxhighlight lang="lua">-- If it's a WB Map, we have more to do.</syntaxhighlight>
{{CodeLine5|0793}}<syntaxhighlight lang="lua">if(mapScript.WBMapData ~= nil) then</syntaxhighlight>
{{CodeLine5|0794}}<syntaxhighlight lang="lua">local wb = mapScript.WBMapData;</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0796}}<syntaxhighlight lang="lua">PreGame.SetEra(wb.StartEra);</syntaxhighlight>
{{CodeLine5|0797}}<syntaxhighlight lang="lua">PreGame.SetGameSpeed(wb.DefaultSpeed);</syntaxhighlight>
{{CodeLine5|0798}}<syntaxhighlight lang="lua">PreGame.SetMaxTurns(wb.MaxTurns);</syntaxhighlight>
{{CodeLine5|0799}}<syntaxhighlight lang="lua">PreGame.SetNumMinorCivs(wb.CityStateCount);</syntaxhighlight>
{{CodeLine5|0800}}<syntaxhighlight lang="lua">PreGame.SetRandomWorldSize(false);</syntaxhighlight>
{{CodeLine5|0801}}<syntaxhighlight lang="lua">PreGame.SetWorldSize(wb.MapSize);</syntaxhighlight>
{{CodeLine5|0802}}<syntaxhighlight lang="lua">PreGame.SetRandomWorldSize(false);</syntaxhighlight>
{{CodeLine5|0803}}<syntaxhighlight lang="lua">PreGame.SetNumMinorCivs(-1);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0805}}<syntaxhighlight lang="lua">local victories = {};</syntaxhighlight>
{{CodeLine5|0806}}<syntaxhighlight lang="lua">for _, v in ipairs(wb.VictoryTypes) do</syntaxhighlight>
{{CodeLine5|0807}}<syntaxhighlight lang="lua">   victories[v] = true;</syntaxhighlight>
{{CodeLine5|0808}}<syntaxhighlight lang="lua">   end</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0810}}<syntaxhighlight lang="lua">   for row in GameInfo.Victories() do</syntaxhighlight>
{{CodeLine5|0811}}<syntaxhighlight lang="lua">   PreGame.SetVictory(row.ID, victories[row.Type]);</syntaxhighlight>
{{CodeLine5|0812}}<syntaxhighlight lang="lua">   end</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0814}}<syntaxhighlight lang="lua">   local numPlayers = wb.PlayerCount;</syntaxhighlight>
{{CodeLine5|0815}}<syntaxhighlight lang="lua">   if(numPlayers == 0) then</syntaxhighlight>
{{CodeLine5|0816}}<syntaxhighlight lang="lua">   numPlayers = GameInfo.Worlds[wb.MapSize].DefaultPlayers</syntaxhighlight>
{{CodeLine5|0817}}<syntaxhighlight lang="lua">   end</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0819}}<syntaxhighlight lang="lua">   for i = numPlayers, GameDefines.MAX_MAJOR_CIVS do</syntaxhighlight>
{{CodeLine5|0820}}<syntaxhighlight lang="lua">   if( PreGame.GetSlotStatus(i) == SlotStatus.SS_COMPUTER) then</syntaxhighlight>
{{CodeLine5|0821}}<syntaxhighlight lang="lua">   PreGame.SetSlotStatus(i, SlotStatus.SS_OPEN);</syntaxhighlight>
{{CodeLine5|0822}}<syntaxhighlight lang="lua">   end</syntaxhighlight>
{{CodeLine5|0823}}<syntaxhighlight lang="lua">   end</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0825}}<syntaxhighlight lang="lua">   ScreenOptions["Teams"].FullSync();</syntaxhighlight>
{{CodeLine5|0826}}<syntaxhighlight lang="lua">   end</syntaxhighlight>
{{CodeLine5|0827}}<syntaxhighlight lang="lua">   end</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0829}}<syntaxhighlight lang="lua">   PerformPartialSync();</syntaxhighlight>
{{CodeLine5|0830}}<syntaxhighlight lang="lua">   end);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0992}}<syntaxhighlight lang="lua">pullDown:RegisterSelectionCallback(function(playerID, playerChoiceID)</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0994}}<syntaxhighlight lang="lua">PreGame.SetTeam(playerID, playerChoiceID);</syntaxhighlight>
{{CodeLine5|0995}}<syntaxhighlight lang="lua">local slotInstance = g_SlotInstances[playerID];</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0997}}<syntaxhighlight lang="lua">if( slotInstance ~= nil ) then</syntaxhighlight>
{{CodeLine5|0998}}<syntaxhighlight lang="lua">slotInstance.TeamLabel:LocalizeAndSetText( "TXT_KEY_MULTIPLAYER_DEFAULT_TEAM_NAME", PreGame.GetTeam(playerID) + 1 );</syntaxhighlight>
{{CodeLine5|0999}}<syntaxhighlight lang="lua">else</syntaxhighlight>
{{CodeLine5|1000}}<syntaxhighlight lang="lua">Controls.TeamLabel:LocalizeAndSetText( "TXT_KEY_MULTIPLAYER_DEFAULT_TEAM_NAME", PreGame.GetTeam(playerID) + 1 );</syntaxhighlight>
{{CodeLine5|1001}}<syntaxhighlight lang="lua">end</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1003}}<syntaxhighlight lang="lua">PerformValidation();</syntaxhighlight>
{{CodeLine5|1004}}<syntaxhighlight lang="lua">end);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DiploCorner.lua}}
:<code>UI/InGame/WorldView/DiploCorner.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0052}}<syntaxhighlight lang="lua">Controls.MultiPull:RegisterSelectionCallback(function(id)</syntaxhighlight>
{{CodeLine5|0053}}<syntaxhighlight lang="lua">local entry = additionalEntries[id];</syntaxhighlight>
{{CodeLine5|0054}}<syntaxhighlight lang="lua">if(entry and entry.call ~= nil) then</syntaxhighlight>
{{CodeLine5|0055}}<syntaxhighlight lang="lua">entry.call();</syntaxhighlight>
{{CodeLine5|0056}}<syntaxhighlight lang="lua">end</syntaxhighlight>
{{CodeLine5|0057}}<syntaxhighlight lang="lua">end);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0307}}<syntaxhighlight lang="lua">Controls.ChatPull:RegisterSelectionCallback( OnChatTarget );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DiploCorner.lua - DLC_01 DLC}}
:<code>DLC/DLC_01/Scenarios/Mongol Scenario/DiploCorner.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0049}}<syntaxhighlight lang="lua">Controls.MultiPull:RegisterSelectionCallback( OnMultiPull );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|InfoCorner.lua}}
:<code>UI/InGame/InfoCorner.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0053}}<syntaxhighlight lang="lua">Controls.LeftPull:RegisterSelectionCallback( OnInfoButton );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|MiniMapPanel.lua}}
:<code>UI/InGame/WorldView/MiniMapPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0207}}<syntaxhighlight lang="lua">pullDown:RegisterSelectionCallback( OnOverlaySelected );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0273}}<syntaxhighlight lang="lua">pullDown:RegisterSelectionCallback( OnIconModeSelected );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|MPGameOptions.lua}}
:<code>UI/FrontEnd/Multiplayer/GameSetup/MPGameOptions.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0431}}<syntaxhighlight lang="lua">Controls.GameSpeedPullDown:RegisterSelectionCallback( SelectSpeed );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0473}}<syntaxhighlight lang="lua">Controls.MapSizePullDown:RegisterSelectionCallback( SelectSize );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0705}}<syntaxhighlight lang="lua">pullDown:RegisterSelectionCallback( TypeSelected );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0724}}<syntaxhighlight lang="lua">Controls.EraPull:RegisterSelectionCallback( OnEraPull );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|OptionsMenu.lua}}
:<code>UI/Options/OptionsMenu.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1119}}<syntaxhighlight lang="lua">Controls.WResolutionPull:RegisterSelectionCallback( OnWResolutionPull );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1134}}<syntaxhighlight lang="lua">Controls.FSResolutionPull:RegisterSelectionCallback( OnFSResolutionPull );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1142}}<syntaxhighlight lang="lua">Controls.MSAAPull:RegisterSelectionCallback( OnMSAAPull );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1218}}<syntaxhighlight lang="lua">Controls.TutorialPull:RegisterSelectionCallback( OnTutorialPull );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1221}}<syntaxhighlight lang="lua">Controls.OverlayPull:RegisterSelectionCallback( OnOverlayPull );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1224}}<syntaxhighlight lang="lua">Controls.ShadowPull:RegisterSelectionCallback( OnShadowPull );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1227}}<syntaxhighlight lang="lua">Controls.FOWPull:RegisterSelectionCallback( OnFOWPull );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1230}}<syntaxhighlight lang="lua">Controls.TerrainDetailPull:RegisterSelectionCallback( OnTerrainDetailPull );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1233}}<syntaxhighlight lang="lua">Controls.TerrainTessPull:RegisterSelectionCallback( OnTerrainTessPull );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1236}}<syntaxhighlight lang="lua">Controls.TerrainShadowPull:RegisterSelectionCallback( OnTerrainShadowPull );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1239}}<syntaxhighlight lang="lua">Controls.WaterPull:RegisterSelectionCallback( OnWaterPull );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1242}}<syntaxhighlight lang="lua">Controls.TextureQualityPull:RegisterSelectionCallback( OnTextureQualityPull );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1251}}<syntaxhighlight lang="lua">Controls.LeaderPull:RegisterSelectionCallback( OnLeaderPull );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1256}}<syntaxhighlight lang="lua">Controls.BindMousePull:RegisterSelectionCallback( OnBindMousePull );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1263}}<syntaxhighlight lang="lua">Controls.LanguagePull:RegisterSelectionCallback( OnLanguagePull );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1272}}<syntaxhighlight lang="lua">Controls.SpokenLanguagePull:RegisterSelectionCallback( OnSpokenLanguagePull );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ReligionOverview.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/Popups/ReligionOverview.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0468}}<syntaxhighlight lang="lua">automaticPurchasePullDown:RegisterSelectionCallback(function(v1, v2)</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0470}}<syntaxhighlight lang="lua">local player = Players[Game.GetActivePlayer()];</syntaxhighlight>
{{CodeLine5|0471}}<syntaxhighlight lang="lua">Network.SendFaithPurchase(Game.GetActivePlayer(), v1, v2);</syntaxhighlight>
{{CodeLine5|0472}}<syntaxhighlight lang="lua">SetCurrentSelection(v1, v2);</syntaxhighlight>
{{CodeLine5|0473}}<syntaxhighlight lang="lua">end);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ReligionOverview.lua (G&K)}}
:<code>DLC/Expansion/Scenarios/MedievalScenario/ReligionOverview.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0475}}<syntaxhighlight lang="lua">automaticPurchasePullDown:RegisterSelectionCallback(function(v1, v2)</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0477}}<syntaxhighlight lang="lua">local player = Players[Game.GetActivePlayer()];</syntaxhighlight>
{{CodeLine5|0478}}<syntaxhighlight lang="lua">player:SetFaithPurchaseType(v1);</syntaxhighlight>
{{CodeLine5|0479}}<syntaxhighlight lang="lua">player:SetFaithPurchaseIndex(v2);</syntaxhighlight>
{{CodeLine5|0480}}<syntaxhighlight lang="lua">SetCurrentSelection(v1, v2);</syntaxhighlight>
{{CodeLine5|0481}}<syntaxhighlight lang="lua">end);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|StagingRoom.lua}}
:<code>UI/FrontEnd/Multiplayer/StagingRoom.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1055}}<syntaxhighlight lang="lua">pullDown:RegisterSelectionCallback( CivSelected );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1091}}<syntaxhighlight lang="lua">pullDown:RegisterSelectionCallback( InviteSelected );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1120}}<syntaxhighlight lang="lua">pullDown:RegisterSelectionCallback( OnSelectTeam );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1141}}<syntaxhighlight lang="lua">pullDown:RegisterSelectionCallback( OnHandicapTeam );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1163}}<syntaxhighlight lang="lua">pullDown:RegisterSelectionCallback( OnPlayerName );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|SteampunkScenarioLoadScreen.lua (G&K)}}
:<code>DLC/Expansion/Scenarios/SteampunkScenario/SteampunkScenarioLoadScreen.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0219}}<syntaxhighlight lang="lua">pullDown:RegisterSelectionCallback( MapSelected );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|UITestMenu.lua}}
:<code>UI/FrontEnd/UITestMenu.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0131}}<syntaxhighlight lang="lua">Controls.PullDown:RegisterSelectionCallback( OnSelectionChanged );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|UnitFlagManager.lua}}
:<code>UI/InGame/UnitFlagManager.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0101}}<syntaxhighlight lang="lua">o.m_CargoControls.PullDown:RegisterSelectionCallback( UnitFlagClicked );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1038}}<syntaxhighlight lang="lua">cityFlagInstance.PullDown:RegisterSelectionCallback( UnitFlagClicked );</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|RegisterSelectionCallback]]