{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|ID.png|The <code>KeyType</code> pseudo-type is actually a regular '''integer'''. Pseudo-types do not exist in Lua, they only serve a documentation purpose on the wiki!
* {{Lua}} Integers labeled as <code>KeyType</code> corresponds to the constants defined in the '''Keys''' Lua enumeration.
}}


= Lua: the Keys enumeration =
Firaxis provides a Lua enumeration named <code>Keys</code>. This is just a regular global table. Its keys are the constants' names and the pairs the corresponding values.

<br/>Below are the values found in this enumeration.
<code>
{|
|-
!align="left" |Key
!
!align="left" |Value 
|-
|align="left" |"VK_BACK"
|
|align="right" |8
|-
|align="left" |"VK_TAB"
|
|align="right" |9
|-
|align="left" |"VK_CLEAR"
|
|align="right" |12
|-
|align="left" |"VK_RETURN"
|
|align="right" |13
|-
|align="left" |"VK_SHIFT"
|
|align="right" |16
|-
|align="left" |"VK_CONTROL"
|
|align="right" |17
|-
|align="left" |"VK_MENU"
|
|align="right" |18
|-
|align="left" |"VK_PAUSE"
|
|align="right" |19
|-
|align="left" |"VK_CAPITAL"
|
|align="right" |20
|-
|align="left" |"VK_HANGEUL"
|
|align="right" |21
|-
|align="left" |"VK_HANGUL"
|
|align="right" |21
|-
|align="left" |"VK_KANA"
|
|align="right" |21
|-
|align="left" |"VK_JUNJA"
|
|align="right" |23
|-
|align="left" |"VK_FINAL"
|
|align="right" |24
|-
|align="left" |"VK_HANJA"
|
|align="right" |25
|-
|align="left" |"VK_KANJI"
|
|align="right" |25
|-
|align="left" |"VK_ESCAPE"
|
|align="right" |27
|-
|align="left" |"VK_CONVERT"
|
|align="right" |28
|-
|align="left" |"VK_NONCONVERT"
|
|align="right" |29
|-
|align="left" |"VK_ACCEPT"
|
|align="right" |30
|-
|align="left" |"VK_MODECHANGE"
|
|align="right" |31
|-
|align="left" |"VK_SPACE"
|
|align="right" |32
|-
|align="left" |"VK_PRIOR"
|
|align="right" |33
|-
|align="left" |"VK_NEXT"
|
|align="right" |34
|-
|align="left" |"VK_END"
|
|align="right" |35
|-
|align="left" |"VK_HOME"
|
|align="right" |36
|-
|align="left" |"VK_LEFT"
|
|align="right" |37
|-
|align="left" |"VK_UP"
|
|align="right" |38
|-
|align="left" |"VK_RIGHT"
|
|align="right" |39
|-
|align="left" |"VK_DOWN"
|
|align="right" |40
|-
|align="left" |"VK_SELECT"
|
|align="right" |41
|-
|align="left" |"VK_PRINT"
|
|align="right" |42
|-
|align="left" |"VK_EXECUTE"
|
|align="right" |43
|-
|align="left" |"VK_SNAPSHOT"
|
|align="right" |44
|-
|align="left" |"VK_INSERT"
|
|align="right" |45
|-
|align="left" |"VK_DELETE"
|
|align="right" |46
|-
|align="left" |"VK_HELP"
|
|align="right" |47
|-
|align="left" |"0"
|
|align="right" |48
|-
|align="left" |"1"
|
|align="right" |49
|-
|align="left" |"2"
|
|align="right" |50
|-
|align="left" |"3"
|
|align="right" |51
|-
|align="left" |"4"
|
|align="right" |52
|-
|align="left" |"5"
|
|align="right" |53
|-
|align="left" |"6"
|
|align="right" |54
|-
|align="left" |"7"
|
|align="right" |55
|-
|align="left" |"8"
|
|align="right" |56
|-
|align="left" |"9"
|
|align="right" |57
|-
|align="left" |"A"
|
|align="right" |65
|-
|align="left" |"B"
|
|align="right" |66
|-
|align="left" |"C"
|
|align="right" |67
|-
|align="left" |"D"
|
|align="right" |68
|-
|align="left" |"E"
|
|align="right" |69
|-
|align="left" |"F"
|
|align="right" |70
|-
|align="left" |"G"
|
|align="right" |71
|-
|align="left" |"H"
|
|align="right" |72
|-
|align="left" |"I"
|
|align="right" |73
|-
|align="left" |"J"
|
|align="right" |74
|-
|align="left" |"K"
|
|align="right" |75
|-
|align="left" |"L"
|
|align="right" |76
|-
|align="left" |"M"
|
|align="right" |77
|-
|align="left" |"N"
|
|align="right" |78
|-
|align="left" |"O"
|
|align="right" |79
|-
|align="left" |"P"
|
|align="right" |80
|-
|align="left" |"Q"
|
|align="right" |81
|-
|align="left" |"R"
|
|align="right" |82
|-
|align="left" |"S"
|
|align="right" |83
|-
|align="left" |"T"
|
|align="right" |84
|-
|align="left" |"U"
|
|align="right" |85
|-
|align="left" |"V"
|
|align="right" |86
|-
|align="left" |"W"
|
|align="right" |87
|-
|align="left" |"X"
|
|align="right" |88
|-
|align="left" |"Y"
|
|align="right" |89
|-
|align="left" |"Z"
|
|align="right" |90
|-
|align="left" |"VK_LWIN"
|
|align="right" |91
|-
|align="left" |"VK_RWIN"
|
|align="right" |92
|-
|align="left" |"VK_APPS"
|
|align="right" |93
|-
|align="left" |"VK_SLEEP"
|
|align="right" |95
|-
|align="left" |"VK_NUMPAD0"
|
|align="right" |96
|-
|align="left" |"VK_NUMPAD1"
|
|align="right" |97
|-
|align="left" |"VK_NUMPAD2"
|
|align="right" |98
|-
|align="left" |"VK_NUMPAD3"
|
|align="right" |99
|-
|align="left" |"VK_NUMPAD4"
|
|align="right" |100
|-
|align="left" |"VK_NUMPAD5"
|
|align="right" |101
|-
|align="left" |"VK_NUMPAD6"
|
|align="right" |102
|-
|align="left" |"VK_NUMPAD7"
|
|align="right" |103
|-
|align="left" |"VK_NUMPAD8"
|
|align="right" |104
|-
|align="left" |"VK_NUMPAD9"
|
|align="right" |105
|-
|align="left" |"VK_MULTIPLY"
|
|align="right" |106
|-
|align="left" |"VK_ADD"
|
|align="right" |107
|-
|align="left" |"VK_SEPARATOR"
|
|align="right" |108
|-
|align="left" |"VK_SUBTRACT"
|
|align="right" |109
|-
|align="left" |"VK_DECIMAL"
|
|align="right" |110
|-
|align="left" |"VK_DIVIDE"
|
|align="right" |111
|-
|align="left" |"VK_F1"
|
|align="right" |112
|-
|align="left" |"VK_F2"
|
|align="right" |113
|-
|align="left" |"VK_F3"
|
|align="right" |114
|-
|align="left" |"VK_F4"
|
|align="right" |115
|-
|align="left" |"VK_F5"
|
|align="right" |116
|-
|align="left" |"VK_F6"
|
|align="right" |117
|-
|align="left" |"VK_F7"
|
|align="right" |118
|-
|align="left" |"VK_F8"
|
|align="right" |119
|-
|align="left" |"VK_F9"
|
|align="right" |120
|-
|align="left" |"VK_F10"
|
|align="right" |121
|-
|align="left" |"VK_F11"
|
|align="right" |122
|-
|align="left" |"VK_F12"
|
|align="right" |123
|-
|align="left" |"VK_F13"
|
|align="right" |124
|-
|align="left" |"VK_F14"
|
|align="right" |125
|-
|align="left" |"VK_F15"
|
|align="right" |126
|-
|align="left" |"VK_F16"
|
|align="right" |127
|-
|align="left" |"VK_F17"
|
|align="right" |128
|-
|align="left" |"VK_F18"
|
|align="right" |129
|-
|align="left" |"VK_F19"
|
|align="right" |130
|-
|align="left" |"VK_F20"
|
|align="right" |131
|-
|align="left" |"VK_F21"
|
|align="right" |132
|-
|align="left" |"VK_F22"
|
|align="right" |133
|-
|align="left" |"VK_F23"
|
|align="right" |134
|-
|align="left" |"VK_F24"
|
|align="right" |135
|-
|align="left" |"VK_NUMLOCK"
|
|align="right" |144
|-
|align="left" |"VK_SCROLL"
|
|align="right" |145
|-
|align="left" |"VK_OEM_NEC_EQUAL"
|
|align="right" |146
|-
|align="left" |"VK_OEM_FJ_JISHO"
|
|align="right" |146
|-
|align="left" |"VK_OEM_FJ_MASSHOU"
|
|align="right" |147
|-
|align="left" |"VK_OEM_FJ_TOUROKU"
|
|align="right" |148
|-
|align="left" |"VK_OEM_FJ_LOYA"
|
|align="right" |149
|-
|align="left" |"VK_OEM_FJ_ROYA"
|
|align="right" |150
|-
|align="left" |"VK_LSHIFT"
|
|align="right" |160
|-
|align="left" |"VK_RSHIFT"
|
|align="right" |161
|-
|align="left" |"VK_LCONTROL"
|
|align="right" |162
|-
|align="left" |"VK_RCONTROL"
|
|align="right" |163
|-
|align="left" |"VK_LMENU"
|
|align="right" |164
|-
|align="left" |"VK_RMENU"
|
|align="right" |165
|-
|align="left" |"VK_BROWSER_BACK"
|
|align="right" |166
|-
|align="left" |"VK_BROWSER_FORWARD"
|
|align="right" |167
|-
|align="left" |"VK_BROWSER_REFRESH"
|
|align="right" |168
|-
|align="left" |"VK_BROWSER_STOP"
|
|align="right" |169
|-
|align="left" |"VK_BROWSER_SEARCH"
|
|align="right" |170
|-
|align="left" |"VK_BROWSER_FAVORITES"
|
|align="right" |171
|-
|align="left" |"VK_BROWSER_HOME"
|
|align="right" |172
|-
|align="left" |"VK_VOLUME_MUTE"
|
|align="right" |173
|-
|align="left" |"VK_VOLUME_DOWN"
|
|align="right" |174
|-
|align="left" |"VK_VOLUME_UP"
|
|align="right" |175
|-
|align="left" |"VK_MEDIA_NEXT_TRACK"
|
|align="right" |176
|-
|align="left" |"VK_MEDIA_PREV_TRACK"
|
|align="right" |177
|-
|align="left" |"VK_MEDIA_STOP"
|
|align="right" |178
|-
|align="left" |"VK_MEDIA_PLAY_PAUSE"
|
|align="right" |179
|-
|align="left" |"VK_LAUNCH_MAIL"
|
|align="right" |180
|-
|align="left" |"VK_LAUNCH_MEDIA_SELECT"
|
|align="right" |181
|-
|align="left" |"VK_LAUNCH_APP1"
|
|align="right" |182
|-
|align="left" |"VK_LAUNCH_APP2"
|
|align="right" |183
|-
|align="left" |"VK_OEM_1"
|
|align="right" |186
|-
|align="left" |"VK_OEM_PLUS"
|
|align="right" |187
|-
|align="left" |"VK_OEM_COMMA"
|
|align="right" |188
|-
|align="left" |"VK_OEM_MINUS"
|
|align="right" |189
|-
|align="left" |"VK_OEM_PERIOD"
|
|align="right" |190
|-
|align="left" |"VK_OEM_2"
|
|align="right" |191
|-
|align="left" |"VK_OEM_3"
|
|align="right" |192
|-
|align="left" |"VK_OEM_4"
|
|align="right" |219
|-
|align="left" |"VK_OEM_5"
|
|align="right" |220
|-
|align="left" |"VK_OEM_6"
|
|align="right" |221
|-
|align="left" |"VK_OEM_7"
|
|align="right" |222
|-
|align="left" |"VK_OEM_8"
|
|align="right" |223
|-
|align="left" |"VK_OEM_AX"
|
|align="right" |225
|-
|align="left" |"VK_OEM_102"
|
|align="right" |226
|-
|align="left" |"VK_ICO_HELP"
|
|align="right" |227
|-
|align="left" |"VK_ICO_00"
|
|align="right" |228
|-
|align="left" |"VK_PROCESSKEY"
|
|align="right" |229
|-
|align="left" |"VK_ICO_CLEAR"
|
|align="right" |230
|-
|align="left" |"VK_PACKET"
|
|align="right" |231
|-
|align="left" |"VK_OEM_RESET"
|
|align="right" |233
|-
|align="left" |"VK_OEM_JUMP"
|
|align="right" |234
|-
|align="left" |"VK_OEM_PA1"
|
|align="right" |235
|-
|align="left" |"VK_OEM_PA2"
|
|align="right" |236
|-
|align="left" |"VK_OEM_PA3"
|
|align="right" |237
|-
|align="left" |"VK_OEM_WSCTRL"
|
|align="right" |238
|-
|align="left" |"VK_OEM_CUSEL"
|
|align="right" |239
|-
|align="left" |"VK_OEM_ATTN"
|
|align="right" |240
|-
|align="left" |"VK_OEM_FINISH"
|
|align="right" |241
|-
|align="left" |"VK_OEM_COPY"
|
|align="right" |242
|-
|align="left" |"VK_OEM_AUTO"
|
|align="right" |243
|-
|align="left" |"VK_OEM_ENLW"
|
|align="right" |244
|-
|align="left" |"VK_OEM_BACKTAB"
|
|align="right" |245
|-
|align="left" |"VK_ATTN"
|
|align="right" |246
|-
|align="left" |"VK_CRSEL"
|
|align="right" |247
|-
|align="left" |"VK_EXSEL"
|
|align="right" |248
|-
|align="left" |"VK_EREOF"
|
|align="right" |249
|-
|align="left" |"VK_PLAY"
|
|align="right" |250
|-
|align="left" |"VK_ZOOM"
|
|align="right" |251
|-
|align="left" |"VK_NONAME"
|
|align="right" |252
|-
|align="left" |"VK_PA1"
|
|align="right" |253
|-
|align="left" |"VK_OEM_CLEAR"
|
|align="right" |254
|}</code>


