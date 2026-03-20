{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Team}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>{{Type5|TeamTechs}} Team:GetTeamTechs<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|CivilopediaScreen.lua}}
:<code>UI/Civilopedia/CivilopediaScreen.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1997}}<syntaxhighlight lang="lua">local pTeamTechs = pTeam:GetTeamTechs();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|Demographics.lua}}
:<code>UI/InGame/Popups/Demographics.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0384}}<syntaxhighlight lang="lua">local pTeamTechs = Teams[ Players[ iPlayer ]:GetTeam() ]:GetTeamTechs();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|PlotMouseoverInclude.lua}}
:<code>UI/InGame/PlotMouseoverInclude.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0184}}<syntaxhighlight lang="lua">if (iTechCityTrade ~= -1 and not pTeam:GetTeamTechs():HasTech(iTechCityTrade)) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TechHelpInclude.lua}}
:<code>UI/InGame/TechTree/TechHelpInclude.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0009}}<syntaxhighlight lang="lua">local pTeamTechs = pActiveTeam:GetTeamTechs();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TechPopup.lua}}
:<code>UI/InGame/TechPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0172}}<syntaxhighlight lang="lua">local teamTechs = activeTeam:GetTeamTechs();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0288}}<syntaxhighlight lang="lua">if activeTeam:GetTeamTechs():HasTech(tech.ID) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TechTree.lua}}
:<code>UI/InGame/TechTree/TechTree.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0588}}<syntaxhighlight lang="lua">if activeTeam:GetTeamTechs():HasTech(techID) then -- the player (or more accurately his team) has already researched this one</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TopPanel.lua}}
:<code>UI/InGame/TopPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0165}}<syntaxhighlight lang="lua">if (pTeam:GetTeamTechs():HasTech(GameInfoTypes[pResource.TechReveal])) then</syntaxhighlight>
{{CodeLine5|0166}}<syntaxhighlight lang="lua">if (pTeam:GetTeamTechs():HasTech(GameInfoTypes[pResource.TechCityTrade])) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TradeLogic.lua}}
:<code>UI/InGame/WorldView/TradeLogic.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1173}}<syntaxhighlight lang="lua">local pUsTeamTechs = g_pUsTeam:GetTeamTechs();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1175}}<syntaxhighlight lang="lua">local pTheirTeamTechs = pTheirTeam:GetTeamTechs();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TurnsRemaining.lua - DLC_02 DLC}}
:<code>DLC/DLC_02/Scenarios/NewWorldScenario/TurnsRemaining.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0294}}<syntaxhighlight lang="lua">if (pTeam:GetTeamTechs():HasTech(iTech)) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|UnitPanel.lua}}
:<code>UI/InGame/WorldView/UnitPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1116}}<syntaxhighlight lang="lua">if (iPrereqTech ~= -1 and not pActiveTeam:GetTeamTechs():HasTech(iPrereqTech)) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|WhosWinningPopup.lua}}
:<code>UI/InGame/Popups/WhosWinningPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0229}}<syntaxhighlight lang="lua">return pTeam:GetTeamTechs():GetNumTechsKnown();</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetTeamTechs]]
[[Category:Civ5 Science API|GetTeamTechs]]
[[Category:Civ5 Diplomacy API|GetTeamTechs]]