{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Events}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''void''' Events.UIPathFinderUpdate<b>(</b>'''unknown''' data<b>)</b></code>


'''Event Type'''
:Regular event: you can subscribe to it through <code>Events.UIPathFinderUpdate.Add(''<function handler>'')</code> or invoke it directly through <code>Events.UIPathFinderUpdate(''<arguments list>'')</code>.

'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|data:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|PathHelpManager.lua}}
:<code>UI/InGame/WorldView/PathHelpManager.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0024}}<syntaxhighlight lang="lua">Events.UIPathFinderUpdate.Add( OnPath );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|WorldView.lua}}
:<code>UI/InGame/WorldView/WorldView.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0740}}<syntaxhighlight lang="lua">Events.UIPathFinderUpdate.Add( OnUIPathFinderUpdate );</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|UIPathFinderUpdate]]
[[Category:Civ5 Movement API|UIPathFinderUpdate]]