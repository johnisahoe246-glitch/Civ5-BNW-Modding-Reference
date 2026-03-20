{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Events}}.<br/>
This is a static method, invoke it with a dot.
}}


This event is triggered every time the flag of a certain unit is selected.


=Usage=
<code>'''void''' Events.SerialEventUnitFlagSelected<b>(</b>{{Type5|PlayerID}} player, {{Type5|HandicapType}} unit<b>)</b></code>


'''Event Type'''
:Regular event: you can subscribe to it through <code>Events.SerialEventUnitFlagSelected.Add(''<function handler>'')</code> or invoke it directly through <code>Events.SerialEventUnitFlagSelected(''<arguments list>'')</code>.

'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|player:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|unit:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|MilitaryOverview.lua}}
:<code>UI/InGame/Popups/MilitaryOverview.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0073}}<syntaxhighlight lang="lua">Events.SerialEventUnitFlagSelected( Game:GetActivePlayer(), unitID );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|UnitFlagManager.lua}}
:<code>UI/InGame/UnitFlagManager.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1161}}<syntaxhighlight lang="lua">Events.SerialEventUnitFlagSelected( playerID, unitID );</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|SerialEventUnitFlagSelected]]
[[Category:Civ5 Units API|SerialEventUnitFlagSelected]]