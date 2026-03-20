{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Team}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>{{Type5|TeamID}} Team:GetLiberatedByTeam<b>(</b>{{Type5|TeamID}} index<b>)</b></code>


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

{{PseudoH4|VictoryProgress.lua}}
:<code>UI/InGame/Popups/VictoryProgress.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0374}}<syntaxhighlight lang="lua">not pPlayer:IsAlive() or Teams[pPlayer:GetTeam()]:GetLiberatedByTeam() ~= -1,</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0685}}<syntaxhighlight lang="lua">not pPlayer:IsAlive() or Teams[pTeam]:GetLiberatedByTeam() ~= -1,</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0720}}<syntaxhighlight lang="lua">if(pTeam == v:GetLiberatedByTeam()) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|VictoryProgress.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/Popups/VictoryProgress.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0690}}<syntaxhighlight lang="lua">not pPlayer:IsAlive() or Teams[iTeam]:GetLiberatedByTeam() ~= -1,</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0722}}<syntaxhighlight lang="lua">if (pTeamLoop:GetLiberatedByTeam() == iTeam) then</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetLiberatedByTeam]]
[[Category:Civ5 Diplomacy API|GetLiberatedByTeam]]
[[Category:Civ5 United Nations API|GetLiberatedByTeam]]
[[Category:Civ5 City States API|GetLiberatedByTeam]]