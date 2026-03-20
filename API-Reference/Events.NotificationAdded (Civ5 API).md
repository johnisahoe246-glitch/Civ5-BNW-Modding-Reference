{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Events}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''void''' Events.NotificationAdded<b>(</b>{{Type5|CityAIFocusType}} notification, {{Type5|NotificationType}} notificationType, '''string''' toolTip, '''string''' summary, '''int''' gameValue, {{Type5|TechType}} extraGameData<b>)</b></code>


'''Event Type'''
:Regular event: you can subscribe to it through <code>Events.NotificationAdded.Add(''<function handler>'')</code> or invoke it directly through <code>Events.NotificationAdded(''<arguments list>'')</code>.

'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|notification:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|notificationType:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|toolTip:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|summary:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|gameValue:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|extraGameData:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|DiploCorner.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/WorldView/DiploCorner.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0422}}<syntaxhighlight lang="lua">Events.NotificationAdded.Add(HandleNotificationAdded);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|NotificationPanel.lua}}
:<code>UI/InGame/WorldView/NotificationPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0293}}<syntaxhighlight lang="lua">Events.NotificationAdded.Add( OnNotificationAdded );</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|NotificationAdded]]
[[Category:Civ5 Notification API|NotificationAdded]]