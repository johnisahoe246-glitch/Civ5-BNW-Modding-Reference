{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a global function. Use: <code>include("InfoTooltipInclude.lua")</code>
}}


=Usage=
<code>'''string''' GetHelpTextForUnit<b>(</b>{{Type5|UnitType}} unit, '''bool''' includeRequirementsInfo<b>)</b></code>


'''Returned Value'''
:No description available.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|unit:
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
{{CodeLine5|0551}}<syntaxhighlight lang="lua">strToolTip = Locale.ConvertTextKey(GetHelpTextForUnit(unitProduction, true)) .. "[NEWLINE][NEWLINE]" .. strToolTip;</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0920}}<syntaxhighlight lang="lua">local strToolTip = Locale.ConvertTextKey(GetHelpTextForUnit(id, bIncludeRequirementsInfo));</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TechButtonInclude.lua}}
:<code>UI/InGame/TechTree/TechButtonInclude.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0346}}<syntaxhighlight lang="lua">thisButton:SetToolTipString( GetHelpTextForUnit(thisUnitInfo.ID, bIncludeRequirementsInfo) );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|UniqueBonuses.lua}}
:<code>UI/FrontEnd/GameSetup/UniqueBonuses.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0020}}<syntaxhighlight lang="lua">thisButton:SetToolTipString( Locale.ConvertTextKey(GetHelpTextForUnit(thisUnitInfo.ID, true)));</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetHelpTextForUnit]]
[[Category:Civ5 Units API|GetHelpTextForUnit]]