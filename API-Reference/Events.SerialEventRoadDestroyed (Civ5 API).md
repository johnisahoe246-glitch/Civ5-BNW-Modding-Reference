{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Events}}.<br/>
This is a static method, invoke it with a dot.
}}


This event is triggered whenever a route is removed (triggers on railroads despite the name). Does not trigger when pillaging, only for the worker action


=Usage=
<code>'''void''' Events.SerialEventRoadDestroyed<b>(</b>'''int''' hexX, '''int''' hexY<b>)</b></code>


'''Event Type'''
:Regular event: you can subscribe to it through <code>Events.SerialEventRoadDestroyed.Add(''<function handler>'')</code> or invoke it directly through <code>Events.SerialEventRoadDestroyed(''<arguments list>'')</code>.

'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|hexX:
|valign="top"| ''Hex x-coordinate of the tile the road was destroyed on which can be converted to map grid coordinates with the {{Type5|ToGridFromHex}} function''
|-
|valign="top" style="padding-right:6px;"|hexY:
|valign="top"| ''Hex y-coordinate of the tile the road was destroyed on which can be converted to map grid coordinates with the {{Type5|ToGridFromHex}} function''
|}


=Source code samples=
{{PseudoH4|DebugMode.lua}}
:<code>UI/InGame/DebugMode.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0426}}<syntaxhighlight lang="lua">Events.SerialEventRoadDestroyed( g_iHexX, g_iHexY );</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|SerialEventRoadDestroyed]]