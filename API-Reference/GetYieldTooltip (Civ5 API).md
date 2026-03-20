{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a global function. Use: <code>include("InfoTooltipInclude.lua")</code>
}}


=Usage=
<code>'''string''' GetYieldTooltip<b>(</b>{{Type5|City}} city, {{Type5|YieldType}} yieldType, '''int''' base, '''int''' total, '''string''' iconString, '''string''' modifiersString<b>)</b></code>


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
|valign="top" style="padding-right:6px;"|base:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|total:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|iconString:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|modifiersString:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|InfoTooltipInclude.lua}}
:<code>UI/InGame/InfoTooltipInclude.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0464}}<syntaxhighlight lang="lua">local strProductionBreakdown = GetYieldTooltip(pCity, YieldTypes.YIELD_PRODUCTION, iBaseProductionPT, iProductionPerTurn, "[ICON_PRODUCTION]", strCodeToolTip);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0632}}<syntaxhighlight lang="lua">local strYieldToolTip = GetYieldTooltip(pCity, iYieldType, iBaseYield, iTotalYield, strIcon, strModifiers);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetYieldTooltip]]
[[Category:Civ5 Yields API|GetYieldTooltip]]