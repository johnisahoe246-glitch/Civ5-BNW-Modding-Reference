{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a global function. Use: <code>include("PlotMouseoverInclude.lua")</code>
}}


=Usage=
<code>'''string''' GetResourceString<b>(</b>{{Type5|Plot}} plot, '''bool''' longForm<b>)</b></code>


'''Returned Value'''
:No description available.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|plot:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|longForm:
|valign="top"| ''No description available.''
|}


=Source code samples=
{{PseudoH4|PlotHelpManager.lua}}
:<code>UI/InGame/PlotHelpManager.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0179}}<syntaxhighlight lang="lua">local strResource = GetResourceString(plot, true);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|PlotHelpText.lua}}
:<code>UI/InGame/WorldView/PlotHelpText.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0024}}<syntaxhighlight lang="lua">local strResourceAndImprovement = GetResourceString(plot, false);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetResourceString]]
[[Category:Civ5 Resources API|GetResourceString]]