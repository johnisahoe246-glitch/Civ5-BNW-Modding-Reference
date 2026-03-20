{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Events}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''void''' Events.UnitMoveQueueChanged<b>(</b>{{Type5|PlayerID}} player, {{Type5|UnitID}} unitID, '''bool''' remainingMoves<b>)</b></code>


'''Event Type'''
:Regular event: you can subscribe to it through <code>Events.UnitMoveQueueChanged.Add(''<function handler>'')</code> or invoke it directly through <code>Events.UnitMoveQueueChanged(''<arguments list>'')</code>.

'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|player:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|unitID:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|remainingMoves:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|CityBannerManager.lua}}
:<code>UI/InGame/CityBannerManager.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1176}}<syntaxhighlight lang="lua">Events.UnitMoveQueueChanged.Add( OnUnitMoveQueueChanged );</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|UnitMoveQueueChanged]]
[[Category:Civ5 Units API|UnitMoveQueueChanged]]
[[Category:Civ5 Movement API|UnitMoveQueueChanged]]