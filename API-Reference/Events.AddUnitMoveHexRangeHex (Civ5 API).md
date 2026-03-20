{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Events}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''void''' Events.AddUnitMoveHexRangeHex<b>(</b>'''float''' i, '''float''' j, '''unknown''' k, '''bool''' attackMove, '''unknown''' unitID<b>)</b></code>


'''Event Type'''
:Regular event: you can subscribe to it through <code>Events.AddUnitMoveHexRangeHex.Add(''<function handler>'')</code> or invoke it directly through <code>Events.AddUnitMoveHexRangeHex(''<arguments list>'')</code>.

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
|valign="top" style="padding-right:6px;"|attackMove:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|unitID:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|WorldView.lua}}
:<code>UI/InGame/WorldView/WorldView.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0770}}<syntaxhighlight lang="lua">Events.AddUnitMoveHexRangeHex.Add( OnAddUnitMoveHexRangeHex );</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|AddUnitMoveHexRangeHex]]
[[Category:Civ5 Units API|AddUnitMoveHexRangeHex]]
[[Category:Civ5 Movement API|AddUnitMoveHexRangeHex]]
[[Category:Civ5 Combat API|AddUnitMoveHexRangeHex]]