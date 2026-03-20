{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Network}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''void''' Network.SendChangeWar<b>(</b>{{Type5|TeamID}} minorCivTeam, '''bool''' arg1<b>)</b></code>


'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|minorCivTeam:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|arg1:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|CityStateDiploPopup.lua}}
:<code>UI/InGame/Popups/CityStateDiploPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0673}}<syntaxhighlight lang="lua">Network.SendChangeWar(g_iMinorCivTeamID, false);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0698}}<syntaxhighlight lang="lua">Network.SendChangeWar(g_iMinorCivTeamID, true);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DeclareWarMovePopup.lua}}
:<code>UI/InGame/PopupsGeneric/DeclareWarMovePopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0070}}<syntaxhighlight lang="lua">Network.SendChangeWar(eRivalTeam, true);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DiploList.lua}}
:<code>UI/InGame/DiploList.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0066}}<syntaxhighlight lang="lua">Network.SendChangeWar( g_WarTarget, true);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|SendChangeWar]]
[[Category:Civ5 Diplomacy API|SendChangeWar]]