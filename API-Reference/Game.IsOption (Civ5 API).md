{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Game}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''int''' Game.IsOption<b>(</b>'''string''' index<b>)</b></code>


'''Returned Value'''
:No description available.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|index:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|ActionInfoPanel.lua}}
:<code>UI/InGame/WorldView/ActionInfoPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0219}}<syntaxhighlight lang="lua">return Game.IsOption(GameOptionTypes.GAMEOPTION_END_TURN_TIMER_ENABLED);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0288}}<syntaxhighlight lang="lua">if (Game.IsOption(GameOptionTypes.GAMEOPTION_POLICY_SAVING)) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CityBannerManager.lua}}
:<code>UI/InGame/CityBannerManager.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0463}}<syntaxhighlight lang="lua">if (Game.IsOption( GameOptionTypes.GAMEOPTION_ALWAYS_WAR )) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CityBannerManager.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/CityBannerManager.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0186}}<syntaxhighlight lang="lua">elseif (Game.IsOption( GameOptionTypes.GAMEOPTION_ALWAYS_WAR )) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CityStateDiploPopup.lua}}
:<code>UI/InGame/Popups/CityStateDiploPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0498}}<syntaxhighlight lang="lua">if (Game.IsOption(GameOptionTypes.GAMEOPTION_ALWAYS_PEACE)) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0501}}<syntaxhighlight lang="lua">if (Game.IsOption(GameOptionTypes.GAMEOPTION_NO_CHANGING_WAR_PEACE)) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CivilopediaScreen.lua (G&K)}}
:<code>DLC/Expansion/UI/Civilopedia/CivilopediaScreen.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0456}}<syntaxhighlight lang="lua">if(Game == nil or not Game.IsOption(GameOptionTypes.GAMEOPTION_NO_RELIGION)) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|2461}}<syntaxhighlight lang="lua">if(Game and not Game.IsOption(GameOptionTypes.GAMEOPTION_NO_RELIGION)) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|2866}}<syntaxhighlight lang="lua">if(Game and Game.IsOption(GameOptionTypes.GAMEOPTION_NO_RELIGION)) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DiploList.lua}}
:<code>UI/InGame/DiploList.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0296}}<syntaxhighlight lang="lua">not Game.IsOption(GameOptionTypes.GAMEOPTION_NO_SCIENCE)) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|EconomicOverview.lua}}
:<code>UI/InGame/Popups/EconomicOverview.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0112}}<syntaxhighlight lang="lua">if (Game.IsOption(GameOptionTypes.GAMEOPTION_NO_HAPPINESS)) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|EspionageOverview.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/Popups/EspionageOverview.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0208}}<syntaxhighlight lang="lua">if (not Game.IsOption("GAMEOPTION_NO_ESPIONAGE")) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|InfoTooltipInclude.lua}}
:<code>UI/InGame/InfoTooltipInclude.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0440}}<syntaxhighlight lang="lua">if (Game.IsOption(GameOptionTypes.GAMEOPTION_NO_SCIENCE)) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0745}}<syntaxhighlight lang="lua">if (Game.IsOption(GameOptionTypes.GAMEOPTION_ALWAYS_WAR)) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|InfoTooltipInclude.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/InfoTooltipInclude.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0592}}<syntaxhighlight lang="lua">if (Game.IsOption(GameOptionTypes.GAMEOPTION_NO_RELIGION)) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|MapGenerator.lua (G&K)}}
:<code>DLC/Expansion/Gameplay/Lua/MapGenerator.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0682}}<syntaxhighlight lang="lua">if (Game.IsOption(GameOptionTypes.GAMEOPTION_NO_GOODY_HUTS)) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ReligionOverview.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/Popups/ReligionOverview.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0150}}<syntaxhighlight lang="lua">if(not Game.IsOption(GameOptionTypes.GAMEOPTION_NO_RELIGION)) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|SaveMenu.lua}}
:<code>UI/InGame/Menus/SaveMenu.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0619}}<syntaxhighlight lang="lua">Game.IsOption( GameOptionTypes.GAMEOPTION_LOCK_MODS ) or</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|SocialPolicyPopup.lua}}
:<code>UI/InGame/Popups/SocialPolicyPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0608}}<syntaxhighlight lang="lua">local bDisablePolicies = Game.IsOption(GameOptionTypes.GAMEOPTION_NO_POLICIES);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TechPopup.lua}}
:<code>UI/InGame/TechPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0095}}<syntaxhighlight lang="lua">if (not Game.IsOption(GameOptionTypes.GAMEOPTION_NO_SCIENCE)) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TechTree.lua}}
:<code>UI/InGame/TechTree/TechTree.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0452}}<syntaxhighlight lang="lua">local scienceDisabled = Game.IsOption(GameOptionTypes.GAMEOPTION_NO_SCIENCE);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TopPanel.lua}}
:<code>UI/InGame/TopPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0131}}<syntaxhighlight lang="lua">if (Game.IsOption(GameOptionTypes.GAMEOPTION_NO_POLICIES)) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TradeLogic.lua}}
:<code>UI/InGame/WorldView/TradeLogic.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0011}}<syntaxhighlight lang="lua">local g_bAlwaysWar = Game.IsOption( GameOptionTypes.GAMEOPTION_ALWAYS_WAR );</syntaxhighlight>
{{CodeLine5|0012}}<syntaxhighlight lang="lua">local g_bAlwaysPeace = Game.IsOption( GameOptionTypes.GAMEOPTION_ALWAYS_PEACE );</syntaxhighlight>
{{CodeLine5|0013}}<syntaxhighlight lang="lua">local g_bNoChangeWar = Game.IsOption( GameOptionTypes.GAMEOPTION_NO_CHANGING_WAR_PEACE );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|2749}}<syntaxhighlight lang="lua">if( Game.IsOption( GameOptionTypes.GAMEOPTION_ALWAYS_WAR ) or</syntaxhighlight>
{{CodeLine5|2750}}<syntaxhighlight lang="lua">Game.IsOption( GameOptionTypes.GAMEOPTION_ALWAYS_PEACE ) or</syntaxhighlight>
{{CodeLine5|2751}}<syntaxhighlight lang="lua">Game.IsOption( GameOptionTypes.GAMEOPTION_NO_CHANGING_WAR_PEACE ) ) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TutorialChecks.lua}}
:<code>Tutorial/TutorialChecks.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0970}}<syntaxhighlight lang="lua">if (Game.IsOption( GameOptionTypes.GAMEOPTION_ONE_CITY_CHALLENGE )) then</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|IsOption]]
[[Category:Civ5 Game Settings API|IsOption]]