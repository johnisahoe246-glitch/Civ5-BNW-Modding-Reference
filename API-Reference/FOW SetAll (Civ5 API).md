{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a built-in global function. No <code>include</code> statement is needed.
}}


=Usage=
<code>'''void''' FOW_SetAll<b>(</b>{{Type5|FogOfWarModeType}} fogOfWarType<b>)</b></code>


'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|fogOfWarType:
|valign="top"| ''No description available.''
|}


=Source code samples=
{{PseudoH4|DebugMenu.lua}}
:<code>UI/InGame/DebugMenu.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0030}}<syntaxhighlight lang="lua">FOW_SetAll(0); -- corresponds to gameplay FOGOFWARMODE_OFF</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0051}}<syntaxhighlight lang="lua">FOW_SetAll(2); -- corresponds to gameplay FOGOFWARMODE_NOVIS</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0058}}<syntaxhighlight lang="lua">FOW_SetAll(1); -- corresponds to gameplay FOGOFWARMODE_UNEXPLORED</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|FOW_SetAll]]