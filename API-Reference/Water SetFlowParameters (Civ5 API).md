{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a built-in global function. No <code>include</code> statement is needed.
}}


=Usage=
<code>'''void''' Water_SetFlowParameters<b>(</b>'''int''' waterFlowStrength, '''int''' waterNoiseStrength, '''int''' waterNoiseScale<b>)</b></code>


'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|waterFlowStrength:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|waterNoiseStrength:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|waterNoiseScale:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|TerrainPanel.lua}}
:<code>UI/InGame/TerrainPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0029}}<syntaxhighlight lang="lua">Water_SetFlowParameters(g_iWaterFlowStrength, g_iWaterNoiseStrength, g_iWaterNoiseScale);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|Water_SetFlowParameters]]