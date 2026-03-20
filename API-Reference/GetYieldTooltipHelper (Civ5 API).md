{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a global function. Use: <code>include("InfoTooltipInclude.lua")</code>
}}


=Usage=
<code>'''string''' GetYieldTooltipHelper<b>(</b>{{Type5|City}} city, {{Type5|YieldType}} yieldType, '''string''' icon<b>)</b></code>


'''Returned Value'''
:No description available.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|city:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|yieldType:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|icon:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|InfoTooltipInclude.lua}}
:<code>UI/InGame/InfoTooltipInclude.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0414}}<syntaxhighlight lang="lua">strFoodToolTip = strFoodToolTip .. GetYieldTooltipHelper(pCity, iYieldType, "[ICON_FOOD]");</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0430}}<syntaxhighlight lang="lua">strGoldToolTip = strGoldToolTip .. GetYieldTooltipHelper(pCity, iYieldType, "[ICON_GOLD]");</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0451}}<syntaxhighlight lang="lua">strScienceToolTip = strScienceToolTip .. GetYieldTooltipHelper(pCity, iYieldType, "[ICON_RESEARCH]");</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetYieldTooltipHelper]]
[[Category:Civ5 Yields API|GetYieldTooltipHelper]]