{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Events}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''void''' Events.LocalMachineAppUpdate<b>(</b>'''unknown''' tickCount, '''int''' timeIncrement<b>)</b></code>


'''Event Type'''
:Regular event: you can subscribe to it through <code>Events.LocalMachineAppUpdate.Add(''<function handler>'')</code> or invoke it directly through <code>Events.LocalMachineAppUpdate(''<arguments list>'')</code>.

'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|tickCount:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|timeIncrement:
|valign="top"| ''No description available.''
|}


=Source code samples=
{{PseudoH4|TutorialEngine.lua}}
:<code>Tutorial/TutorialEngine.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0642}}<syntaxhighlight lang="lua">Events.LocalMachineAppUpdate.Add(HandleAppUpdate);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|LocalMachineAppUpdate]]