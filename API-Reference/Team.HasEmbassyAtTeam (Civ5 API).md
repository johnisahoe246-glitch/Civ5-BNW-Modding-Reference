{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Team}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''bool''' Team:HasEmbassyAtTeam<b>(</b>{{Type5|TeamID}} themTeam<b>)</b></code>


'''Returned Value'''
:No description available.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|themTeam:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|TradeLogic.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/WorldView/TradeLogic.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1103}}<syntaxhighlight lang="lua">if (g_pThemTeam:HasEmbassyAtTeam(g_iUsTeam)) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1126}}<syntaxhighlight lang="lua">if (g_pUsTeam:HasEmbassyAtTeam(g_iThemTeam)) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1160}}<syntaxhighlight lang="lua">elseif (not g_pUsTeam:HasEmbassyAtTeam(g_iThemTeam)) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1180}}<syntaxhighlight lang="lua">elseif (not g_pThemTeam:HasEmbassyAtTeam(g_iUsTeam)) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1204}}<syntaxhighlight lang="lua">elseif (not g_pUsTeam:HasEmbassyAtTeam(g_iThemTeam) or not g_pThemTeam:HasEmbassyAtTeam(g_iUsTeam)) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1268}}<syntaxhighlight lang="lua">if (not g_pUsTeam:HasEmbassyAtTeam(g_iThemTeam) or not g_pThemTeam:HasEmbassyAtTeam(g_iUsTeam)) then</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|HasEmbassyAtTeam]]
[[Category:Civ5 Diplomacy API|HasEmbassyAtTeam]]