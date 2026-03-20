{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Events}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''void''' Events.StrategicViewStateChanged<b>(</b>'''int''' strategicView, '''int''' cityBanners<b>)</b></code>


'''Event Type'''
:Regular event: you can subscribe to it through <code>Events.StrategicViewStateChanged.Add(''<function handler>'')</code> or invoke it directly through <code>Events.StrategicViewStateChanged(''<arguments list>'')</code>.

'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|strategicView:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|cityBanners:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|CityBannerManager.lua}}
:<code>UI/InGame/CityBannerManager.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1218}}<syntaxhighlight lang="lua">Events.StrategicViewStateChanged.Add(OnStrategicViewStateChanged);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|MiniMapPanel.lua}}
:<code>UI/InGame/WorldView/MiniMapPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0052}}<syntaxhighlight lang="lua">Events.StrategicViewStateChanged.Add( OnStrategicViewStateChanged );</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|StrategicViewStateChanged]]