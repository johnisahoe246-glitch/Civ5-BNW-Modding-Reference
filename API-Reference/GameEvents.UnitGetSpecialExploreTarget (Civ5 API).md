{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|GameEvents}}.<br/>
This is a static method, invoke it with a dot.
}}


Appears to be triggered when the 'explore' order is given, or some subset thereof. The unit structure for the relevant unit is manipulated to set the explore target.
====Listener Prototype====
listener(iPlayerID, iUnitID)
*'''iPlayerID''' The ID of the player who issued the explore order.
*'''iUnitID''' The ID of the unit the order was issued to.


=Usage=
<code>'''void''' GameEvents.UnitGetSpecialExploreTarget<b>(</b>{{Type5|PlayerID}} player, {{Type5|UnitID}} unitID<b>)</b></code>


'''Event Type'''
:Unknown

'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|player:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|unitID:
|valign="top"| ''No description available.''
|}


=Source code samples=
{{PseudoH4|TurnsRemaining.lua - DLC_02 DLC}}
:<code>DLC/DLC_02/Scenarios/NewWorldScenario/TurnsRemaining.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0576}}<syntaxhighlight lang="lua">GameEvents.UnitGetSpecialExploreTarget.Add(OnSpecialExploreRequest);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|UnitGetSpecialExploreTarget]]
[[Category:Civ5 Units API|UnitGetSpecialExploreTarget]]
[[Category:Civ5 Combat API|UnitGetSpecialExploreTarget]]