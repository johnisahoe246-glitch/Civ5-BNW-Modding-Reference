{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Events}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''void''' Events.HexFOWStateChanged<b>(</b>{{Type5|Vector2}} hexPos, '''int''' fowType, '''bool''' wholeMap<b>)</b></code>


'''Event Type'''
:Regular event: you can subscribe to it through <code>Events.HexFOWStateChanged.Add(''<function handler>'')</code> or invoke it directly through <code>Events.HexFOWStateChanged(''<arguments list>'')</code>.

'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|hexPos:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|fowType:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|wholeMap:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|CityBannerManager.lua}}
:<code>UI/InGame/CityBannerManager.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0978}}<syntaxhighlight lang="lua">Events.HexFOWStateChanged.Add( OnHexFogEvent );</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|HexFOWStateChanged]]
[[Category:Civ5 Fog API|HexFOWStateChanged]]