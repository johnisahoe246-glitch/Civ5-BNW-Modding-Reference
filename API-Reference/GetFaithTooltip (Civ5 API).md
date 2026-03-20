{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a global function. Use: <code>include("InfoTooltipInclude.lua")</code>
<br/>
*This method was added in Gods & Kings.
}}


=Usage=
<code>'''string''' GetFaithTooltip<b>(</b>{{Type5|City}} city<b>)</b></code>


'''Returned Value'''
:No description available.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|city:
|valign="top"| ''No description available.''
|}


=Source code samples=
{{PseudoH4|CityView.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/CityView/CityView.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1693}}<syntaxhighlight lang="lua">local strFaithToolTip = GetFaithTooltip(pCity);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ProductionPopup.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/Popups/ProductionPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0305}}<syntaxhighlight lang="lua">local strFaithToolTip = GetFaithTooltip(city);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetFaithTooltip]]
[[Category:Civ5 Religion API|GetFaithTooltip]]