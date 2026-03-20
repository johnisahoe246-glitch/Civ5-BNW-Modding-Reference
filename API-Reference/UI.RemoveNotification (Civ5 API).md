{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|UI}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''void''' UI.RemoveNotification<b>(</b>{{Type5|EndTurnBlockingType}} blockingNotificationIndex<b>)</b></code>


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
{{CodeLine5|0171}}<syntaxhighlight lang="lua">UI.RemoveNotification( blockingNotificationIndex );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|NotificationPanel.lua}}
:<code>UI/InGame/WorldView/NotificationPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0030}}<syntaxhighlight lang="lua">UI.RemoveNotification( Id )</syntaxhighlight>
{{CodeLine5|0031}}<syntaxhighlight lang="lua">end</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|RemoveNotification]]
[[Category:Civ5 Notification API|RemoveNotification]]