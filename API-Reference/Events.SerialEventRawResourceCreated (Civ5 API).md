{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Events}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''void''' Events.SerialEventRawResourceCreated<b>(</b>'''float''' hexX, '''int''' hexY, {{Type5|ArtStyleType}} continent, {{Type5|ArtStyleType}} continent, {{Type5|PlayerID}} player, '''int''' arg5, '''int''' createResourceType, '''int''' arg7, '''int''' arg8<b>)</b></code>


'''Event Type'''
:Regular event: you can subscribe to it through <code>Events.SerialEventRawResourceCreated.Add(''<function handler>'')</code> or invoke it directly through <code>Events.SerialEventRawResourceCreated(''<arguments list>'')</code>.

'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|hexX:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|hexY:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|continent:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|continent:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|player:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|arg5:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|createResourceType:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|arg7:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|arg8:
|valign="top"| ''No description available.''
|}


=Source code samples=
{{PseudoH4|DebugMode.lua}}
:<code>UI/InGame/DebugMode.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0463}}<syntaxhighlight lang="lua">Events.SerialEventRawResourceCreated( iHexX, iHexY, continent,   continent,     playerID,   -1,              g_iCreateResourceType, 0,              0                );</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|SerialEventRawResourceCreated]]
[[Category:Civ5 Resources API|SerialEventRawResourceCreated]]