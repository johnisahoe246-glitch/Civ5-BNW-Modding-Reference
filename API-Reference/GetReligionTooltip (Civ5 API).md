{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a global function. Use: <code>include("InfoTooltipInclude.lua")</code>
<br/>
*This method was added in Gods & Kings.
}}


=Usage=
<code>'''string''' GetReligionTooltip<b>(</b>{{Type5|City}} city<b>)</b></code>


'''Returned Value'''
:No description available.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|city:
|valign="top"| ''No description available.''
|}


=Source code samples=
{{PseudoH4|CityBannerManager.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/CityBannerManager.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0209}}<syntaxhighlight lang="lua">religionToolTip = GetReligionTooltip(city);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|InfoTooltipInclude.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/InfoTooltipInclude.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0647}}<syntaxhighlight lang="lua">table.insert(faithTips, GetReligionTooltip(pCity));</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetReligionTooltip]]
[[Category:Civ5 Religion API|GetReligionTooltip]]