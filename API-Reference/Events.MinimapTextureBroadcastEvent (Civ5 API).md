{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Events}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''void''' Events.MinimapTextureBroadcastEvent<b>(</b>'''unknown''' uiHandle, '''int''' width, '''int''' height, '''unknown''' paddingX<b>)</b></code>


'''Event Type'''
:Regular event: you can subscribe to it through <code>Events.MinimapTextureBroadcastEvent.Add(''<function handler>'')</code> or invoke it directly through <code>Events.MinimapTextureBroadcastEvent(''<arguments list>'')</code>.

'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|uiHandle:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|width:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|height:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|paddingX:
|valign="top"| ''No description available.''
|}


=Source code samples=
{{PseudoH4|MiniMapPanel.lua}}
:<code>UI/InGame/WorldView/MiniMapPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0014}}<syntaxhighlight lang="lua">Events.MinimapTextureBroadcastEvent.Add( OnMinimapInfo );</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|MinimapTextureBroadcastEvent]]