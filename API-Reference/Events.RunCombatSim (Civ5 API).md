{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Events}}.<br/>
This is a static method, invoke it with a dot.
}}


This event is triggered every time a unit begins combat. The event will trigger off of any type of combat including but not limited to Melee, Ranged, Bombard, Air Missions and Nuclear. It has not yet been tested whether or not the triggering unit needs to be seen by the (human) player.


=Usage=
<code>'''void''' Events.RunCombatSim<b>(</b>{{Type5|PlayerID}} attackingPlayer, {{Type5|UnitID}} attackingUnit, '''int''' attackingUnitDamage, '''int''' attackingUnitFinalDamage, '''int''' attackingUnitMaxHitPoints, {{Type5|PlayerID}} defendingPlayer, {{Type5|UnitID}} defendingUnit, '''int''' defendingUnitDamage, '''int''' defendingUnitFinalDamage, '''int''' defendingUnitMaxHitPoints<b>)</b></code>


'''Event Type'''
:Regular event: you can subscribe to it through <code>Events.RunCombatSim.Add(''<function handler>'')</code> or invoke it directly through <code>Events.RunCombatSim(''<arguments list>'')</code>.

'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|attackingPlayer:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|attackingUnit:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|attackingUnitDamage:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|attackingUnitFinalDamage:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|attackingUnitMaxHitPoints:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|defendingPlayer:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|defendingUnit:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|defendingUnitDamage:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|defendingUnitFinalDamage:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|defendingUnitMaxHitPoints:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|TutorialChecks.lua}}
:<code>Tutorial/TutorialChecks.lua</code>
:{{CodeBegin5}}
{{CodeLine5|3153}}<syntaxhighlight lang="lua">Events.RunCombatSim.Add( CombatStarted );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|UnitFlagManager.lua}}
:<code>UI/InGame/UnitFlagManager.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1505}}<syntaxhighlight lang="lua">Events.RunCombatSim.Add( OnCombatBegin );</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|RunCombatSim]]
[[Category:Civ5 Combat API|RunCombatSim]]