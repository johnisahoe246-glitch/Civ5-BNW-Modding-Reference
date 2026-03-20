{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Locale}}.<br/>
This is a static method, invoke it with a dot.
}}


Returns a localized description for a hotkey


=Usage=
<code>'''unknown''' Locale.GetHotKeyDescription<b>(</b>'''string''' key, '''bool''' ctrl = nil, '''bool''' alt = nil, '''bool''' shift = nil<b>)</b></code>


'''Returned Value'''
:Returns a localized string for the hot key.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|key:
|valign="top"| ''The name of the hot key.''
|-
|valign="top" style="padding-right:6px;"|ctrl:
|valign="top"| ''Whether the control key is pressed.''
|-
|valign="top" style="padding-right:6px;"|alt:
|valign="top"| ''Whether the alt key is pressed.''
|-
|valign="top" style="padding-right:6px;"|shift:
|valign="top"| ''Whether the shift key is pressed.''
|}


=Examples=
<syntaxhighlight lang="lua" class="civ5-example">
local hotKeyDesc = Locale.GetHotKeyDescription("KB_Y", false, true, true);</syntaxhighlight>


=Source code samples=
{{PseudoH4|MiniMapPanel.lua}}
:<code>UI/InGame/WorldView/MiniMapPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0422}}<syntaxhighlight lang="lua">local keyDesc = Locale.GetHotKeyDescription(hotKey, controlInfo.CtrlDown, controlInfo.AltDown, controlInfo.ShiftDown);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetHotKeyDescription]]