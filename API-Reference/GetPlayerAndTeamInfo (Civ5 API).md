{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a global function. Use: <code>include("MapmakerUtilities.lua")</code>
}}


=Usage=
<code>'''int''', '''int''', table('''int''' => {{Type5|PlayerID}}), '''bool''', table('''int''' => '''int'''), '''table''' GetPlayerAndTeamInfo<b>(</b><b>)</b></code>


'''Returned Values'''
:No description available.


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|AssignStartingPlots.lua (G&K)}}
:<code>DLC/Expansion/Gameplay/Lua/AssignStartingPlots.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1469}}<syntaxhighlight lang="lua">self.iNumCivs, self.iNumCityStates, self.player_ID_list, self.bTeamGame, self.teams_with_major_civs, self.number_civs_per_team = GetPlayerAndTeamInfo()</syntaxhighlight>
{{CodeLine5|1470}}<syntaxhighlight lang="lua">self.iNumCityStatesUnassigned = self.iNumCityStates;</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|Ring.lua}}
:<code>Maps/Ring.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0566}}<syntaxhighlight lang="lua">self.iNumCivs, self.iNumCityStates, self.player_ID_list, self.bTeamGame, self.teams_with_major_civs, self.number_civs_per_team = GetPlayerAndTeamInfo()</syntaxhighlight>
{{CodeLine5|0567}}<syntaxhighlight lang="lua">if self.iNumCityStates > 5 then</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetPlayerAndTeamInfo]]
[[Category:Civ5 Players API|GetPlayerAndTeamInfo]]
[[Category:Civ5 Diplomacy API|GetPlayerAndTeamInfo]]