{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Events}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''void''' Events.SerialEventCityContinentChanged<b>(</b>'''float''' hexX, '''int''' hexY, '''int''' arg2<b>)</b></code>


'''Event Type'''
:Regular event: you can subscribe to it through <code>Events.SerialEventCityContinentChanged.Add(''<function handler>'')</code> or invoke it directly through <code>Events.SerialEventCityContinentChanged(''<arguments list>'')</code>.

'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|hexX:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|hexY:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|arg2:
|valign="top"| ''No description available.''
|}


=Source code samples=
{{PseudoH4|DebugMode.lua}}
:<code>UI/InGame/DebugMode.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0174}}<syntaxhighlight lang="lua">Events.SerialEventCityContinentChanged( g_iHexX, g_iHexY, (g_iCityContinent - 1) );</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|SerialEventCityContinentChanged]]
[[Category:Civ5 Cities API|SerialEventCityContinentChanged]]