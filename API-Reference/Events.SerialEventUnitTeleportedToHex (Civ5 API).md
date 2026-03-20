{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Events}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''void''' Events.SerialEventUnitTeleportedToHex<b>(</b>'''unknown''' i, '''unknown''' j, {{Type5|PlayerID}} player, {{Type5|UnitID}} unitID<b>)</b></code>


'''Event Type'''
:Regular event: you can subscribe to it through <code>Events.SerialEventUnitTeleportedToHex.Add(''<function handler>'')</code> or invoke it directly through <code>Events.SerialEventUnitTeleportedToHex(''<arguments list>'')</code>.

'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|i:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|j:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|player:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|unitID:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|UnitFlagManager.lua}}
:<code>UI/InGame/UnitFlagManager.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0963}}<syntaxhighlight lang="lua">Events.SerialEventUnitTeleportedToHex.Add( OnUnitTeleported );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|UnitList.lua}}
:<code>UI/InGame/UnitList.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0089}}<syntaxhighlight lang="lua">Events.SerialEventUnitTeleportedToHex.Add( OnChangeEvent );</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|SerialEventUnitTeleportedToHex]]
[[Category:Civ5 Units API|SerialEventUnitTeleportedToHex]]