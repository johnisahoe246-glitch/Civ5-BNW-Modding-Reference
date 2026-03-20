{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of ControlBase.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>{{Type5|Button}} UIElement:GetButton<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
''Too many occurences. Only 50 out of 180 are listed.''

{{PseudoH4|AdvancedSetup.lua}}
:<code>UI/FrontEnd/GameSetup/AdvancedSetup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0099}}<syntaxhighlight lang="lua">local dropDownButton = gameOption.OptionDropDown:GetButton();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0491}}<syntaxhighlight lang="lua">pullDown:GetButton():LocalizeAndSetText(era.Description);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0531}}<syntaxhighlight lang="lua">pullDown:GetButton():SetToolTipString( Locale.ConvertTextKey( gameSpeed.Help ) );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0539}}<syntaxhighlight lang="lua">Controls.GameSpeedPullDown:GetButton():SetToolTipString( Locale.ConvertTextKey( info.Help ) );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0564}}<syntaxhighlight lang="lua">pullDown:GetButton():LocalizeAndSetText(handicap.Description);</syntaxhighlight>
{{CodeLine5|0565}}<syntaxhighlight lang="lua">pullDown:GetButton():LocalizeAndSetToolTip(handicap.Help);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0574}}<syntaxhighlight lang="lua">Controls.HandicapPullDown:GetButton():LocalizeAndSetToolTip(info.Help);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0605}}<syntaxhighlight lang="lua">pullDown:GetButton():LocalizeAndSetToolTip("TXT_KEY_RANDOM_MAP_SIZE_HELP");</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0839}}<syntaxhighlight lang="lua">pullDown:GetButton():LocalizeAndSetToolTip("TXT_KEY_MAP_EARTH_HELP");</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0845}}<syntaxhighlight lang="lua">pullDown:GetButton():LocalizeAndSetToolTip(row.Description or "");</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0872}}<syntaxhighlight lang="lua">pullDown:GetButton():LocalizeAndSetText(name);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0887}}<syntaxhighlight lang="lua">pullDown:GetButton():LocalizeAndSetText("TXT_KEY_RANDOM_MAP_SCRIPT");</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1139}}<syntaxhighlight lang="lua">Controls.CivPulldown:GetButton():LocalizeAndSetText("TXT_KEY_RANDOM_LEADER_CIV", Locale.ConvertTextKey(leaderDescription), Locale.ConvertTextKey(civ.ShortDescription));</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DiploCorner.lua}}
:<code>UI/InGame/WorldView/DiploCorner.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0297}}<syntaxhighlight lang="lua">Controls.ChatPull:GetButton():SetText( Controls.LengthTest:GetText() );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|MiniMapPanel.lua}}
:<code>UI/InGame/WorldView/MiniMapPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0204}}<syntaxhighlight lang="lua">Controls.OverlayDropDown:GetButton():SetText(Locale.ConvertTextKey( g_Overlays[1] ));</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0270}}<syntaxhighlight lang="lua">Controls.IconDropDown:GetButton():SetText(Locale.ConvertTextKey( g_IconModes[1] ));</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|MPGameOptions.lua}}
:<code>UI/FrontEnd/Multiplayer/GameSetup/MPGameOptions.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0180}}<syntaxhighlight lang="lua">Controls.MapSizePullDown:GetButton():SetDisabled(true);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0253}}<syntaxhighlight lang="lua">pullDown:GetButton():SetText("[COLOR_RED]" .. fileTitle .. "[ENDCOLOR]");</syntaxhighlight>
{{CodeLine5|0254}}<syntaxhighlight lang="lua">pullDown:GetButton():LocalizeAndSetToolTip(mapScriptFileName);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0304}}<syntaxhighlight lang="lua">Controls.MapSizePullDown:GetButton():SetDisabled( not bCanEdit );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0311}}<syntaxhighlight lang="lua">Controls.MapSizePullDown:GetButton():LocalizeAndSetText( info.Description );</syntaxhighlight>
{{CodeLine5|0312}}<syntaxhighlight lang="lua">Controls.MapSizePullDown:GetButton():LocalizeAndSetToolTip( info.Help );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0334}}<syntaxhighlight lang="lua">Controls.GameSpeedPullDown:GetButton():LocalizeAndSetToolTip( info.Help );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0339}}<syntaxhighlight lang="lua">Controls.EraPull:GetButton():LocalizeAndSetText( info.Description );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0427}}<syntaxhighlight lang="lua">Controls.GameSpeedPullDown:GetButton():LocalizeAndSetText(GameInfo.GameSpeeds[id].Description);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0468}}<syntaxhighlight lang="lua">Controls.MapSizePullDown:GetButton():LocalizeAndSetText(GameInfo.Worlds[id].Description);</syntaxhighlight>
{{CodeLine5|0469}}<syntaxhighlight lang="lua">Controls.MapSizePullDown:GetButton():LocalizeAndSetToolTip(GameInfo.Worlds[id].Help);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|OptionsMenu.lua}}
:<code>UI/Options/OptionsMenu.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0522}}<syntaxhighlight lang="lua">Controls.LanguagePull:GetButton():SetText(Locale.GetCurrentLanguage().DisplayName);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0675}}<syntaxhighlight lang="lua">Controls.BindMousePull:GetButton():SetText( m_BindMouseText[ OptionsManager.GetBindMouseMode_Cached() ] );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0681}}<syntaxhighlight lang="lua">Controls.TutorialPull:GetButton():SetText( m_TutorialLevelText[ iTutorialLevel ] );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0684}}<syntaxhighlight lang="lua">Controls.SpokenLanguagePull:GetButton():SetText(Locale.GetCurrentSpokenLanguage().DisplayName); --TODO: make this work like its friends -KS</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0731}}<syntaxhighlight lang="lua">Controls.FSResolutionPull:GetButton():SetText( kResInfo.Width .. "x" .. kResInfo.Height .. "   " .. kResInfo.Refresh .. " Hz" );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0735}}<syntaxhighlight lang="lua">Controls.WResolutionPull:GetButton():SetText( x .. "x" .. y );</syntaxhighlight>
{{CodeLine5|0736}}<syntaxhighlight lang="lua">Controls.MSAAPull:GetButton():SetText( m_MSAAText[ m_MSAAInvMap[OptionsManager.GetAASamples_Cached()] ] );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0741}}<syntaxhighlight lang="lua">Controls.LeaderPull:GetButton():SetText( m_LeaderText[ OptionsManager.GetLeaderQuality_Cached() ] );</syntaxhighlight>
{{CodeLine5|0742}}<syntaxhighlight lang="lua">Controls.OverlayPull:GetButton():SetText( m_OverlayText[ OptionsManager.GetOverlayLevel_Cached() ] );</syntaxhighlight>
{{CodeLine5|0743}}<syntaxhighlight lang="lua">Controls.ShadowPull:GetButton():SetText( m_ShadowText[ OptionsManager.GetShadowLevel_Cached() ] );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0745}}<syntaxhighlight lang="lua">Controls.TerrainDetailPull:GetButton():SetText( m_TerrainDetailText[ OptionsManager.GetTerrainDetailLevel_Cached() ] );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1064}}<syntaxhighlight lang="lua">Controls.FOWPull:GetButton():SetText( m_FOWText[ level ] );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1080}}<syntaxhighlight lang="lua">Controls.TerrainTessPull:GetButton():SetText( m_TerrainTessText[ level ] );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1096}}<syntaxhighlight lang="lua">Controls.WaterPull:GetButton():SetText( m_WaterText[ level ] );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1104}}<syntaxhighlight lang="lua">Controls.TextureQualityPull:GetButton():SetText( m_TextureQualityText[ level ] );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1131}}<syntaxhighlight lang="lua">Controls.WResolutionPull:GetButton():SetText( kResInfo.Width .. "x" .. kResInfo.Height );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ReligionOverview.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/Popups/ReligionOverview.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0419}}<syntaxhighlight lang="lua">automaticPurchasePullDown:GetButton():LocalizeAndSetText("TXT_KEY_RO_AUTO_FAITH_PROMPT");</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0425}}<syntaxhighlight lang="lua">automaticPurchasePullDown:GetButton():LocalizeAndSetText("TXT_KEY_RO_AUTO_FAITH_PURCHASE_GREAT_PERSON", gpString);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ReplayViewer.lua}}
:<code>UI/InGame/Popups/ReplayViewer.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1097}}<syntaxhighlight lang="lua">local replayInfoPulldownButton = Controls.ReplayInfoPulldown:GetButton();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|StagingRoom.lua}}
:<code>UI/FrontEnd/Multiplayer/StagingRoom.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0157}}<syntaxhighlight lang="lua">slotInstance.InvitePulldown:GetButton():LocalizeAndSetText( "TXT_KEY_AI_NICKNAME" );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0387}}<syntaxhighlight lang="lua">slotInstance.InvitePulldown:GetButton():SetText( playerName );</syntaxhighlight>
{{CodeLine5|0388}}<syntaxhighlight lang="lua">slotInstance.PlayerNamePulldown:GetButton():SetText( playerName );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|UITestMenu.lua}}
:<code>UI/FrontEnd/UITestMenu.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0129}}<syntaxhighlight lang="lua">Controls.PullDown:GetButton():SetText( one );</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetButton]]