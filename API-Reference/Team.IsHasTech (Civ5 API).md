{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Team}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''bool''' Team:IsHasTech<b>(</b>{{Type5|TechType}} index<b>)</b></code>


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

{{PseudoH4|GameplayUtils.lua (G&K)}}
:<code>DLC/Expansion/Scenarios/SteampunkScenario/GameplayUtils.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0199}}<syntaxhighlight lang="lua">if (Teams[iTeam]:IsHasTech(iTech)) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TechPopup.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/TechPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0140}}<syntaxhighlight lang="lua">if (opponentTeam:IsHasTech(techID)) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TurnsRemaining.lua (G&K)}}
:<code>DLC/Expansion/Scenarios/MedievalScenario/TurnsRemaining.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0655}}<syntaxhighlight lang="lua">if (pTeam:IsHasTech(GameInfoTypes["TECH_EXPLORATION"])) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|VictoryProgress.lua}}
:<code>UI/InGame/Popups/VictoryProgress.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0993}}<syntaxhighlight lang="lua">if(pTeam:IsHasTech(techID)) then</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|IsHasTech]]
[[Category:Civ5 Science API|IsHasTech]]