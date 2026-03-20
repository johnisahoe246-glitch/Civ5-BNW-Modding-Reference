{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Game}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''int''' Game.GetPreviousVoteCast<b>(</b>{{Type5|TeamID}} teamLoop<b>)</b></code>


'''Returned Value'''
:No description available.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|teamLoop:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|VictoryProgress.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/Popups/VictoryProgress.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0735}}<syntaxhighlight lang="lua">elseif (not pLeaderLoop:IsMinorCiv() and Game.GetPreviousVoteCast(iTeamLoop) == iTeam) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0781}}<syntaxhighlight lang="lua">local iPreviousVoteCast = Game.GetPreviousVoteCast(iTeam);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetPreviousVoteCast]]
[[Category:Civ5 United Nations API|GetPreviousVoteCast]]