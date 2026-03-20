{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a built-in global function. No <code>include</code> statement is needed.
}}


=Usage=
<code>'''void''' Water_SetSpec<b>(</b>'''int''' waterSunSpec, '''int''' waterSkySpec<b>)</b></code>


'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|waterSunSpec:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|waterSkySpec:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|TerrainPanel.lua}}
:<code>UI/InGame/TerrainPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0024}}<syntaxhighlight lang="lua">Water_SetSpec(g_iWaterSunSpec, g_iWaterSkySpec);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|Water_SetSpec]]