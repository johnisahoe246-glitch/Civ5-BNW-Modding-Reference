{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|TeamTechs}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>{{Type5|TechType}} TeamTechs:GetLastTechAcquired<b>(</b>{{Type5|TechType}} index<b>)</b></code>


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

{{PseudoH4|TechPanel.lua}}
:<code>UI/InGame/TechPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0057}}<syntaxhighlight lang="lua">eRecentTech = pTeamTechs:GetLastTechAcquired();</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetLastTechAcquired]]
[[Category:Civ5 Science API|GetLastTechAcquired]]