{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a built-in global function. No <code>include</code> statement is needed.
}}


=Usage=
<code>'''void''' Water_SetAutoReload<b>(</b>'''bool''' waterReload<b>)</b></code>


'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|waterReload:
|valign="top"| ''No description available.''
|}


=Source code samples=
{{PseudoH4|TerrainPanel.lua}}
:<code>UI/InGame/TerrainPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0023}}<syntaxhighlight lang="lua">Water_SetAutoReload(g_bWaterReload);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0046}}<syntaxhighlight lang="lua">Water_SetAutoReload(g_iWaterReload);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|Water_SetAutoReload]]