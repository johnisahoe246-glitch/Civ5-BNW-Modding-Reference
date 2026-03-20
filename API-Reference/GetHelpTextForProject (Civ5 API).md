{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a global function. Use: <code>include("InfoTooltipInclude.lua")</code>
}}


=Usage=
<code>'''string''' GetHelpTextForProject<b>(</b>{{Type5|ProjectType}} project, '''bool''' includeRequirementsInfo<b>)</b></code>


'''Returned Value'''
:No description available.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|project:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|includeRequirementsInfo:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|ProductionPopup.lua}}
:<code>UI/InGame/Popups/ProductionPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0575}}<syntaxhighlight lang="lua">strToolTip = Locale.ConvertTextKey(GetHelpTextForProject(projectProduction, true)) .. "[NEWLINE][NEWLINE]" .. strToolTip;</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0979}}<syntaxhighlight lang="lua">strToolTip = GetHelpTextForProject(id, bIncludeRequirementsInfo);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TechButtonInclude.lua}}
:<code>UI/InGame/TechTree/TechButtonInclude.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0390}}<syntaxhighlight lang="lua">thisButton:SetToolTipString( GetHelpTextForProject(thisProjectInfo.ID, bIncludeRequirementsInfo) );</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetHelpTextForProject]]
[[Category:Civ5 Buildings API|GetHelpTextForProject]]