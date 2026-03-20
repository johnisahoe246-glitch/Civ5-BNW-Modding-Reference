{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|UI}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''void''' UI.SelectUnit<b>(</b>{{Type5|Unit}} v<b>)</b></code>


'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|v:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|ActionInfoPanel.lua}}
:<code>UI/InGame/WorldView/ActionInfoPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0109}}<syntaxhighlight lang="lua">UI.SelectUnit(v);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0122}}<syntaxhighlight lang="lua">UI.SelectUnit(pUnit);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TutorialEngine.lua}}
:<code>Tutorial/TutorialEngine.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0467}}<syntaxhighlight lang="lua">UI.SelectUnit(unit);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|SelectUnit]]
[[Category:Civ5 Units API|SelectUnit]]