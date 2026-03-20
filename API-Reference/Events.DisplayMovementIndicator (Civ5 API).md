{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Events}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''void''' Events.DisplayMovementIndicator<b>(</b>'''bool''' show<b>)</b></code>


'''Event Type'''
:Regular event: you can subscribe to it through <code>Events.DisplayMovementIndicator.Add(''<function handler>'')</code> or invoke it directly through <code>Events.DisplayMovementIndicator(''<arguments list>'')</code>.

'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|show:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|InGame.lua}}
:<code>UI/InGame/InGame.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0519}}<syntaxhighlight lang="lua">Events.DisplayMovementIndicator( true );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0524}}<syntaxhighlight lang="lua">Events.DisplayMovementIndicator( false );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|PathHelpManager.lua}}
:<code>UI/InGame/WorldView/PathHelpManager.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0055}}<syntaxhighlight lang="lua">Events.DisplayMovementIndicator.Add( OnDisplay );</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|DisplayMovementIndicator]]
[[Category:Civ5 Movement API|DisplayMovementIndicator]]