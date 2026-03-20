{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Network}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''unknown''' Network.GetPlayerTurnSliceInfo<b>(</b>'''int''' arg0<b>)</b></code>


'''Returned Value'''
:No description available.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|arg0:
|valign="top"| ''No description available.''
|}


=Source code samples=
{{PseudoH4|NetworkDebug.lua}}
:<code>UI/InGame/NetworkDebug.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0028}}<syntaxhighlight lang="lua">local playerInfo = Network.GetPlayerTurnSliceInfo(i - 1);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetPlayerTurnSliceInfo]]
[[Category:Civ5 Players API|GetPlayerTurnSliceInfo]]
[[Category:Civ5 Turns API|GetPlayerTurnSliceInfo]]