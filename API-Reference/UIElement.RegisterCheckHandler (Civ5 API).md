{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of ControlBase.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''void''' UIElement:RegisterCheckHandler<b>(</b>('''void''' func<b>(</b>'''bool''' bIsChecked<b>)</b>) OnPolicyInfo<b>)</b></code>


'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|OnPolicyInfo:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Too many occurences. Only 50 out of 69 are listed.''

{{PseudoH4|AdvancedSetup.lua}}
:<code>UI/FrontEnd/GameSetup/AdvancedSetup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0228}}<syntaxhighlight lang="lua">gameOption.GameOptionRoot:RegisterCheckHandler( function(bCheck)</syntaxhighlight>
{{CodeLine5|0229}}<syntaxhighlight lang="lua">PreGame.SetGameOption(option.Type, bCheck);</syntaxhighlight>
{{CodeLine5|0230}}<syntaxhighlight lang="lua">end);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0232}}<syntaxhighlight lang="lua">gameOption.GameOptionRoot:RegisterCheckHandler( function(bCheck)</syntaxhighlight>
{{CodeLine5|0233}}<syntaxhighlight lang="lua">PreGame.SetMapOption(option.ID, bCheck);</syntaxhighlight>
{{CodeLine5|0234}}<syntaxhighlight lang="lua">end);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1062}}<syntaxhighlight lang="lua">victoryCondition.GameOptionRoot:RegisterCheckHandler( function(bCheck)</syntaxhighlight>
{{CodeLine5|1063}}<syntaxhighlight lang="lua">PreGame.SetVictory(row.ID, bCheck);</syntaxhighlight>
{{CodeLine5|1064}}<syntaxhighlight lang="lua">end);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CityView.lua}}
:<code>UI/InGame/CityView/CityView.lua</code>
:{{CodeBegin5}}
{{CodeLine5|2258}}<syntaxhighlight lang="lua">Controls.HideQueueButton:RegisterCheckHandler( OnHideQueue );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|InstalledPanel.lua}}
:<code>UI/FrontEnd/Modding/InstalledPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0863}}<syntaxhighlight lang="lua">Controls.ShowDLCMods:RegisterCheckHandler( function(bCheck)</syntaxhighlight>
{{CodeLine5|0864}}<syntaxhighlight lang="lua">if(bCheck) then</syntaxhighlight>
{{CodeLine5|0865}}<syntaxhighlight lang="lua">Modding.SetSystemProperty("ShowDLCMods", "1");</syntaxhighlight>
{{CodeLine5|0866}}<syntaxhighlight lang="lua">else</syntaxhighlight>
{{CodeLine5|0867}}<syntaxhighlight lang="lua">Modding.SetSystemProperty("ShowDLCMods", "0");</syntaxhighlight>
{{CodeLine5|0868}}<syntaxhighlight lang="lua">end</syntaxhighlight>
{{CodeLine5|0869}}<syntaxhighlight lang="lua">end);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|LoadMenu.lua}}
:<code>UI/FrontEnd/LoadMenu.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0082}}<syntaxhighlight lang="lua">Controls.AutoCheck:RegisterCheckHandler( function(checked)</syntaxhighlight>
{{CodeLine5|0083}}<syntaxhighlight lang="lua">g_ShowAutoSaves = checked;</syntaxhighlight>
{{CodeLine5|0084}}<syntaxhighlight lang="lua">if(g_ShowAutoSaves) then</syntaxhighlight>
{{CodeLine5|0085}}<syntaxhighlight lang="lua">g_ShowCloudSaves = false;</syntaxhighlight>
{{CodeLine5|0086}}<syntaxhighlight lang="lua">end</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0088}}<syntaxhighlight lang="lua">UpdateControlStates();</syntaxhighlight>
{{CodeLine5|0089}}<syntaxhighlight lang="lua">SetupFileButtonList();</syntaxhighlight>
{{CodeLine5|0090}}<syntaxhighlight lang="lua">end);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0093}}<syntaxhighlight lang="lua">Controls.CloudCheck:RegisterCheckHandler( function(checked)</syntaxhighlight>
{{CodeLine5|0094}}<syntaxhighlight lang="lua">g_ShowCloudSaves = checked;</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0096}}<syntaxhighlight lang="lua">if(g_ShowCloudSaves) then</syntaxhighlight>
{{CodeLine5|0097}}<syntaxhighlight lang="lua">Controls.SortByPullDown:SetHide(true);</syntaxhighlight>
{{CodeLine5|0098}}<syntaxhighlight lang="lua">g_ShowAutoSaves = false;</syntaxhighlight>
{{CodeLine5|0099}}<syntaxhighlight lang="lua">else</syntaxhighlight>
{{CodeLine5|0100}}<syntaxhighlight lang="lua">Controls.SortByPullDown:SetHide(false);</syntaxhighlight>
{{CodeLine5|0101}}<syntaxhighlight lang="lua">end</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0103}}<syntaxhighlight lang="lua">UpdateControlStates();</syntaxhighlight>
{{CodeLine5|0104}}<syntaxhighlight lang="lua">SetupFileButtonList();</syntaxhighlight>
{{CodeLine5|0105}}<syntaxhighlight lang="lua">end);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|MiniMapPanel.lua}}
:<code>UI/InGame/WorldView/MiniMapPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0296}}<syntaxhighlight lang="lua">Controls.ShowFeatures:RegisterCheckHandler( OnShowFeaturesChecked );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0306}}<syntaxhighlight lang="lua">Controls.ShowFogOfWar:RegisterCheckHandler( OnShowFOWChecked );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0321}}<syntaxhighlight lang="lua">Controls.ShowGrid:RegisterCheckHandler( OnShowGridChecked );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0358}}<syntaxhighlight lang="lua">Controls.ShowYield:RegisterCheckHandler( OnYieldChecked );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0372}}<syntaxhighlight lang="lua">Controls.ShowResources:RegisterCheckHandler( OnResourcesChecked );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0413}}<syntaxhighlight lang="lua">Controls.HideRecommendation:RegisterCheckHandler( OnRecommendationChecked );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|MPGameOptions.lua}}
:<code>UI/FrontEnd/Multiplayer/GameSetup/MPGameOptions.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0885}}<syntaxhighlight lang="lua">victoryCondition.GameOptionRoot:RegisterCheckHandler( function(bCheck)</syntaxhighlight>
{{CodeLine5|0886}}<syntaxhighlight lang="lua">PreGame.SetVictory(row.ID, bCheck);</syntaxhighlight>
{{CodeLine5|0887}}<syntaxhighlight lang="lua">SendGameOptionChanged();</syntaxhighlight>
{{CodeLine5|0888}}<syntaxhighlight lang="lua">end);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0959}}<syntaxhighlight lang="lua">gameOption.GameOptionRoot:RegisterCheckHandler( function(bCheck)</syntaxhighlight>
{{CodeLine5|0960}}<syntaxhighlight lang="lua">PreGame.SetGameOption(option.Type, bCheck);</syntaxhighlight>
{{CodeLine5|0961}}<syntaxhighlight lang="lua">SendGameOptionChanged();</syntaxhighlight>
{{CodeLine5|0962}}<syntaxhighlight lang="lua">end);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0964}}<syntaxhighlight lang="lua">gameOption.GameOptionRoot:RegisterCheckHandler( function(bCheck)</syntaxhighlight>
{{CodeLine5|0965}}<syntaxhighlight lang="lua">PreGame.SetMapOption(option.ID, bCheck);</syntaxhighlight>
{{CodeLine5|0966}}<syntaxhighlight lang="lua">SendGameOptionChanged();</syntaxhighlight>
{{CodeLine5|0967}}<syntaxhighlight lang="lua">end);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0995}}<syntaxhighlight lang="lua">dlcEntries.GameOptionRoot:RegisterCheckHandler( function(bCheck)</syntaxhighlight>
{{CodeLine5|0996}}<syntaxhighlight lang="lua">PreGame.SetDLCAllowed(row.PackageID, bCheck);</syntaxhighlight>
{{CodeLine5|0997}}<syntaxhighlight lang="lua">SendGameOptionChanged();</syntaxhighlight>
{{CodeLine5|0998}}<syntaxhighlight lang="lua">end</syntaxhighlight>
{{CodeLine5|0999}}<syntaxhighlight lang="lua">);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|OptionsMenu.lua}}
:<code>UI/Options/OptionsMenu.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0777}}<syntaxhighlight lang="lua">Controls.AutoWorkersDontReplaceCB:RegisterCheckHandler( OnAutoWorkersDontReplaceCheckbox );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0784}}<syntaxhighlight lang="lua">Controls.AutoWorkersDontRemoveFeaturesCB:RegisterCheckHandler( OnAutoWorkersDontRemoveFeaturesCheckbox );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0791}}<syntaxhighlight lang="lua">Controls.NoRewardPopupsCheckbox:RegisterCheckHandler( OnNoRewardPopupsCheckbox );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0798}}<syntaxhighlight lang="lua">Controls.NoTileRecommendationsCheckbox:RegisterCheckHandler( OnNoTileRecommendationsCheckbox );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0805}}<syntaxhighlight lang="lua">Controls.CivilianYieldsCheckbox:RegisterCheckHandler( OnCivilianYieldsCheckbox );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0812}}<syntaxhighlight lang="lua">Controls.NoBasicHelpCheckbox:RegisterCheckHandler( OnNoBasicHelpCheckbox );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0835}}<syntaxhighlight lang="lua">Controls.ZoomCheck:RegisterCheckHandler( OnZoomCheck );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0850}}<syntaxhighlight lang="lua">Controls.SinglePlayerAutoEndTurnCheckBox:RegisterCheckHandler(OnSinglePlayerAutoEndTurnCheck);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0857}}<syntaxhighlight lang="lua">Controls.MultiplayerAutoEndTurnCheckbox:RegisterCheckHandler(OnMultiplayerAutoEndTurnCheck);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0871}}<syntaxhighlight lang="lua">Controls.SPQuickCombatCheckBox:RegisterCheckHandler(OnSinglePlayerQuickCombatCheck);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0885}}<syntaxhighlight lang="lua">Controls.SPQuickMovementCheckBox:RegisterCheckHandler(OnSinglePlayerQuickMovementCheck);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0899}}<syntaxhighlight lang="lua">Controls.MPQuickCombatCheckbox:RegisterCheckHandler(OnMultiplayerQuickCombatCheck);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0913}}<syntaxhighlight lang="lua">Controls.MPQuickMovementCheckbox:RegisterCheckHandler(OnMultiplayerQuickMovementCheck);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0930}}<syntaxhighlight lang="lua">Controls.AutoUIAssetsCheck:RegisterCheckHandler( OnAutoUI );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0938}}<syntaxhighlight lang="lua">Controls.SmallUIAssetsCheck:RegisterCheckHandler( OnSmallUI );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0978}}<syntaxhighlight lang="lua">Controls.AutoUnitCycleCheck:RegisterCheckHandler( OnAutoUnitCycleCheck );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0986}}<syntaxhighlight lang="lua">Controls.ScoreListCheck:RegisterCheckHandler( OnScoreListCheck );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0993}}<syntaxhighlight lang="lua">Controls.SkipIntroVideoCheck:RegisterCheckHandler( OnSkipIntroVideo );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1016}}<syntaxhighlight lang="lua">Controls.HDStratCheck:RegisterCheckHandler( OnHDStrategicView );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1027}}<syntaxhighlight lang="lua">Controls.FullscreenCheck:RegisterCheckHandler( OnFullscreen );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1035}}<syntaxhighlight lang="lua">Controls.VSyncCheck:RegisterCheckHandler( OnVSync );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ReplayViewer.lua}}
:<code>UI/InGame/Popups/ReplayViewer.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0731}}<syntaxhighlight lang="lua">graphLegendInstance.ShowHide:RegisterCheckHandler( function(bCheck)</syntaxhighlight>
{{CodeLine5|0732}}<syntaxhighlight lang="lua">local segments = panel.SegmentsByPlayer[i];</syntaxhighlight>
{{CodeLine5|0733}}<syntaxhighlight lang="lua">if(segments) then</syntaxhighlight>
{{CodeLine5|0734}}<syntaxhighlight lang="lua">for i,v in ipairs(segments) do</syntaxhighlight>
{{CodeLine5|0735}}<syntaxhighlight lang="lua">   v.LineSegment:SetHide(not bCheck);</syntaxhighlight>
{{CodeLine5|0736}}<syntaxhighlight lang="lua">   end</syntaxhighlight>
{{CodeLine5|0737}}<syntaxhighlight lang="lua">   end</syntaxhighlight>
{{CodeLine5|0738}}<syntaxhighlight lang="lua">   end);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|SaveMenu.lua}}
:<code>UI/InGame/Menus/SaveMenu.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0151}}<syntaxhighlight lang="lua">Controls.CloudCheck:RegisterCheckHandler(function(checked)</syntaxhighlight>
{{CodeLine5|0152}}<syntaxhighlight lang="lua">Controls.NameBox:ClearString();</syntaxhighlight>
{{CodeLine5|0153}}<syntaxhighlight lang="lua">SetSelected( nil );</syntaxhighlight>
{{CodeLine5|0154}}<syntaxhighlight lang="lua">SetupFileButtonList();</syntaxhighlight>
{{CodeLine5|0155}}<syntaxhighlight lang="lua">end);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|SocialPolicyPopup.lua}}
:<code>UI/InGame/Popups/SocialPolicyPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0555}}<syntaxhighlight lang="lua">Controls.PolicyInfo:RegisterCheckHandler( OnPolicyInfo );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|StagingRoom.lua}}
:<code>UI/FrontEnd/Multiplayer/StagingRoom.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0197}}<syntaxhighlight lang="lua">Controls.LocalReadyCheck:RegisterCheckHandler( OnReadyCheck );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1272}}<syntaxhighlight lang="lua">instance.LockCheck:RegisterCheckHandler( OnLock );</syntaxhighlight>
{{CodeLine5|1273}}<syntaxhighlight lang="lua">instance.EnableCheck:RegisterCheckHandler( OnEnable );</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|RegisterCheckHandler]]