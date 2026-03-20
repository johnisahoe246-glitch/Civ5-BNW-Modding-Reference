{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Events}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''void''' Events.AddPopupTextEvent<b>(</b>{{Type5|Vector3}} worldPosition, '''unknown''' text, '''int''' delay<b>)</b></code>


'''Event Type'''
:Regular event: you can subscribe to it through <code>Events.AddPopupTextEvent.Add(''<function handler>'')</code> or invoke it directly through <code>Events.AddPopupTextEvent(''<arguments list>'')</code>.

'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|worldPosition:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|text:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|delay:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|InGame.lua}}
:<code>UI/InGame/InGame.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0924}}<syntaxhighlight lang="lua">Events.AddPopupTextEvent.Add( AddPopupText );</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|AddPopupTextEvent]]