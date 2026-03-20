{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Events}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''void''' Events.UnitHexHighlight<b>(</b>'''float''' i, '''int''' j, '''unknown''' k, '''bool''' on, '''int''' unitId<b>)</b></code>


'''Event Type'''
:Regular event: you can subscribe to it through <code>Events.UnitHexHighlight.Add(''<function handler>'')</code> or invoke it directly through <code>Events.UnitHexHighlight(''<arguments list>'')</code>.

'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|i:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|j:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|k:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|on:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|unitId:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|InGame.lua}}
:<code>UI/InGame/InGame.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0975}}<syntaxhighlight lang="lua">Events.UnitHexHighlight.Add( OnUnitHexHighlight )</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0980}}<syntaxhighlight lang="lua">function RequestYieldDisplay()</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|UnitHexHighlight]]
[[Category:Civ5 Units API|UnitHexHighlight]]