{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a global function. Use: <code>include("FLuaVector.lua")</code>
}}


=Usage=
<code>{{Type5|Vector3}} Vector3<b>(</b>'''float''' i, '''float''' j, '''float''' k<b>)</b></code>


'''Returned Value'''
:No description available.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|i:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|j:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|k:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|UnitFlagManager.lua}}
:<code>UI/InGame/UnitFlagManager.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0920}}<syntaxhighlight lang="lua">local worldOffset = Vector3( 0, 0, 35 );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|UnitMemberOverlay.lua}}
:<code>UI/InGame/UnitMemberOverlay.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0136}}<syntaxhighlight lang="lua">local worldOffset = Vector3( 0, 0, 0 );</syntaxhighlight>
{{CodeLine5|0137}}<syntaxhighlight lang="lua">local position = VecAdd( Vector3( worldPosX, worldPosY, worldPosZ ), worldOffset );</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|Vector3]]