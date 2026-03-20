{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Steam}}.<br/>
This is a static method, invoke it with a dot.
}}


Adjusts where the overlay notification is displayed for the user


=Usage=
<code>'''void''' Steam.SetOverlayNotificationPosition<b>(</b>'''string''' position = nil<b>)</b></code>


'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|position:
|valign="top"| ''The position the overlay should display in.
Valid Values are: top_left, top_right, bottom_left, bottom_right''
|}


=Examples=
<syntaxhighlight lang="lua" class="civ5-example">
--Move notification to top right
Steam.SetOverlayNotificationPosition("top_right");</syntaxhighlight>


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|MainMenu.lua}}
:<code>UI/FrontEnd/MainMenu.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0110}}<syntaxhighlight lang="lua">Steam.SetOverlayNotificationPosition( "bottom_left" );</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|SetOverlayNotificationPosition]]
[[Category:Civ5 Notification API|SetOverlayNotificationPosition]]