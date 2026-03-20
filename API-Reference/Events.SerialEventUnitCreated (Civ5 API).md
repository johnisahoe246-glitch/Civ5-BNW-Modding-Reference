{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Events}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''void''' Events.SerialEventUnitCreated<b>(</b>{{Type5|PlayerID}} player, {{Type5|UnitID}} unitID, '''int''' hexVec, '''int''' unitType, '''int''' cultureType, '''int''' civID, '''int''' primaryColor, '''int''' secondaryColor, '''int''' unitFlagIndex, '''int''' fogState<b>)</b></code>


'''Event Type'''
:Regular event: you can subscribe to it through <code>Events.SerialEventUnitCreated.Add(''<function handler>'')</code> or invoke it directly through <code>Events.SerialEventUnitCreated(''<arguments list>'')</code>.

'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|player:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|unitID:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|hexVec:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|unitType:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|cultureType:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|civID:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|primaryColor:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|secondaryColor:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|unitFlagIndex:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|fogState:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|UnitFlagManager.lua}}
:<code>UI/InGame/UnitFlagManager.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0898}}<syntaxhighlight lang="lua">Events.SerialEventUnitCreated.Add( OnUnitCreated );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|UnitList.lua}}
:<code>UI/InGame/UnitList.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0081}}<syntaxhighlight lang="lua">Events.SerialEventUnitCreated.Add( OnChangeEvent );</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|SerialEventUnitCreated]]
[[Category:Civ5 Units API|SerialEventUnitCreated]]