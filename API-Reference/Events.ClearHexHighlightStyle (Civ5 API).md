{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Events}}.<br/>
This is a static method, invoke it with a dot.
}}


Triggers when a highlighting style that was activated by {{Func5|Events|SerialEventHexHighlight}} is cleared. Can be invoked from Lua, which is the common usage.


=Usage=
<code>'''void''' Events.ClearHexHighlightStyle<b>(</b>'''string''' highlightStyle<b>)</b></code>


'''Event Type'''
:Regular event: you can subscribe to it through <code>Events.ClearHexHighlightStyle.Add(''<function handler>'')</code> or invoke it directly through <code>Events.ClearHexHighlightStyle(''<arguments list>'')</code>.

'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|highlightStyle:
|valign="top"| ''Highlighting style to clear. Known highlighting styles are: "MovementRangeBorder", "AMRBorder", "FireRangeBorder", "ValidFireTargetBorder"''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|InGame.lua}}
:<code>UI/InGame/InGame.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0501}}<syntaxhighlight lang="lua">Events.ClearHexHighlightStyle(pathBorderStyle);</syntaxhighlight>
{{CodeLine5|0502}}<syntaxhighlight lang="lua">Events.ClearHexHighlightStyle(attackPathBorderStyle);</syntaxhighlight>
{{CodeLine5|0503}}<syntaxhighlight lang="lua">Events.ClearHexHighlightStyle(genericUnitHexBorder);</syntaxhighlight>
{{CodeLine5|0504}}<syntaxhighlight lang="lua">Events.ClearHexHighlightStyle("FireRangeBorder");</syntaxhighlight>
{{CodeLine5|0505}}<syntaxhighlight lang="lua">Events.ClearHexHighlightStyle("GroupBorder");</syntaxhighlight>
{{CodeLine5|0506}}<syntaxhighlight lang="lua">Events.ClearHexHighlightStyle("ValidFireTargetBorder");</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|ClearHexHighlightStyle]]