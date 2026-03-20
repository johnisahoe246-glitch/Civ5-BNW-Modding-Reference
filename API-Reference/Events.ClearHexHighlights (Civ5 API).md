{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Events}}.<br/>
This is a static method, invoke it with a dot.
}}


Triggers when highlights are cleared that were set by {{Func5|Events|SerialEventHexHighlight}}. Can be invoked from Lua, which is the common usage.


=Usage=
<code>'''void''' Events.ClearHexHighlights<b>(</b><b>)</b></code>


'''Event Type'''
:Regular event: you can subscribe to it through <code>Events.ClearHexHighlights.Add(''<function handler>'')</code> or invoke it directly through <code>Events.ClearHexHighlights(''<arguments list>'')</code>.



=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|InGame.lua}}
:<code>UI/InGame/InGame.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0497}}<syntaxhighlight lang="lua">Events.ClearHexHighlights();</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|ClearHexHighlights]]