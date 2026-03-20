{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a global function. Use: <code>include("InfoTooltipInclude.lua")</code>
}}


=Usage=
<code>'''string''' GetHelpTextForImprovement<b>(</b>{{Type5|ImprovementType}} improvement, '''bool''' excludeName, '''bool''' excludeHeader, '''bool''' noMaintenance<b>)</b></code>


'''Returned Value'''
:No description available.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|improvement:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|excludeName:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|excludeHeader:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|noMaintenance:
|valign="top"| ''No description available.''
|}


=Source code samples=
{{PseudoH4|UniqueBonuses.lua}}
:<code>UI/FrontEnd/GameSetup/UniqueBonuses.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0076}}<syntaxhighlight lang="lua">thisButton:SetToolTipString( Locale.ConvertTextKey(GetHelpTextForImprovement(thisImprovmentInfo.ID, false, false, false)));</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetHelpTextForImprovement]]
[[Category:Civ5 Improvements API|GetHelpTextForImprovement]]