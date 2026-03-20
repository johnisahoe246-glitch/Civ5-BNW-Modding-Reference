{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|UI}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''void''' UI.ActivateNotification<b>(</b>{{Type5|PlayerID}} blockingNotificationIndex<b>)</b></code>


'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|blockingNotificationIndex:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|ActionInfoPanel.lua}}
:<code>UI/InGame/WorldView/ActionInfoPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0103}}<syntaxhighlight lang="lua">UI.ActivateNotification(blockingNotificationIndex);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|NotificationLogPopup.lua}}
:<code>UI/InGame/Popups/NotificationLogPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0079}}<syntaxhighlight lang="lua">UI.ActivateNotification(id);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|NotificationPanel.lua}}
:<code>UI/InGame/WorldView/NotificationPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0023}}<syntaxhighlight lang="lua">UI.ActivateNotification( Id )</syntaxhighlight>
{{CodeLine5|0024}}<syntaxhighlight lang="lua">end</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|ActivateNotification]]
[[Category:Civ5 Notification API|ActivateNotification]]