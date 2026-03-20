{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Locale}}.<br/>
This is a static method, invoke it with a dot.
}}


Converts a text key into a localized string


=Usage=
<code>'''string''' Locale.Lookup<b>(</b>'''string''' key, ...<b>)</b></code>


'''Returned Value'''
:Returns the textkey if it cannot be found in the dictionary, or a translated string.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|key:
|valign="top"| ''A valid text key.''
|-
|valign="top" style="padding-right:6px;"|...:
|valign="top"| ''none or many arguments that are used when composing the final localized string.''
|}
'''Notes'''
:This method does the exact same thing as Locale.ConvertTextKey.
:This localized string may or may not be in the user's current language.  With support for fall-back language support, the localization system will attempt to search all available languages for the string.


=Examples=
<syntaxhighlight lang="lua" class="civ5-example">
local foo = Locale.ConvertTextKey("TXT_KEY_MAIN_MENU");
print(foo); -- prints "Main Menu" in English</syntaxhighlight>


=Source code samples=
''Too many occurences. Only 50 out of 349 are listed.''

{{PseudoH4|Advisors.lua}}
:<code>UI/InGame/WorldView/Advisors.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0061}}<syntaxhighlight lang="lua">[AdvisorTypes.ADVISOR_ECONOMIC] = Locale.Lookup("TXT_KEY_ADVISOR_ECON_TITLE"),</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ChooseReligionPopup.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/Popups/ChooseReligionPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0307}}<syntaxhighlight lang="lua">local t = Locale.Lookup("TXT_KEY_CHOOSE_RELIGION_ALREADY_FOUNDED", row.Description, takenReligions[row.ID]);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0361}}<syntaxhighlight lang="lua">Controls.FounderBeliefName:SetText(Locale.Lookup(belief.ShortDescription));</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0370}}<syntaxhighlight lang="lua">Controls.BonusBeliefDescription:SetText(Locale.Lookup(belief.Description));</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0565}}<syntaxhighlight lang="lua">local customName = Locale.Lookup(g_CurrentReligionName);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0641}}<syntaxhighlight lang="lua">t = Locale.Lookup("TXT_KEY_CHOOSE_RELIGION_CONFIRM", g_CurrentReligionName);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CityBannerManager.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/CityBannerManager.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0117}}<syntaxhighlight lang="lua">strSpyName = Locale.Lookup(v.Name);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CityStateDiploPopup.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/Popups/CityStateDiploPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0493}}<syntaxhighlight lang="lua">local strProtectTT = Locale.Lookup("TXT_KEY_POP_CSTATE_PLEDGE_TT", 10, 10); --antonjs: todo: xml</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CityStateStatusHelper.lua (G&K)}}
:<code>DLC/Expansion/UI/CityStateStatusHelper.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0395}}<syntaxhighlight lang="lua">return Locale.Lookup("TXT_KEY_CITY_STATE_QUEST_NONE");</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0484}}<syntaxhighlight lang="lua">sToolTipText = sToolTipText .. Locale.Lookup( "TXT_KEY_CITY_STATE_QUEST_CONNECT_RESOURCE_FORMAL", GameInfo.Resources[iQuestData1].Description );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0492}}<syntaxhighlight lang="lua">sToolTipText = sToolTipText .. Locale.Lookup( "TXT_KEY_CITY_STATE_QUEST_FIND_PLAYER_FORMAL", Players[iQuestData1]:GetCivilizationShortDescriptionKey() );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0498}}<syntaxhighlight lang="lua">sToolTipText = sToolTipText .. Locale.Lookup( "TXT_KEY_CITY_STATE_QUEST_PLEDGE_TO_PROTECT_FORMAL", Players[iQuestData1]:GetCivilizationShortDescriptionKey() );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0511}}<syntaxhighlight lang="lua">sToolTipText = sToolTipText .. Locale.Lookup( "TXT_KEY_CITY_STATE_QUEST_CONTEST_FAITH_WINNING_FORMAL", iMajorScore );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CivilopediaScreen.lua (G&K)}}
:<code>DLC/Expansion/UI/Civilopedia/CivilopediaScreen.lua</code>
:{{CodeBegin5}}
{{CodeLine5|2473}}<syntaxhighlight lang="lua">costString = Locale.Lookup("TXT_KEY_PEDIA_A_OR_B", tostring(cost) .. " [ICON_PRODUCTION]", tostring(faithCost) .. " [ICON_PEACE");</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|2949}}<syntaxhighlight lang="lua">table.insert(defenseEntries, Locale.Lookup("TXT_KEY_PEDIA_DEFENSE_HITPOINTS", iExtraHitPoints));</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DiploCorner.lua}}
:<code>UI/InGame/WorldView/DiploCorner.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0039}}<syntaxhighlight lang="lua">{ text = Locale.Lookup("TXT_KEY_VP_TT"),                     call=function() Popup(ButtonPopupTypes.BUTTONPOPUP_VICTORY_INFO); end };</syntaxhighlight>
{{CodeLine5|0040}}<syntaxhighlight lang="lua">{ text = Locale.Lookup("TXT_KEY_DEMOGRAPHICS"),                  call=function() Popup(ButtonPopupTypes.BUTTONPOPUP_DEMOGRAPHICS); end };</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|EspionageOverview.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/Popups/EspionageOverview.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0365}}<syntaxhighlight lang="lua">agent.AgentActivity = Locale.Lookup(agent.State);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0407}}<syntaxhighlight lang="lua">if (agent.AgentActivity == Locale.Lookup("TXT_KEY_SPY_STATE_UNASSIGNED")) then</syntaxhighlight>
{{CodeLine5|0408}}<syntaxhighlight lang="lua">strActivityTT = Locale.Lookup("TXT_KEY_EO_SPY_UNASSIGNED_TT", agent.Rank, agent.Name);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0415}}<syntaxhighlight lang="lua">elseif (agent.AgentActivity == Locale.Lookup("TXT_KEY_SPY_STATE_RIGGING_ELECTION")) then</syntaxhighlight>
{{CodeLine5|0416}}<syntaxhighlight lang="lua">strActivityTT = Locale.Lookup("TXT_KEY_EO_SPY_RIGGING_ELECTIONS_TT", agent.Rank, agent.Name, city:GetName());</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0441}}<syntaxhighlight lang="lua">strActivityTT = strActivityTT .. Locale.Lookup("TXT_KEY_EO_SPY_COUNTER_INTEL_SUM_TT", iFinalChance);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0444}}<syntaxhighlight lang="lua">strActivityTT = Locale.Lookup("TXT_KEY_EO_SPY_BUTTON_DISABLED_SPY_DEAD_TT", agent.Rank, agent.Name);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0523}}<syntaxhighlight lang="lua">v.AgentActivity = Locale.Lookup(v.State);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0604}}<syntaxhighlight lang="lua">elseif (v.AgentActivity == Locale.Lookup("TXT_KEY_SPY_STATE_RIGGING_ELECTION")) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0842}}<syntaxhighlight lang="lua">strTempResult = strTempResult .. Locale.Lookup("TXT_KEY_EO_POTENTIAL_WONDER_MOD_TITLE");</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0883}}<syntaxhighlight lang="lua">strPolicyTT = strPolicyTT .. Locale.Lookup("TXT_KEY_EO_INCREASED_CHANCE_TO_CATCH_SPY_THEM", strLeaderName, policyInfo.Description, iEspionageMod);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1182}}<syntaxhighlight lang="lua">local strCityNameToolTip = Locale.Lookup("TXT_KEY_EO_CITY_NAME_TT", cityInfo.Name, cityInfo.CivilizationNameKey);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1197}}<syntaxhighlight lang="lua">strCityStateTT = strCityStateTT .. Locale.Lookup("TXT_KEY_EO_CITY_STATE_ELECTION", Game.GetTurnsBetweenMinorCivElections(), Game.GetTurnsUntilMinorCivElection());</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1205}}<syntaxhighlight lang="lua">strPotentialToolTip = Locale.Lookup("TXT_KEY_EO_CITY_POTENTIAL_TT", agent.Rank, agent.Name, cityInfo.Potential, cityInfo.Name, cityInfo.Name, cityInfo.BasePotential);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1323}}<syntaxhighlight lang="lua">v.CivilizationName = Locale.Lookup(theirCivilization.ShortDescription);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|GameplayUtils.lua (G&K)}}
:<code>DLC/Expansion/Scenarios/SteampunkScenario/GameplayUtils.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0059}}<syntaxhighlight lang="lua">Name = Locale.Lookup("TXT_KEY_STEAMPUNK_SCENARIO_VICTORY_CATEGORY_INDUSTRY"),</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0068}}<syntaxhighlight lang="lua">Title = Locale.Lookup("TXT_KEY_STEAMPUNK_SCENARIO_VICTORY_CATEGORY_CULTURE_TITLE"),</syntaxhighlight>
{{CodeLine5|0069}}<syntaxhighlight lang="lua">Help = Locale.Lookup("TXT_KEY_STEAMPUNK_SCENARIO_VICTORY_CATEGORY_CULTURE_HELP"),</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|InstalledPanel.lua}}
:<code>UI/FrontEnd/Modding/InstalledPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0655}}<syntaxhighlight lang="lua">dlcTitle = Locale.Lookup("TXT_KEY_" .. packageID .. "_DESCRIPTION");</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0745}}<syntaxhighlight lang="lua">LuaEvents.ModBrowserSetDeleteButtonState(true, true, Locale.Lookup("TXT_KEY_MODDING_DELETEMOD"));</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|LoadMenu.lua}}
:<code>UI/FrontEnd/LoadMenu.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0351}}<syntaxhighlight lang="lua">name = Locale.Lookup(name);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|Lobby.lua}}
:<code>UI/FrontEnd/Multiplayer/Lobby.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0357}}<syntaxhighlight lang="lua">sortData.ServerHasDlc = Locale.Lookup("TXT_KEY_MULTIPLAYER_LOBBY_NO");</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0403}}<syntaxhighlight lang="lua">local lines = {Locale.Lookup(headerString)};</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|OptionsMenu.lua (G&K)}}
:<code>DLC/Expansion/UI/Options/OptionsMenu.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1355}}<syntaxhighlight lang="lua">table.insert(TutorialLevels, Locale.Lookup("TXT_KEY_OPSCREEN_TUTORIAL_MEDIUM"));</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ReligionOverview.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/Popups/ReligionOverview.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0116}}<syntaxhighlight lang="lua">text = Locale.Lookup("TXT_KEY_RO_STATUS_CAN_CREATE_PANTHEON");</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0131}}<syntaxhighlight lang="lua">return Locale.Lookup("TXT_KEY_RO_BELIEF_TYPE_PANTHEON");</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0428}}<syntaxhighlight lang="lua">local gpString = string.format("%s (%i [ICON_PEACE])", Locale.Lookup(GameInfo.Buildings[v2].Description), faithCost);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ReplayViewer.lua}}
:<code>UI/InGame/Popups/ReplayViewer.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0758}}<syntaxhighlight lang="lua">Tooltip = Locale.Lookup("TXT_KEY_REPLAY_VIEWER_MAP_TT"),</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|SaveMenu.lua}}
:<code>UI/InGame/Menus/SaveMenu.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0538}}<syntaxhighlight lang="lua">title = Locale.Lookup("TXT_KEY_RANDOM_LEADER_CIV", leaderDescription, civName );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TechButtonInclude.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/TechTree/TechButtonInclude.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0463}}<syntaxhighlight lang="lua">techPediaSearchStrings[tostring(thisButton)] =  Locale.Lookup(thisResourceInfo.Description);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|VictoryStatus.lua (G&K)}}
:<code>DLC/Expansion/Scenarios/SteampunkScenario/VictoryStatus.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0117}}<syntaxhighlight lang="lua">local sCivDesc = Locale.Lookup(Players[iPlayer]:GetCivilizationShortDescriptionKey());</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0153}}<syntaxhighlight lang="lua">s = s .. "[COLOR_WARNING_TEXT]" .. Locale.Lookup("TXT_KEY_STEAMPUNK_SCENARIO_VICTORY_CATEGORY_TECH_UNLOCK", GameInfo.Technologies[iUnlockTech].Description) .. "[ENDCOLOR]";</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0169}}<syntaxhighlight lang="lua">s = s .. Locale.Lookup("TXT_KEY_STEAMPUNK_SCENARIO_VICTORY_CATEGORY_MILITARY_TT", GameInfo.UnitClasses[iLandshipClass].Description, GameInfo.UnitClasses[iAirshipClass].Description);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|Lookup]]