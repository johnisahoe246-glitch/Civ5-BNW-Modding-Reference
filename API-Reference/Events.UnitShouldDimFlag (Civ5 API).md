{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Events}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''void''' Events.UnitShouldDimFlag<b>(</b>{{Type5|PlayerID}} player, {{Type5|UnitID}} unitID, '''int''' dim<b>)</b></code>


'''Event Type'''
:Regular event: you can subscribe to it through <code>Events.UnitShouldDimFlag.Add(''<function handler>'')</code> or invoke it directly through <code>Events.UnitShouldDimFlag(''<arguments list>'')</code>.

'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|player:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|unitID:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|dim:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|UnitFlagManager.lua}}
:<code>UI/InGame/UnitFlagManager.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1347}}<syntaxhighlight lang="lua">Events.UnitShouldDimFlag.Add( OnDimEvent );</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|UnitShouldDimFlag]]
[[Category:Civ5 Units API|UnitShouldDimFlag]]