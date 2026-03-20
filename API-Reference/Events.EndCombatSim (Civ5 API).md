{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Events}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''void''' Events.EndCombatSim<b>(</b>{{Type5|PlayerID}} attackingPlayer, {{Type5|UnitID}} attackingUnit, '''int''' attackingUnitDamage, '''int''' attackingUnitFinalDamage, '''int''' attackingUnitMaxHitPoints, {{Type5|PlayerID}} defendingPlayer, {{Type5|UnitID}} defendingUnit, '''int''' defendingUnitDamage, '''int''' defendingUnitFinalDamage, '''int''' defendingUnitMaxHitPoints<b>)</b></code>


'''Event Type'''
:Regular event: you can subscribe to it through <code>Events.EndCombatSim.Add(''<function handler>'')</code> or invoke it directly through <code>Events.EndCombatSim(''<arguments list>'')</code>.

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
{{CodeLine5|3183}}<syntaxhighlight lang="lua">Events.EndCombatSim.Add( CombatEnded );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|UnitFlagManager.lua}}
:<code>UI/InGame/UnitFlagManager.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1541}}<syntaxhighlight lang="lua">Events.EndCombatSim.Add( OnCombatEnd );</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|EndCombatSim]]
[[Category:Civ5 Combat API|EndCombatSim]]