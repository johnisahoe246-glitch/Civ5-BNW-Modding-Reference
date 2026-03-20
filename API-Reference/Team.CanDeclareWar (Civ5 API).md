{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Team}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''int''' Team:CanDeclareWar<b>(</b>{{Type5|TeamID}} team<b>)</b></code>


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

{{PseudoH4|DiploList.lua}}
:<code>UI/InGame/DiploList.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0170}}<syntaxhighlight lang="lua">if (g_pTeam:CanDeclareWar(Players[ ePlayer ]:GetTeam())) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0355}}<syntaxhighlight lang="lua">not g_pTeam:IsAtWar( pOtherPlayer:GetTeam()) and g_pTeam:CanDeclareWar(pOtherPlayer:GetTeam()) and</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|LeaderHeadRoot.lua}}
:<code>UI/InGame/LeaderHead/LeaderHeadRoot.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0188}}<syntaxhighlight lang="lua">elseif (not pActiveTeam:CanDeclareWar(g_iAITeam)) then</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|CanDeclareWar]]
[[Category:Civ5 Diplomacy API|CanDeclareWar]]