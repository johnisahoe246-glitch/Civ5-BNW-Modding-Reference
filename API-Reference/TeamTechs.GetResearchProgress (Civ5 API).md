{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|TeamTechs}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''int''' TeamTechs:GetResearchProgress<b>(</b>{{Type5|TechType}} index<b>)</b></code>


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

{{PseudoH4|TechPopup.lua}}
:<code>UI/InGame/TechPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0176}}<syntaxhighlight lang="lua">local currentResearchProgress = teamTechs:GetResearchProgress(techID);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetResearchProgress]]
[[Category:Civ5 Science API|GetResearchProgress]]