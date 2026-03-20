{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Events}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''void''' Events.ShowHexYield<b>(</b>'''int''' x, '''int''' y, '''bool''' show<b>)</b></code>


'''Event Type'''
:Regular event: you can subscribe to it through <code>Events.ShowHexYield.Add(''<function handler>'')</code> or invoke it directly through <code>Events.ShowHexYield(''<arguments list>'')</code>.

'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|x:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|y:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|show:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|YieldIconManager.lua}}
:<code>UI/InGame/YieldIconManager.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0064}}<syntaxhighlight lang="lua">Events.ShowHexYield.Add( ShowHexYield );</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|ShowHexYield]]
[[Category:Civ5 Yields API|ShowHexYield]]