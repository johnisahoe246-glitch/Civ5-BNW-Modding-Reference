{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Events}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''void''' Events.HexYieldMightHaveChanged<b>(</b>'''int''' gridX, '''int''' gridY<b>)</b></code>


'''Event Type'''
:Regular event: you can subscribe to it through <code>Events.HexYieldMightHaveChanged.Add(''<function handler>'')</code> or invoke it directly through <code>Events.HexYieldMightHaveChanged(''<arguments list>'')</code>.

'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|gridX:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|gridY:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|YieldIconManager.lua}}
:<code>UI/InGame/YieldIconManager.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0269}}<syntaxhighlight lang="lua">Events.HexYieldMightHaveChanged.Add( OnYieldChangeEvent );</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|HexYieldMightHaveChanged]]
[[Category:Civ5 Yields API|HexYieldMightHaveChanged]]