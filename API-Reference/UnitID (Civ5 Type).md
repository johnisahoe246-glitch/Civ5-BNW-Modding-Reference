{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|ID.png|The <code>UnitID</code> pseudo-type is actually a regular '''integer'''. Pseudo-types do not exist in Lua, they only serve a documentation purpose on the wiki!}}


=Used by=
{|cellspacing="4" cellpadding="0" width="100%" style="background-color:#F0F0F0"
<!-- 
UNITMOVING
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Func5|UnitMoving}}<b>(</b>{{Type5|PlayerID}} player, {{Type5|UnitID}} unit<b>)</b></code>
<!-- 
SETVOIDS
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Button}}:{{Func5|UIElement|SetVoids}}<b>(</b>{{Type5|PlayerID}} building, {{Type5|UnitID}} addToList<b>)</b></code>
<!-- 
ENDCOMBATSIM
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Events}}.{{Func5|Events|EndCombatSim}}<b>(</b>{{Type5|PlayerID}} attackingPlayer, {{Type5|UnitID}} attackingUnit, '''int''' attackingUnitDamage, '''int''' attackingUnitFinalDamage, '''int''' attackingUnitMaxHitPoints, {{Type5|PlayerID}} defendingPlayer, {{Type5|UnitID}} defendingUnit, '''int''' defendingUnitDamage, '''int''' defendingUnitFinalDamage, '''int''' defendingUnitMaxHitPoints<b>)</b></code>
<!-- 
LOCALMACHINEUNITPOSITIONCHANGED
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Events}}.{{Func5|Events|LocalMachineUnitPositionChanged}}<b>(</b>{{Type5|PlayerID}} player, {{Type5|UnitID}} unitID, {{Type5|Vector3}} unitPosition<b>)</b></code>
<!-- 
RUNCOMBATSIM
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Events}}.{{Func5|Events|RunCombatSim}}<b>(</b>{{Type5|PlayerID}} attackingPlayer, {{Type5|UnitID}} attackingUnit, '''int''' attackingUnitDamage, '''int''' attackingUnitFinalDamage, '''int''' attackingUnitMaxHitPoints, {{Type5|PlayerID}} defendingPlayer, {{Type5|UnitID}} defendingUnit, '''int''' defendingUnitDamage, '''int''' defendingUnitFinalDamage, '''int''' defendingUnitMaxHitPoints<b>)</b></code>
<!-- 
SERIALEVENTUNITCREATED
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Events}}.{{Func5|Events|SerialEventUnitCreated}}<b>(</b>{{Type5|PlayerID}} player, {{Type5|UnitID}} unitID, '''int''' hexVec, '''int''' unitType, '''int''' cultureType, '''int''' civID, '''int''' primaryColor, '''int''' secondaryColor, '''int''' unitFlagIndex, '''int''' fogState<b>)</b></code>
<!-- 
SERIALEVENTUNITDESTROYED
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Events}}.{{Func5|Events|SerialEventUnitDestroyed}}<b>(</b>{{Type5|PlayerID}} player, {{Type5|UnitID}} unitID<b>)</b></code>
<!-- 
SERIALEVENTUNITSETDAMAGE
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Events}}.{{Func5|Events|SerialEventUnitSetDamage}}<b>(</b>{{Type5|PlayerID}} player, {{Type5|UnitID}} unitID, '''int''' damage, '''int''' previousDamage<b>)</b></code>
<!-- 
SERIALEVENTUNITTELEPORTEDTOHEX
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Events}}.{{Func5|Events|SerialEventUnitTeleportedToHex}}<b>(</b>'''unknown''' i, '''unknown''' j, {{Type5|PlayerID}} player, {{Type5|UnitID}} unitID<b>)</b></code>
<!-- 
SHOWATTACKTARGETS
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Events}}.{{Func5|Events|ShowAttackTargets}}<b>(</b>{{Type5|PlayerID}} player, {{Type5|UnitID}} arg1<b>)</b></code>
<!-- 
SHOWMOVEMENTRANGE
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Events}}.{{Func5|Events|ShowMovementRange}}<b>(</b>{{Type5|PlayerID}} player, {{Type5|UnitID}} arg1<b>)</b></code>
<!-- 
UNITACTIONCHANGED
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Events}}.{{Func5|Events|UnitActionChanged}}<b>(</b>{{Type5|PlayerID}} player, {{Type5|UnitID}} unitID<b>)</b></code>
<!-- 
UNITEMBARK
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Events}}.{{Func5|Events|UnitEmbark}}<b>(</b>{{Type5|PlayerID}} player, {{Type5|UnitID}} unitID<b>)</b></code>
<!-- 
UNITGARRISON
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Events}}.{{Func5|Events|UnitGarrison}}<b>(</b>{{Type5|PlayerID}} player, {{Type5|UnitID}} unitID, '''int''' garrisoned<b>)</b></code>
<!-- 
UNITMARKTHREATENING
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Events}}.{{Func5|Events|UnitMarkThreatening}}<b>(</b>{{Type5|PlayerID}} player, {{Type5|UnitID}} unitID, '''bool''' mark<b>)</b></code>
<!-- 
UNITMEMBERCOMBATSTATECHANGED
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Events}}.{{Func5|Events|UnitMemberCombatStateChanged}}<b>(</b>{{Type5|PlayerID}} player, {{Type5|UnitID}} unitID, '''int''' memberID, '''unknown''' stateID<b>)</b></code>
<!-- 
UNITMEMBERCOMBATTARGETCHANGED
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Events}}.{{Func5|Events|UnitMemberCombatTargetChanged}}<b>(</b>{{Type5|PlayerID}} player, {{Type5|UnitID}} unitID, '''int''' memberID, '''unknown''' targetPlayerID, '''unknown''' targetUnitID, '''int''' targetMemberID<b>)</b></code>
<!-- 
UNITMEMBEROVERLAYADD
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Events}}.{{Func5|Events|UnitMemberOverlayAdd}}<b>(</b>{{Type5|PlayerID}} player, {{Type5|UnitID}} unitID, '''int''' memberID, '''unknown''' position<b>)</b></code>
<!-- 
UNITMEMBEROVERLAYREMOVE
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Events}}.{{Func5|Events|UnitMemberOverlayRemove}}<b>(</b>{{Type5|PlayerID}} player, {{Type5|UnitID}} unitID, '''int''' memberID<b>)</b></code>
<!-- 
UNITMEMBEROVERLAYSHOWHIDE
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Events}}.{{Func5|Events|UnitMemberOverlayShowHide}}<b>(</b>{{Type5|PlayerID}} player, {{Type5|UnitID}} unitID, '''int''' memberID, '''bool''' show<b>)</b></code>
<!-- 
UNITMEMBERPOSITIONCHANGED
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Events}}.{{Func5|Events|UnitMemberPositionChanged}}<b>(</b>{{Type5|PlayerID}} player, {{Type5|UnitID}} unitID, '''int''' memberID, '''unknown''' unitPosition<b>)</b></code>
<!-- 
UNITMOVEQUEUECHANGED
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Events}}.{{Func5|Events|UnitMoveQueueChanged}}<b>(</b>{{Type5|PlayerID}} player, {{Type5|UnitID}} unitID, '''bool''' remainingMoves<b>)</b></code>
<!-- 
UNITSELECTIONCHANGED
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Events}}.{{Func5|Events|UnitSelectionChanged}}<b>(</b>{{Type5|PlayerID}} player, {{Type5|UnitID}} u, '''float''' hexX, '''float''' hexY, '''int''' k, '''bool''' isSelected, '''bool''' arg6<b>)</b></code>
<!-- 
UNITSHOULDDIMFLAG
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Events}}.{{Func5|Events|UnitShouldDimFlag}}<b>(</b>{{Type5|PlayerID}} player, {{Type5|UnitID}} unitID, '''int''' dim<b>)</b></code>
<!-- 
UNITSTATECHANGEDETECTED
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Events}}.{{Func5|Events|UnitStateChangeDetected}}<b>(</b>{{Type5|PlayerID}} player, {{Type5|UnitID}} unitID, '''int''' fogState<b>)</b></code>
<!-- 
UNITVISIBILITYCHANGED
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Events}}.{{Func5|Events|UnitVisibilityChanged}}<b>(</b>{{Type5|PlayerID}} player, {{Type5|UnitID}} unitID, '''bool''' visible, '''bool''' checkFlag, '''unknown''' blendTime<b>)</b></code>
<!-- 
SELECTIONLISTGAMENETMESSAGE
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Game}}.{{Func5|Game|SelectionListGameNetMessage}}<b>(</b>{{Type5|GameMessageType}} message, '''int''' data2 = -1, {{Type5|BuildActionType}} data3 = -1, {{Type5|UnitID}} data4 = -1, '''int''' flags = 0, '''bool''' alt = false, '''bool''' shift = false<b>)</b></code>
<!-- 
UNITGETSPECIALEXPLORETARGET
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|GameEvents}}.{{Func5|GameEvents|UnitGetSpecialExploreTarget}}<b>(</b>{{Type5|PlayerID}} player, {{Type5|UnitID}} unitID<b>)</b></code>
<!-- 
UNITSETXY
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|GameEvents}}.{{Func5|GameEvents|UnitSetXY}}<b>(</b>{{Type5|PlayerID}} player, {{Type5|UnitID}} unit, '''int''' x, '''int''' y<b>)</b></code>
<!-- 
SENDGIFTUNIT
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Network}}.{{Func5|Network|SendGiftUnit}}<b>(</b>'''int''' giftedPlayer, {{Type5|UnitID}} unitIndex<b>)</b></code>
<!-- 
SENDRENAMEUNIT
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Network}}.{{Func5|Network|SendRenameUnit}}<b>(</b>{{Type5|UnitID}} arg0, '''string''' arg1<b>)</b></code>
<!-- 
SENDRETURNCIVILIAN
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Network}}.{{Func5|Network|SendReturnCivilian}}<b>(</b>'''bool''' arg0, '''int''' giftedPlayer, {{Type5|UnitID}} unitIndex<b>)</b></code>
<!-- 
GETUNITBYID
-->
|-
|align="right" width="200" |<code>{{Type5|Unit}}</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|GetUnitByID}}<b>(</b>{{Type5|UnitID}} unit<b>)</b></code>
<!-- 
GETUNIT
-->
|-
|align="right" width="200" |<code>{{Type5|Unit}}</code>
|style="padding-left:6px" |<code>{{Type5|Plot}}:{{Func5|Plot|GetUnit}}<b>(</b>{{Type5|UnitID}} id<b>)</b></code>
<!-- 
GETID
-->
|-
|align="right" width="200" |<code>{{Type5|UnitID}}</code>
|style="padding-left:6px" |<code>{{Type5|Unit}}:{{Func5|Unit|GetID}}<b>(</b><!-- No arguments --><b>)</b></code>
|}




{{Civ5 API Footer}}
[[Category:Civ5 Types|UnitID]]