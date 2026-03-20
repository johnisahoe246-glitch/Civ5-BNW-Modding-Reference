{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Events}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''void''' Events.InterfaceModeChanged<b>(</b>{{Type5|InterfaceMode}} oldInterfaceMode, {{Type5|InterfaceMode}} newInterfaceMode<b>)</b></code>


'''Event Type'''
:Regular event: you can subscribe to it through <code>Events.InterfaceModeChanged.Add(''<function handler>'')</code> or invoke it directly through <code>Events.InterfaceModeChanged(''<arguments list>'')</code>.

'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|oldInterfaceMode:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|newInterfaceMode:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|CityBannerManager.lua}}
:<code>UI/InGame/CityBannerManager.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1209}}<syntaxhighlight lang="lua">Events.InterfaceModeChanged.Add(OnInterfaceModeChanged);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|InGame.lua}}
:<code>UI/InGame/InGame.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0714}}<syntaxhighlight lang="lua">Events.InterfaceModeChanged.Add( OnInterfaceModeChanged );</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|InterfaceModeChanged]]