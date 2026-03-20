{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Game}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''void''' Game.CycleUnits<b>(</b>'''bool''' clear, '''bool''' forward, '''bool''' workers<b>)</b></code>


'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|clear:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|forward:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|workers:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|UnitPanel.lua}}
:<code>UI/InGame/WorldView/UnitPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0692}}<syntaxhighlight lang="lua">Game.CycleUnits(true, false, false);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0702}}<syntaxhighlight lang="lua">Game.CycleUnits(true, true, false);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|CycleUnits]]
[[Category:Civ5 Units API|CycleUnits]]