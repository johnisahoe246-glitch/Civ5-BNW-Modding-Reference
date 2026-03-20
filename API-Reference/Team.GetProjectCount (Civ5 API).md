{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Team}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''int''' Team:GetProjectCount<b>(</b>{{Type5|ProjectType}} index<b>)</b></code>


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
{{CodeLine5|0290}}<syntaxhighlight lang="lua">if(Teams[iTeam]:GetProjectCount(apolloProj) == 1) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0320}}<syntaxhighlight lang="lua">if(v:GetProjectCount(apolloProj) == 1) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0341}}<syntaxhighlight lang="lua">local numBuilt = Teams[ iTeam ]:GetProjectCount( proj );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0440}}<syntaxhighlight lang="lua">if(Teams[pPlayer:GetTeam()]:GetProjectCount(proj) > 0)then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0584}}<syntaxhighlight lang="lua">if(Teams[pTeam]:GetProjectCount(apolloProj) == 1) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0605}}<syntaxhighlight lang="lua">local apolloA = pTeamA:GetProjectCount(apolloProj) == 1;</syntaxhighlight>
{{CodeLine5|0606}}<syntaxhighlight lang="lua">local apolloB = pTeamB:GetProjectCount(apolloProj) == 1;</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0615}}<syntaxhighlight lang="lua">partsA = partsA + pTeamA:GetProjectCount(proj);</syntaxhighlight>
{{CodeLine5|0616}}<syntaxhighlight lang="lua">partsB = partsB + pTeamB:GetProjectCount(proj);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetProjectCount]]
[[Category:Civ5 Buildings API|GetProjectCount]]