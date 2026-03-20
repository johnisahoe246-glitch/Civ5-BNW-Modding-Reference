{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This method is declared by '''ControlBase'''.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''void''' UIElement:LocalizeAndSetToolTip<b>(</b>'''string''' description, '''string''' minFaithForProphet = nil, '''string''' threshold, '''string''' moodText, '''string''' spyRank, '''string''' spyName, '''string''' spyRank, '''string''' spyName, '''unknown''' arg8, '''unknown''' arg9, '''string''' arg10, '''unknown''' arg11, '''unknown''' arg12<b>)</b></code>


'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|description:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|minFaithForProphet:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|threshold:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|moodText:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|spyRank:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|spyName:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|spyRank:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|spyName:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|arg8:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|arg9:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|arg10:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|arg11:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|arg12:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Too many occurences. Only 50 out of 142 are listed.''

{{PseudoH4|AdvancedSetup.lua}}
:<code>UI/FrontEnd/GameSetup/AdvancedSetup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0424}}<syntaxhighlight lang="lua">controlTable.Button:LocalizeAndSetToolTip("TXT_KEY_RANDOM_LEADER_HELP");</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0499}}<syntaxhighlight lang="lua">Controls.EraPullDown:GetButton():LocalizeAndSetToolTip(info.Strategy);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0565}}<syntaxhighlight lang="lua">pullDown:GetButton():LocalizeAndSetToolTip(handicap.Help);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0588}}<syntaxhighlight lang="lua">instance.Button:LocalizeAndSetToolTip("TXT_KEY_RANDOM_MAP_SIZE_HELP");</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0605}}<syntaxhighlight lang="lua">pullDown:GetButton():LocalizeAndSetToolTip("TXT_KEY_RANDOM_MAP_SIZE_HELP");</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0637}}<syntaxhighlight lang="lua">Controls.MapSizePullDown:GetButton():LocalizeAndSetToolTip("TXT_KEY_RANDOM_MAP_SIZE_HELP");</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0839}}<syntaxhighlight lang="lua">pullDown:GetButton():LocalizeAndSetToolTip("TXT_KEY_MAP_EARTH_HELP");</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0845}}<syntaxhighlight lang="lua">pullDown:GetButton():LocalizeAndSetToolTip(row.Description or "");</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1107}}<syntaxhighlight lang="lua">Controls.StartButton:LocalizeAndSetToolTip(args.Reason);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CityBannerManager.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/CityBannerManager.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0290}}<syntaxhighlight lang="lua">controls.SpyIcon:LocalizeAndSetToolTip("TXT_KEY_CITY_SPY_OTHER_CIV_TT", strSpyRank, strSpyName, city:GetName(), strSpyRank, strSpyName, strSpyRank, strSpyName);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CityView.lua}}
:<code>UI/InGame/CityView/CityView.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0656}}<syntaxhighlight lang="lua">Controls.ConnectedIcon:LocalizeAndSetToolTip("TXT_KEY_CITY_CONNECTED");</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0673}}<syntaxhighlight lang="lua">Controls.RazingIcon:LocalizeAndSetToolTip("TXT_KEY_CITY_BURNING", pCity:GetRazingTurns());</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0689}}<syntaxhighlight lang="lua">Controls.PuppetIcon:LocalizeAndSetToolTip("TXT_KEY_CITY_PUPPET");</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DiploCorner.lua}}
:<code>UI/InGame/WorldView/DiploCorner.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0064}}<syntaxhighlight lang="lua">controlTable.Button:LocalizeAndSetToolTip( v.tip );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DiploCorner.lua - DLC_01 DLC}}
:<code>DLC/DLC_01/Scenarios/Mongol Scenario/DiploCorner.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0038}}<syntaxhighlight lang="lua">controlTable.Button:LocalizeAndSetToolTip( g_MultiPullInfo[i].tip );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DiploList.lua}}
:<code>UI/InGame/DiploList.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0495}}<syntaxhighlight lang="lua">controlTable.QuestIcon:LocalizeAndSetToolTip( "TXT_KEY_CITY_STATE_QUEST_ROUTE_FORMAL" );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0499}}<syntaxhighlight lang="lua">controlTable.QuestIcon:LocalizeAndSetToolTip( "TXT_KEY_CITY_STATE_QUEST_KILL_CAMP_FORMAL" );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0510}}<syntaxhighlight lang="lua">controlTable.QuestIcon:LocalizeAndSetToolTip( "TXT_KEY_CITY_STATE_QUEST_CONSTRUCT_WONDER_FORMAL", GameInfo.Buildings[iQuestData1].Description );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0526}}<syntaxhighlight lang="lua">controlTable.QuestIcon:LocalizeAndSetToolTip( "TXT_KEY_CITY_STATE_QUEST_FIND_PLAYER_FORMAL", Players[iQuestData1]:GetCivilizationShortDescriptionKey() );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|EconomicOverview.lua}}
:<code>UI/InGame/Popups/EconomicOverview.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0114}}<syntaxhighlight lang="lua">Controls.HappinessButton:LocalizeAndSetToolTip("TXT_KEY_TOP_PANEL_HAPPINESS_OFF_TOOLTIP");</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|EspionageOverview.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/Popups/EspionageOverview.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0371}}<syntaxhighlight lang="lua">Controls.AgentRank:LocalizeAndSetToolTip("TXT_KEY_EO_SPY_RANK_TT", agent.Name, agent.Rank);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0397}}<syntaxhighlight lang="lua">Controls.AgentLocationIcon:LocalizeAndSetToolTip("TXT_KEY_EO_SPY_LOCATION_TT", agent.Rank, agent.Name, city:GetName());</syntaxhighlight>
{{CodeLine5|0398}}<syntaxhighlight lang="lua">Controls.AgentLocation:LocalizeAndSetToolTip("TXT_KEY_EO_SPY_LOCATION_TT", agent.Rank, agent.Name, city:GetName());</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0546}}<syntaxhighlight lang="lua">agentEntry.AgentName:LocalizeAndSetToolTip("TXT_KEY_EO_SPY_NAMEPLATE_TT", v.Rank, v.Name);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0548}}<syntaxhighlight lang="lua">agentEntry.AgentIcon:LocalizeAndSetToolTip("TXT_KEY_EO_SPY_RANK_TT", v.Name, v.Rank);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0564}}<syntaxhighlight lang="lua">agentEntry.AgentLocation:LocalizeAndSetToolTip("TXT_KEY_EO_SPY_NEEDS_ASSIGNMENT_TT");</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0684}}<syntaxhighlight lang="lua">agentEntry.RelocateButton:LocalizeAndSetToolTip("TXT_KEY_EO_SPY_MOVE_TT", v.Rank, v.Name);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0742}}<syntaxhighlight lang="lua">agentEntry.StageCoupButton:LocalizeAndSetToolTip("TXT_KEY_EO_SPY_COUP_DISABLED_NO_ALLY_TT", v.Rank, v.Name, city:GetNameKey(), city:GetNameKey());</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0744}}<syntaxhighlight lang="lua">agentEntry.StageCoupButton:LocalizeAndSetToolTip("TXT_KEY_EO_SPY_COUP_DISABLED_YOU_ALLY_TT", v.Rank, v.Name, city:GetNameKey());</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0760}}<syntaxhighlight lang="lua">agentEntry.ViewCityButton:LocalizeAndSetToolTip("TXT_KEY_EO_CITY_VIEW_DISABLED_YOUR_CITY_TT", city:GetNameKey());</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0767}}<syntaxhighlight lang="lua">agentEntry.ViewCityButton:LocalizeAndSetToolTip("TXT_KEY_EO_CITY_VIEW_DISABLED_NO_CITY_TT");</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1021}}<syntaxhighlight lang="lua">entry.SpyInCityIcon:LocalizeAndSetToolTip("TXT_KEY_SPY_OCCUPYING_CITY", agent.Name);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1288}}<syntaxhighlight lang="lua">entry.DisabledViewCityIcon:LocalizeAndSetToolTip("TXT_KEY_EO_CITY_VIEW_DISABLED_TT", cityInfo.Name);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|GameMenu.lua}}
:<code>UI/InGame/Menus/GameMenu.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0248}}<syntaxhighlight lang="lua">Controls.TypeFrame:LocalizeAndSetToolTip("TXT_KEY_MAP_EARTH_TITLE");</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|LoadMenu.lua}}
:<code>UI/FrontEnd/LoadMenu.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0338}}<syntaxhighlight lang="lua">Controls.MapType:LocalizeAndSetToolTip("TXT_KEY_MAP_EARTH_TITLE");</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|MilitaryOverview.lua}}
:<code>UI/InGame/Popups/MilitaryOverview.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0090}}<syntaxhighlight lang="lua">Controls.GPBox:LocalizeAndSetToolTip( "TXT_KEY_MO_GENERAL_TT", fProgress, fThreshold );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|MPGameOptions.lua}}
:<code>UI/FrontEnd/Multiplayer/GameSetup/MPGameOptions.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0254}}<syntaxhighlight lang="lua">pullDown:GetButton():LocalizeAndSetToolTip(mapScriptFileName);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0461}}<syntaxhighlight lang="lua">Controls.MapSizePullDown:GetButton():LocalizeAndSetToolTip( "TXT_KEY_RANDOM_MAP_SIZE_HELP" );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ProductionPopup.lua}}
:<code>UI/InGame/Popups/ProductionPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0172}}<syntaxhighlight lang="lua">Controls.PurchaseButton:LocalizeAndSetToolTip( "TXT_KEY_CITYVIEW_PURCHASE_TT" );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|StagingRoom.lua}}
:<code>UI/FrontEnd/Multiplayer/StagingRoom.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0356}}<syntaxhighlight lang="lua">Controls.LocalReadyCheck:LocalizeAndSetToolTip( "TXT_KEY_MP_READY_CHECK" );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0690}}<syntaxhighlight lang="lua">Controls.LaunchButton:LocalizeAndSetToolTip( "TXT_KEY_BAD_TEAMS" );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0915}}<syntaxhighlight lang="lua">Controls.MapTypeLabel:LocalizeAndSetToolTip("TXT_KEY_MAP_EARTH_HELP");</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0938}}<syntaxhighlight lang="lua">Controls.MapTypeLabel:LocalizeAndSetToolTip(mapScriptFileName);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0947}}<syntaxhighlight lang="lua">Controls.MapTypeLabel:LocalizeAndSetToolTip( "TXT_KEY_RANDOM_MAP_SCRIPT_HELP" );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0957}}<syntaxhighlight lang="lua">Controls.MapSizeLabel:LocalizeAndSetToolTip( "TXT_KEY_RANDOM_MAP_SIZE_HELP" );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0963}}<syntaxhighlight lang="lua">Controls.GameSpeedLabel:LocalizeAndSetToolTip( info.Help );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TradeLogic.lua}}
:<code>UI/InGame/WorldView/TradeLogic.lua</code>
:{{CodeBegin5}}
{{CodeLine5|2485}}<syntaxhighlight lang="lua">Controls.UsPocketCities:LocalizeAndSetToolTip( "TXT_KEY_DIPLO_TO_TRADE_CITY_NO_TT" );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|UnitFlagManager.lua}}
:<code>UI/InGame/UnitFlagManager.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1080}}<syntaxhighlight lang="lua">cityFlagInstance.PullDown:LocalizeAndSetToolTip( "TXT_KEY_STATIONED_AIRCRAFT", cargoCount );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|VictoryProgress.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/Popups/VictoryProgress.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0822}}<syntaxhighlight lang="lua">controlTable.LastVoteCivIconBG:LocalizeAndSetToolTip("TXT_KEY_VP_DIPLO_LIBERATED_CIV_TT_ALT", strLeaderShortDesc, strLastVoteLeader, strMoodText);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0844}}<syntaxhighlight lang="lua">controlTable.ProjectedVotes:LocalizeAndSetToolTip(strProjVotesTT);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|LocalizeAndSetToolTip]]