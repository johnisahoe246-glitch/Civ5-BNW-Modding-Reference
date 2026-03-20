{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Events}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''void''' Events.SerialEventEraChanged<b>(</b>'''int''' arg0, {{Type5|PlayerID}} currPlayer<b>)</b></code>


'''Event Type'''
:Regular event: you can subscribe to it through <code>Events.SerialEventEraChanged.Add(''<function handler>'')</code> or invoke it directly through <code>Events.SerialEventEraChanged(''<arguments list>'')</code>.

'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|arg0:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|currPlayer:
|valign="top"| ''No description available.''
|}


=Source code samples=
{{PseudoH4|DebugMode.lua}}
:<code>UI/InGame/DebugMode.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0152}}<syntaxhighlight lang="lua">Events.SerialEventEraChanged( g_iCityEra-1, g_iCurrPlayer );</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|SerialEventEraChanged]]