= Examples =
Here is how to use the LUA enumeration to retrieve the ''ID'' from the ''type''. Those examples will return and assign the integer value 8.
<syntaxhighlight lang="lua" class="civ5-example">
local id = Keys.VK_BACK
local id = Keys["VK_BACK"]
</syntaxhighlight>


=Used by=
{|cellspacing="4" cellpadding="0" width="100%" style="background-color:#F0F0F0"
<!-- 
SETINPUTHANDLER
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Context}}:{{Func5|UIElement|SetInputHandler}}<b>(</b>('''void''' func<b>(</b>{{Type5|MouseEventType}} uiMsg, {{Type5|KeyType}} wParam, '''unknown''' lParam<b>)</b>) InputHandler<b>)</b></code>
<!-- 
KEYUPEVENT
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Events}}.{{Func5|Events|KeyUpEvent}}<b>(</b>{{Type5|KeyType}} wParam<b>)</b></code>
<!-- 
DEBUGKEYHANDLER
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|UI}}.{{Func5|UI|DebugKeyHandler}}<b>(</b>{{Type5|KeyEventType}} uiMsg, {{Type5|KeyType}} wParam, '''unknown''' lParam<b>)</b></code>
|}




{{Civ5 API Footer}}
[[Category:Civ5 Types|KeyType]]