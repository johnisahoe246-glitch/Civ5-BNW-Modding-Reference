{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Events}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''void''' Events.NotificationRemoved<b>(</b>{{Type5|CityAIFocusType}} <b>)</b></code>


'''Event Type'''
:Regular event: you can subscribe to it through <code>Events.NotificationRemoved.Add(''<function handler>'')</code> or invoke it directly through <code>Events.NotificationRemoved(''<arguments list>'')</code>.

'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|NotificationPanel.lua}}
:<code>UI/InGame/WorldView/NotificationPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0342}}<syntaxhighlight lang="lua">Events.NotificationRemoved.Add( NotificationRemoved );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TutorialEngine.lua}}
:<code>Tutorial/TutorialEngine.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0648}}<syntaxhighlight lang="lua">Events.NotificationRemoved.Add(HandleNotificationRemoved);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|NotificationRemoved]]
[[Category:Civ5 Notification API|NotificationRemoved]]