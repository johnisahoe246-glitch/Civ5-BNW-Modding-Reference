{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Team}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''int''' Team:GetNumTurnsLockedIntoWar<b>(</b>{{Type5|TeamID}} team<b>)</b></code>


'''Returned Value'''
:No description available.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|team:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|LeaderHeadRoot.lua}}
:<code>UI/InGame/LeaderHead/LeaderHeadRoot.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0168}}<syntaxhighlight lang="lua">local iLockedWarTurns = pActiveTeam:GetNumTurnsLockedIntoWar(g_iAITeam);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetNumTurnsLockedIntoWar]]
[[Category:Civ5 Diplomacy API|GetNumTurnsLockedIntoWar]]