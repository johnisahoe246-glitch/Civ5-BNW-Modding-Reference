{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a global function. Use: <code>include("InfoTooltipInclude.lua")</code>
}}


=Usage=
<code>'''string''' GetGoldTooltip<b>(</b>{{Type5|City}} city<b>)</b></code>


'''Returned Value'''
:No description available.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|city:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|CityView.lua}}
:<code>UI/InGame/CityView/CityView.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1651}}<syntaxhighlight lang="lua">local strGoldToolTip = GetGoldTooltip(pCity);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ProductionPopup.lua}}
:<code>UI/InGame/Popups/ProductionPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0243}}<syntaxhighlight lang="lua">local strGoldToolTip = GetGoldTooltip(city);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetGoldTooltip]]
[[Category:Civ5 Gold API|GetGoldTooltip]]