{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Events}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''void''' Events.GameplayAlertMessage<b>(</b>'''unknown''' data<b>)</b></code>


'''Event Type'''
:Regular event: you can subscribe to it through <code>Events.GameplayAlertMessage.Add(''<function handler>'')</code> or invoke it directly through <code>Events.GameplayAlertMessage(''<arguments list>'')</code>.

'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|data:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|InGame.lua}}
:<code>UI/InGame/InGame.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0397}}<syntaxhighlight lang="lua">Events.GameplayAlertMessage.Add( OnGameplayAlertMessage );</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GameplayAlertMessage]]