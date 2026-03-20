{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



= Usage =
This object exposes events designed to make the UI react to data changes. You may try to use them to implement gameplay changes but be aware that those events may not be fired in circumstances where the UI do not need it. For example the events used by the city screen may not be fired for cities controlled by the AI.


=Static Events=
Events can be subscribed by using <code>Events.SomeEvent.Add(SomeFunction)</code>. Regular events can also be fired through a '''dot''' by using <code>Events.SomeEvent(&lt;args&gt;)</code>. This will invoke all subscribers with the provided arguments.<br/>
==A==
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
ACTIVEPLAYERTURNEND
-->
|-
{{FuncInfos5|yes  |yes  |yes|Fires on the turn end of the active player. The active player is the player playing on the local machine. In other words, this fires whenever your turn end. Compare to Events.ActivePlayerTurnStart Note: This event does not fire when using Autoplay.}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Events|ActivePlayerTurnEnd}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ACTIVEPLAYERTURNSTART
-->
|-
{{FuncInfos5|yes  |yes  |yes|Fires on the turn start of the active player. The active player is the player playing on the local machine. In other words, this fires whenever your turn starts. Compare to Events.ActivePlayerTurnEnd Note: This event does not fire when using Autoplay.}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Events|ActivePlayerTurnStart}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ADDPOPUPTEXTEVENT
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Events|AddPopupTextEvent}}<b>(</b>{{Type5|Vector3}} worldPosition, '''unknown''' text, '''int''' delay<b>)</b></code>
<!-- 
ADDUNITMOVEHEXRANGEHEX
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Events|AddUnitMoveHexRangeHex}}<b>(</b>'''float''' i, '''float''' j, '''unknown''' k, '''bool''' attackMove, '''unknown''' unitID<b>)</b></code>
<!-- 
ADVISORDISPLAYHIDE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Events|AdvisorDisplayHide}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ADVISORDISPLAYSHOW
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Events|AdvisorDisplayShow}}<b>(</b>{{Type5|AdvisorEventInfo}} info<b>)</b></code>
<!-- 
AFTERMODSACTIVATE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Events|AfterModsActivate}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
AFTERMODSDEACTIVATE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Events|AfterModsDeactivate}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
AILEADERMESSAGE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Events|AILeaderMessage}}<b>(</b>{{Type5|PlayerID}} player, {{Type5|DiploUIStateType}} diploUIState, '''string''' leaderMessage, '''int''' animationAction, '''int''' data1<b>)</b></code>
<!-- 
AUDIODEBUGCHANGEMUSIC
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Events|AudioDebugChangeMusic}}<b>(</b>'''bool''' arg0, '''bool''' arg1, '''bool''' arg2<b>)</b></code>
<!-- 
AUDIOPLAY2DSOUND
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Events|AudioPlay2DSound}}<b>(</b>'''string''' audio<b>)</b></code>
|}

==B==
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
BUILDINGLIBRARYSWAP
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Events|BuildingLibrarySwap}}<b>(</b>'''int''' assetCulture, '''int''' assetEra<b>)</b></code>
|}

==C==
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
CAMERASTARTPITCHINGDOWN
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Events|CameraStartPitchingDown}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
CAMERASTARTPITCHINGUP
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Events|CameraStartPitchingUp}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
CAMERASTARTROTATINGCCW
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Events|CameraStartRotatingCCW}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
CAMERASTARTROTATINGCW
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Events|CameraStartRotatingCW}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
CAMERASTOPPITCHINGDOWN
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Events|CameraStopPitchingDown}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
CAMERASTOPPITCHINGUP
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Events|CameraStopPitchingUp}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
CAMERASTOPROTATINGCCW
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Events|CameraStopRotatingCCW}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
CAMERASTOPROTATINGCW
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Events|CameraStopRotatingCW}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
CAMERAVIEWCHANGED
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Events|CameraViewChanged}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
CLEARDIPLOMACYTRADETABLE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Events|ClearDiplomacyTradeTable}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
CLEARHEXHIGHLIGHTS
-->
|-
{{FuncInfos5|yes  |yes  |yes|Triggers when highlights are cleared that were set by Events.SerialEventHexHighlight. Can be invoked from Lua, which is the common usage.}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Events|ClearHexHighlights}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
CLEARHEXHIGHLIGHTSTYLE
-->
|-
{{FuncInfos5|yes  |yes  |yes|Triggers when a highlighting style that was activated by Events.SerialEventHexHighlight is cleared. Can be invoked from Lua, which is the common usage.}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Events|ClearHexHighlightStyle}}<b>(</b>'''string''' highlightStyle<b>)</b></code>
<!-- 
CLEARUNITMOVEHEXRANGE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Events|ClearUnitMoveHexRange}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
CONNECTEDTONETWORKHOST
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Events|ConnectedToNetworkHost}}<b>(</b>{{Type5|PlayerID}} player<b>)</b></code>
|}

==D==
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
DISPLAYMOVEMENTINDICATOR
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Events|DisplayMovementIndicator}}<b>(</b>'''bool''' show<b>)</b></code>
|}

==E==
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
ENDCOMBATSIM
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Events|EndCombatSim}}<b>(</b>{{Type5|PlayerID}} attackingPlayer, {{Type5|UnitID}} attackingUnit, '''int''' attackingUnitDamage, '''int''' attackingUnitFinalDamage, '''int''' attackingUnitMaxHitPoints, {{Type5|PlayerID}} defendingPlayer, {{Type5|UnitID}} defendingUnit, '''int''' defendingUnitDamage, '''int''' defendingUnitFinalDamage, '''int''' defendingUnitMaxHitPoints<b>)</b></code>
<!-- 
ENDGAMESHOW
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Events|EndGameShow}}<b>(</b>{{Type5|EndGameType}} type, {{Type5|TeamID}} team<b>)</b></code>
<!-- 
ENDTURNBLOCKINGCHANGED
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Events|EndTurnBlockingChanged}}<b>(</b>{{Type5|EndTurnBlockingType}} prevEndTurnBlockingType, {{Type5|EndTurnBlockingType}} newEndTurnBlockingType<b>)</b></code>
<!-- 
ENDTURNTIMERUPDATE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Events|EndTurnTimerUpdate}}<b>(</b>'''int''' percentComplete<b>)</b></code>
<!-- 
EVENTOPENOPTIONSSCREEN
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Events|EventOpenOptionsScreen}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
EVENTPOLICIESDIRTY
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Events|EventPoliciesDirty}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
EXITTOMAINMENU
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Events|ExitToMainMenu}}<b>(</b><!-- No arguments --><b>)</b></code>
|}

==F==
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
FRONTENDPOPUP
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Events|FrontEndPopup}}<b>(</b>'''string''' string<b>)</b></code>
|}

==G==
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
GAMEMESSAGECHAT
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Events|GameMessageChat}}<b>(</b>{{Type5|PlayerID}} fromPlayer, {{Type5|PlayerID}} toPlayer, '''string''' text, {{Type5|ChatTargetType}} targetType<b>)</b></code>
<!-- 
GAMEOPTIONSCHANGED
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Events|GameOptionsChanged}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GAMEPLAYALERTMESSAGE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Events|GameplayAlertMessage}}<b>(</b>'''unknown''' data<b>)</b></code>
<!-- 
GAMEPLAYFX
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Events|GameplayFX}}<b>(</b>'''float''' arg0, '''float''' arg1, '''int''' arg2<b>)</b></code>
<!-- 
GAMEPLAYSETACTIVEPLAYER
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Events|GameplaySetActivePlayer}}<b>(</b>{{Type5|PlayerID}} activePlayer, '''int''' prevActivePlayer<b>)</b></code>
<!-- 
GENERICWORLDANCHOR
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Events|GenericWorldAnchor}}<b>(</b>{{Type5|GenericWorldAnchorType}} type, '''bool''' show, '''int''' plotX, '''int''' plotY, {{Type5|FeatureType}} data1 = nil<b>)</b></code>
<!-- 
GOTOPEDIAHOMEPAGE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Events|GoToPediaHomePage}}<b>(</b>{{Type5|ImprovementType}} homePage<b>)</b></code>
<!-- 
GRAPHICSOPTIONSCHANGED
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Events|GraphicsOptionsChanged}}<b>(</b><!-- No arguments --><b>)</b></code>
|}

==H==
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
HEXFOWSTATECHANGED
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Events|HexFOWStateChanged}}<b>(</b>{{Type5|Vector2}} hexPos, '''int''' fowType, '''bool''' wholeMap<b>)</b></code>
<!-- 
HEXYIELDMIGHTHAVECHANGED
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Events|HexYieldMightHaveChanged}}<b>(</b>'''int''' gridX, '''int''' gridY<b>)</b></code>
|}

==I==
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
INITCITYRANGESTRIKE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Events|InitCityRangeStrike}}<b>(</b>{{Type5|PlayerID}} Player, {{Type5|CityID}} CityID<b>)</b></code>
<!-- 
INSTALLEDMODSUPDATED
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Events|InstalledModsUpdated}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
INTERFACEMODECHANGED
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Events|InterfaceModeChanged}}<b>(</b>{{Type5|InterfaceMode}} oldInterfaceMode, {{Type5|InterfaceMode}} newInterfaceMode<b>)</b></code>
|}

==K==
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
KEYUPEVENT
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Events|KeyUpEvent}}<b>(</b>{{Type5|KeyType}} wParam<b>)</b></code>
|}

==L==
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
LANDMARKLIBRARYSWAP
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Events|LandmarkLibrarySwap}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
LEAVINGLEADERVIEWMODE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Events|LeavingLeaderViewMode}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
LOADSCREENCLOSE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Events|LoadScreenClose}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
LOCALMACHINEAPPUPDATE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Events|LocalMachineAppUpdate}}<b>(</b>'''unknown''' tickCount, '''int''' timeIncrement<b>)</b></code>
<!-- 
LOCALMACHINEUNITPOSITIONCHANGED
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Events|LocalMachineUnitPositionChanged}}<b>(</b>{{Type5|PlayerID}} player, {{Type5|UnitID}} unitID, {{Type5|Vector3}} unitPosition<b>)</b></code>
|}

==M==
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
MINIMAPCLICKEDEVENT
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Events|MinimapClickedEvent}}<b>(</b>'''int''' x, '''int''' y<b>)</b></code>
<!-- 
MINIMAPTEXTUREBROADCASTEVENT
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Events|MinimapTextureBroadcastEvent}}<b>(</b>'''unknown''' uiHandle, '''int''' width, '''int''' height, '''unknown''' paddingX<b>)</b></code>
<!-- 
MULTIPLAYERCONNECTIONFAILED
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Events|MultiplayerConnectionFailed}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
MULTIPLAYERGAMEABANDONED
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Events|MultiplayerGameAbandoned}}<b>(</b>{{Type5|NetKicked}} reason<b>)</b></code>
<!-- 
MULTIPLAYERGAMEINVITE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Events|MultiplayerGameInvite}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
MULTIPLAYERGAMELAUNCHED
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Events|MultiplayerGameLaunched}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
MULTIPLAYERGAMELISTCLEAR
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Events|MultiplayerGameListClear}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
MULTIPLAYERGAMELISTCOMPLETE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Events|MultiplayerGameListComplete}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
MULTIPLAYERGAMEPLAYERDISCONNECTED
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Events|MultiplayerGamePlayerDisconnected}}<b>(</b>{{Type5|PlayerID}} player<b>)</b></code>
<!-- 
MULTIPLAYERGAMEPLAYERUPDATED
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Events|MultiplayerGamePlayerUpdated}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
MULTIPLAYERJOINROOMCOMPLETE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Events|MultiplayerJoinRoomComplete}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
MULTIPLAYERJOINROOMFAILED
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Events|MultiplayerJoinRoomFailed}}<b>(</b>{{Type5|NetError}} extendedError, '''unknown''' aExtendedErrorText<b>)</b></code>
<!-- 
MULTIPLAYERPINGTIMESCHANGED
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Events|MultiplayerPingTimesChanged}}<b>(</b><!-- No arguments --><b>)</b></code>
|}

==N==
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
NATURALWONDERREVEALED
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Events|NaturalWonderRevealed}}<b>(</b>'''float''' i, '''int''' j<b>)</b></code>
<!-- 
NOTIFICATIONADDED
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Events|NotificationAdded}}<b>(</b>{{Type5|CityAIFocusType}} notification, {{Type5|NotificationType}} notificationType, '''string''' toolTip, '''string''' summary, '''int''' gameValue, {{Type5|TechType}} extraGameData<b>)</b></code>
<!-- 
NOTIFICATIONREMOVED
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Events|NotificationRemoved}}<b>(</b>{{Type5|CityAIFocusType}} <b>)</b></code>
|}

==O==
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
OPENINFOCORNER
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Events|OpenInfoCorner}}<b>(</b>{{Type5|InfoCornerID}} infoType<b>)</b></code>
<!-- 
OPENPLAYERDEALSCREENEVENT
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Events|OpenPlayerDealScreenEvent}}<b>(</b>{{Type5|PlayerID}} player, '''int''' target = nil<b>)</b></code>
|}

==P==
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
PARTICLEEFFECTRELOADREQUESTED
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Events|ParticleEffectReloadRequested}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
PARTICLEEFFECTSTATSREQUESTED
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Events|ParticleEffectStatsRequested}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
PARTICLEEFFECTSTATSRESPONSE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Events|ParticleEffectStatsResponse}}<b>(</b>'''unknown''' responseData<b>)</b></code>
<!-- 
PLAYERCHOSETOLOADGAME
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Events|PlayerChoseToLoadGame}}<b>(</b>'''string''' thisLoadFile, '''bool''' arg1 = nil<b>)</b></code>
<!-- 
PLAYERVERSIONMISMATCHEVENT
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Events|PlayerVersionMismatchEvent}}<b>(</b>{{Type5|PlayerID}} player, '''unknown''' playerName, '''bool''' isHost<b>)</b></code>
<!-- 
PREGAMEDIRTY
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Events|PreGameDirty}}<b>(</b><!-- No arguments --><b>)</b></code>
|}

==R==
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
REMOTEPLAYERTURNEND
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Events|RemotePlayerTurnEnd}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
REMOVEALLARROWSEVENT
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Events|RemoveAllArrowsEvent}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
REQUESTYIELDDISPLAY
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Events|RequestYieldDisplay}}<b>(</b>{{Type5|YieldDisplayType}} type, {{Type5|ResourceType}} arg1 = nil, {{Type5|ResourceType}} gridX = nil, '''int''' gridY = nil<b>)</b></code>
<!-- 
RUNCOMBATSIM
-->
|-
{{FuncInfos5|yes  |yes  |yes|This event is triggered every time a unit begins combat. The event will trigger off of any type of combat including but not limited to Melee, Ranged, Bombard, Air Missions and Nuclear. It has not yet been tested whether or not the triggering unit needs to be seen by the (human) player.}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Events|RunCombatSim}}<b>(</b>{{Type5|PlayerID}} attackingPlayer, {{Type5|UnitID}} attackingUnit, '''int''' attackingUnitDamage, '''int''' attackingUnitFinalDamage, '''int''' attackingUnitMaxHitPoints, {{Type5|PlayerID}} defendingPlayer, {{Type5|UnitID}} defendingUnit, '''int''' defendingUnitDamage, '''int''' defendingUnitFinalDamage, '''int''' defendingUnitMaxHitPoints<b>)</b></code>
|}

==S==
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
SEARCHFORPEDIAENTRY
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Events|SearchForPediaEntry}}<b>(</b>'''string''' searchString<b>)</b></code>
<!-- 
SEQUENCEGAMEINITCOMPLETE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Events|SequenceGameInitComplete}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
SERIALEVENTBUILDINGSIZECHANGED
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Events|SerialEventBuildingSizeChanged}}<b>(</b>'''int''' arg0<b>)</b></code>
<!-- 
SERIALEVENTCAMERAIN
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Events|SerialEventCameraIn}}<b>(</b>{{Type5|Vector2}} arg0<b>)</b></code>
<!-- 
SERIALEVENTCAMERAOUT
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Events|SerialEventCameraOut}}<b>(</b>{{Type5|Vector2}} arg0<b>)</b></code>
<!-- 
SERIALEVENTCAMERASTARTMOVINGBACK
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Events|SerialEventCameraStartMovingBack}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
SERIALEVENTCAMERASTARTMOVINGFORWARD
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Events|SerialEventCameraStartMovingForward}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
SERIALEVENTCAMERASTARTMOVINGLEFT
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Events|SerialEventCameraStartMovingLeft}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
SERIALEVENTCAMERASTARTMOVINGRIGHT
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Events|SerialEventCameraStartMovingRight}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
SERIALEVENTCAMERASTOPMOVINGBACK
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Events|SerialEventCameraStopMovingBack}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
SERIALEVENTCAMERASTOPMOVINGFORWARD
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Events|SerialEventCameraStopMovingForward}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
SERIALEVENTCAMERASTOPMOVINGLEFT
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Events|SerialEventCameraStopMovingLeft}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
SERIALEVENTCAMERASTOPMOVINGRIGHT
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Events|SerialEventCameraStopMovingRight}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
SERIALEVENTCITYCAPTURED
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Events|SerialEventCityCaptured}}<b>(</b>{{Type5|Vector2}} hexPos, {{Type5|PlayerID}} player, '''int''' cityID, {{Type5|PlayerID}} newPlayer<b>)</b></code>
<!-- 
SERIALEVENTCITYCONTINENTCHANGED
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Events|SerialEventCityContinentChanged}}<b>(</b>'''float''' hexX, '''int''' hexY, '''int''' arg2<b>)</b></code>
<!-- 
SERIALEVENTCITYCREATED
-->
|-
{{FuncInfos5|yes  |yes  |yes|This event is triggered when a city is created.}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Events|SerialEventCityCreated}}<b>(</b>{{Type5|Vector2}} vHexPos, {{Type5|PlayerID}} player, {{Type5|CityID}} cityID, {{Type5|ArtStyleType}} artStyleType, {{Type5|EraType}} eraType, '''int''' continent, '''int''' populationSize, '''int''' size, '''int''' fogState<b>)</b></code>
<!-- 
SERIALEVENTCITYCULTURECHANGED
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Events|SerialEventCityCultureChanged}}<b>(</b>'''float''' hexX, '''int''' hexY, '''int''' arg2<b>)</b></code>
<!-- 
SERIALEVENTCITYDESTROYED
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Events|SerialEventCityDestroyed}}<b>(</b>{{Type5|Vector2}} hexPos, {{Type5|PlayerID}} player, '''int''' cityID, {{Type5|PlayerID}} newPlayer<b>)</b></code>
<!-- 
SERIALEVENTCITYHEXHIGHLIGHTDIRTY
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Events|SerialEventCityHexHighlightDirty}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
SERIALEVENTCITYINFODIRTY
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Events|SerialEventCityInfoDirty}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
SERIALEVENTCITYPOPULATIONCHANGED
-->
|-
{{FuncInfos5|yes  |yes  |yes|This event is triggered every time the population of a city changes. The triggering city need not belong to the active (human) player, although the city needs to have been discovered by that player. Cities that the active player has no knowledge of will not trigger this event.}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Events|SerialEventCityPopulationChanged}}<b>(</b>'''float''' hexX, '''int''' hexY, '''int''' newPop, '''int''' unknown<b>)</b></code>
<!-- 
SERIALEVENTCITYSCREENDIRTY
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Events|SerialEventCityScreenDirty}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
SERIALEVENTCITYSETDAMAGE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Events|SerialEventCitySetDamage}}<b>(</b>{{Type5|PlayerID}} player, {{Type5|CityID}} cityID, '''int''' damage, '''int''' previousDamage<b>)</b></code>
<!-- 
SERIALEVENTDAWNOFMANHIDE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Events|SerialEventDawnOfManHide}}<b>(</b>'''int''' civID<b>)</b></code>
<!-- 
SERIALEVENTDAWNOFMANSHOW
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Events|SerialEventDawnOfManShow}}<b>(</b>'''int''' civID<b>)</b></code>
<!-- 
SERIALEVENTENDTURNDIRTY
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Events|SerialEventEndTurnDirty}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
SERIALEVENTENTERCITYSCREEN
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Events|SerialEventEnterCityScreen}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
SERIALEVENTERACHANGED
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Events|SerialEventEraChanged}}<b>(</b>'''int''' arg0, {{Type5|PlayerID}} currPlayer<b>)</b></code>
<!-- 
SERIALEVENTESPIONAGESCREENDIRTY
-->
|-
{{FuncInfos5|maybe|yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Events|SerialEventEspionageScreenDirty}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
SERIALEVENTEXITCITYSCREEN
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Events|SerialEventExitCityScreen}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
SERIALEVENTGAMEDATADIRTY
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Events|SerialEventGameDataDirty}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
SERIALEVENTGAMEMESSAGEPOPUP
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Events|SerialEventGameMessagePopup}}<b>(</b>{{Type5|PopupInfo}} popupInfo<b>)</b></code>
<!-- 
SERIALEVENTGAMEMESSAGEPOPUPPROCESSED
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Events|SerialEventGameMessagePopupProcessed}}<b>(</b>{{Type5|ButtonPopupType}} mostRecentPopup, '''int''' arg1<b>)</b></code>
<!-- 
SERIALEVENTGAMEMESSAGEPOPUPSHOWN
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Events|SerialEventGameMessagePopupShown}}<b>(</b>{{Type5|PopupInfo}} PopupInfo<b>)</b></code>
<!-- 
SERIALEVENTHEXCULTURECHANGED
-->
|-
{{FuncInfos5|maybe|maybe|yes|This event is triggered every time a hex changes ownership anywhere on the map.}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Events|SerialEventHexCultureChanged}}<b>(</b>'''int''' hexX, '''int''' hexY, {{Type5|PlayerID}} player, '''bool''' unknown<b>)</b></code>
<!-- 
SERIALEVENTHEXDESELECTED
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Events|SerialEventHexDeSelected}}<b>(</b>'''float''' hexX, '''int''' hexY<b>)</b></code>
<!-- 
SERIALEVENTHEXGRIDOFF
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Events|SerialEventHexGridOff}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
SERIALEVENTHEXGRIDON
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Events|SerialEventHexGridOn}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
SERIALEVENTHEXHIGHLIGHT
-->
|-
{{FuncInfos5|yes  |yes  |yes|This event is triggered every time a hex is highlighted by the UI. Can be invoked from the Lua side, which highlights a hex and is the common usage. If a highlight style is given, it can be cleared again by using Events.ClearHexHighlightStyle or [[Lua_Game_Objects/Events#ClearHexHighlights|ClearHexHighlights]]}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Events|SerialEventHexHighlight}}<b>(</b>{{Type5|Vector2}} hex, '''bool''' highlight, {{Type5|Vector4}} highlightColor, '''string''' highlightStyle<b>)</b></code>
<!-- 
SERIALEVENTHEXSELECTED
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Events|SerialEventHexSelected}}<b>(</b>'''float''' hexX, '''int''' hexY<b>)</b></code>
<!-- 
SERIALEVENTIMPROVEMENTCREATED
-->
|-
{{FuncInfos5|yes  |yes  |yes|This event is triggered whenever an improvement appears on a player's map &mdash; not when an improvement is created on the general game map. This will be the result of an improvement being created on a tile already been discovered by the active player, or a tile being discovered that already hosts an improvement. Barbarian camps and ancient ruins count as improvements, as indexed in the Improvements table. In the course of building an improvement in the standard game, this event will fire twice, once when the game places the graphic for the improvement in progress of being built, and then again when the improvement is built and the graphic changes to indicate that. The GetImprovementType method on a Plot object, however, will only return improvements that are complete.}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Events|SerialEventImprovementCreated}}<b>(</b>'''float''' hexX, '''int''' hexY, {{Type5|ArtStyleType}} continent1, {{Type5|ArtStyleType}} continent2, {{Type5|PlayerID}} player, '''int''' createImprovementType, {{Type5|ImprovementType}} createImprovementRRType, '''int''' createImprovementEra, '''int''' createImprovementState, '''unknown''' ImprovementEra = nil<b>)</b></code>
<!-- 
SERIALEVENTIMPROVEMENTDESTROYED
-->
|-
{{FuncInfos5|maybe|maybe|yes|Like SerialEventImprovementCreated, this event is triggered whenever an improvement appears on a player's map, as a result of an improvement being created on a tile already been discovered by the active player, or a tile being discovered that already hosts an improvement. Barbarian camps and ancient ruins count as improvements, as listed on the Improvement table. A completed improvement replacing an improvement in progress will not trigger this event.}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Events|SerialEventImprovementDestroyed}}<b>(</b>'''int''' hexX, '''int''' hexY, '''int''' continent1, '''int''' continent2<b>)</b></code>
<!-- 
SERIALEVENTMOUSEOVERHEX
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Events|SerialEventMouseOverHex}}<b>(</b>'''int''' hexX, '''int''' hexY<b>)</b></code>
<!-- 
SERIALEVENTRAWRESOURCECREATED
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Events|SerialEventRawResourceCreated}}<b>(</b>'''float''' hexX, '''int''' hexY, {{Type5|ArtStyleType}} continent, {{Type5|ArtStyleType}} continent, {{Type5|PlayerID}} player, '''int''' arg5, '''int''' createResourceType, '''int''' arg7, '''int''' arg8<b>)</b></code>
<!-- 
SERIALEVENTRAWRESOURCEICONCREATED
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Events|SerialEventRawResourceIconCreated}}<b>(</b>'''float''' hexPosX, '''int''' hexPosY, '''unknown''' ImprovementType, {{Type5|ResourceType}} ResourceType<b>)</b></code>
<!-- 
SERIALEVENTRESEARCHDIRTY
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Events|SerialEventResearchDirty}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
SERIALEVENTROADCREATED
-->
|-
{{FuncInfos5|yes  |yes  |yes|This event is triggered whenever a route is built (triggers on railroads despite the name). The tile must have been discovered by the active player but doesn't have to be visible. This also triggers when a new city is founded, which immediately builds a road and railroad on the spot.}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Events|SerialEventRoadCreated}}<b>(</b>'''int''' hexX, '''int''' hexY, {{Type5|PlayerID}} player, '''int''' routeType<b>)</b></code>
<!-- 
SERIALEVENTROADDESTROYED
-->
|-
{{FuncInfos5|yes  |yes  |yes|This event is triggered whenever a route is removed (triggers on railroads despite the name). Does not trigger when pillaging, only for the worker action}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Events|SerialEventRoadDestroyed}}<b>(</b>'''int''' hexX, '''int''' hexY<b>)</b></code>
<!-- 
SERIALEVENTSCOREDIRTY
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Events|SerialEventScoreDirty}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
SERIALEVENTSTARTGAME
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Events|SerialEventStartGame}}<b>(</b>'''int''' arg0 = nil<b>)</b></code>
<!-- 
SERIALEVENTTURNTIMERDIRTY
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Events|SerialEventTurnTimerDirty}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
SERIALEVENTUNITCREATED
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Events|SerialEventUnitCreated}}<b>(</b>{{Type5|PlayerID}} player, {{Type5|UnitID}} unitID, '''int''' hexVec, '''int''' unitType, '''int''' cultureType, '''int''' civID, '''int''' primaryColor, '''int''' secondaryColor, '''int''' unitFlagIndex, '''int''' fogState<b>)</b></code>
<!-- 
SERIALEVENTUNITDESTROYED
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Events|SerialEventUnitDestroyed}}<b>(</b>{{Type5|PlayerID}} player, {{Type5|UnitID}} unitID<b>)</b></code>
<!-- 
SERIALEVENTUNITFLAGSELECTED
-->
|-
{{FuncInfos5|yes  |yes  |yes|This event is triggered every time the flag of a certain unit is selected.}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Events|SerialEventUnitFlagSelected}}<b>(</b>{{Type5|PlayerID}} player, {{Type5|HandicapType}} unit<b>)</b></code>
<!-- 
SERIALEVENTUNITINFODIRTY
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Events|SerialEventUnitInfoDirty}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
SERIALEVENTUNITMOVE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Events|SerialEventUnitMove}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
SERIALEVENTUNITMOVETOHEXES
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Events|SerialEventUnitMoveToHexes}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
SERIALEVENTUNITSETDAMAGE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Events|SerialEventUnitSetDamage}}<b>(</b>{{Type5|PlayerID}} player, {{Type5|UnitID}} unitID, '''int''' damage, '''int''' previousDamage<b>)</b></code>
<!-- 
SERIALEVENTUNITTELEPORTEDTOHEX
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Events|SerialEventUnitTeleportedToHex}}<b>(</b>'''unknown''' i, '''unknown''' j, {{Type5|PlayerID}} player, {{Type5|UnitID}} unitID<b>)</b></code>
<!-- 
SHOWATTACKTARGETS
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Events|ShowAttackTargets}}<b>(</b>{{Type5|PlayerID}} player, {{Type5|UnitID}} arg1<b>)</b></code>
<!-- 
SHOWHEXYIELD
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Events|ShowHexYield}}<b>(</b>'''int''' x, '''int''' y, '''bool''' show<b>)</b></code>
<!-- 
SHOWMOVEMENTRANGE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Events|ShowMovementRange}}<b>(</b>{{Type5|PlayerID}} player, {{Type5|UnitID}} arg1<b>)</b></code>
<!-- 
SPAWNARROWEVENT
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Events|SpawnArrowEvent}}<b>(</b>{{Type5|ResourceType}} arg0, {{Type5|ResourceType}} arg1, '''int''' hexX, '''int''' hexY<b>)</b></code>
<!-- 
SPECIFICCITYINFODIRTY
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Events|SpecificCityInfoDirty}}<b>(</b>{{Type5|PlayerID}} player, {{Type5|CityID}} cityID, {{Type5|CityUpdateType}} updateType<b>)</b></code>
<!-- 
STARTUNITMOVEHEXRANGE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Events|StartUnitMoveHexRange}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
STRATEGICVIEWSTATECHANGED
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Events|StrategicViewStateChanged}}<b>(</b>'''int''' strategicView, '''int''' cityBanners<b>)</b></code>
<!-- 
SYSTEMUPDATEUI
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Events|SystemUpdateUI}}<b>(</b>{{Type5|SystemUpdateUIType}} type<b>)</b></code>
|}

==T==
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
TASKLISTUPDATE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Events|TaskListUpdate}}<b>(</b>{{Type5|PopupInfo}} TaskListInfo<b>)</b></code>
<!-- 
TECHACQUIRED
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Events|TechAcquired}}<b>(</b><!-- No arguments --><b>)</b></code>
|}

==U==
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
UIPATHFINDERUPDATE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Events|UIPathFinderUpdate}}<b>(</b>'''unknown''' data<b>)</b></code>
<!-- 
UNITACTIONCHANGED
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Events|UnitActionChanged}}<b>(</b>{{Type5|PlayerID}} player, {{Type5|UnitID}} unitID<b>)</b></code>
<!-- 
UNITDATAEDITED
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Events|UnitDataEdited}}<b>(</b>'''int''' floatVarList, '''int''' memberCount, '''int''' memberIndex, '''bool''' isDebugFSM, {{Type5|SpecialistType}} specRender, '''bool''' isFromLua = nil<b>)</b></code>
<!-- 
UNITDATAREQUESTED
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Events|UnitDataRequested}}<b>(</b>'''int''' arg0<b>)</b></code>
<!-- 
UNITDEBUGFSM
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Events|UnitDebugFSM}}<b>(</b>'''int''' arg0<b>)</b></code>
<!-- 
UNITEMBARK
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Events|UnitEmbark}}<b>(</b>{{Type5|PlayerID}} player, {{Type5|UnitID}} unitID<b>)</b></code>
<!-- 
UNITFLAGUPDATED
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Events|UnitFlagUpdated}}<b>(</b>'''int''' unitCulture, '''int''' unitType, '''float''' unitHealth, '''bool''' unitFortified<b>)</b></code>
<!-- 
UNITGARRISON
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Events|UnitGarrison}}<b>(</b>{{Type5|PlayerID}} player, {{Type5|UnitID}} unitID, '''int''' garrisoned<b>)</b></code>
<!-- 
UNITHEXHIGHLIGHT
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Events|UnitHexHighlight}}<b>(</b>'''float''' i, '''int''' j, '''unknown''' k, '''bool''' on, '''int''' unitId<b>)</b></code>
<!-- 
UNITLIBRARYSWAP
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Events|UnitLibrarySwap}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
UNITMARKTHREATENING
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Events|UnitMarkThreatening}}<b>(</b>{{Type5|PlayerID}} player, {{Type5|UnitID}} unitID, '''bool''' mark<b>)</b></code>
<!-- 
UNITMEMBERCOMBATSTATECHANGED
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Events|UnitMemberCombatStateChanged}}<b>(</b>{{Type5|PlayerID}} player, {{Type5|UnitID}} unitID, '''int''' memberID, '''unknown''' stateID<b>)</b></code>
<!-- 
UNITMEMBERCOMBATTARGETCHANGED
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Events|UnitMemberCombatTargetChanged}}<b>(</b>{{Type5|PlayerID}} player, {{Type5|UnitID}} unitID, '''int''' memberID, '''unknown''' targetPlayerID, '''unknown''' targetUnitID, '''int''' targetMemberID<b>)</b></code>
<!-- 
UNITMEMBEROVERLAYADD
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Events|UnitMemberOverlayAdd}}<b>(</b>{{Type5|PlayerID}} player, {{Type5|UnitID}} unitID, '''int''' memberID, '''unknown''' position<b>)</b></code>
<!-- 
UNITMEMBEROVERLAYREMOVE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Events|UnitMemberOverlayRemove}}<b>(</b>{{Type5|PlayerID}} player, {{Type5|UnitID}} unitID, '''int''' memberID<b>)</b></code>
<!-- 
UNITMEMBEROVERLAYSHOWHIDE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Events|UnitMemberOverlayShowHide}}<b>(</b>{{Type5|PlayerID}} player, {{Type5|UnitID}} unitID, '''int''' memberID, '''bool''' show<b>)</b></code>
<!-- 
UNITMEMBERPOSITIONCHANGED
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Events|UnitMemberPositionChanged}}<b>(</b>{{Type5|PlayerID}} player, {{Type5|UnitID}} unitID, '''int''' memberID, '''unknown''' unitPosition<b>)</b></code>
<!-- 
UNITMOVEQUEUECHANGED
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Events|UnitMoveQueueChanged}}<b>(</b>{{Type5|PlayerID}} player, {{Type5|UnitID}} unitID, '''bool''' remainingMoves<b>)</b></code>
<!-- 
UNITSELECTIONCHANGED
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Events|UnitSelectionChanged}}<b>(</b>{{Type5|PlayerID}} player, {{Type5|UnitID}} u, '''float''' hexX, '''float''' hexY, '''int''' k, '''bool''' isSelected, '''bool''' arg6<b>)</b></code>
<!-- 
UNITSELECTIONCLEARED
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Events|UnitSelectionCleared}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
UNITSHOULDDIMFLAG
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Events|UnitShouldDimFlag}}<b>(</b>{{Type5|PlayerID}} player, {{Type5|UnitID}} unitID, '''int''' dim<b>)</b></code>
<!-- 
UNITSTATECHANGEDETECTED
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Events|UnitStateChangeDetected}}<b>(</b>{{Type5|PlayerID}} player, {{Type5|UnitID}} unitID, '''int''' fogState<b>)</b></code>
<!-- 
UNITTYPECHANGED
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Events|UnitTypeChanged}}<b>(</b>'''string''' arg0<b>)</b></code>
<!-- 
UNITVISIBILITYCHANGED
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Events|UnitVisibilityChanged}}<b>(</b>{{Type5|PlayerID}} player, {{Type5|UnitID}} unitID, '''bool''' visible, '''bool''' checkFlag, '''unknown''' blendTime<b>)</b></code>
<!-- 
USERREQUESTCLOSE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Events|UserRequestClose}}<b>(</b><!-- No arguments --><b>)</b></code>
|}

==W==
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
WARSTATECHANGED
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Events|WarStateChanged}}<b>(</b>{{Type5|TeamID}} team1, {{Type5|TeamID}} team2, '''bool''' war<b>)</b></code>
<!-- 
WORLDMOUSEOVER
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Events|WorldMouseOver}}<b>(</b>'''int''' worldHasMouseOver<b>)</b></code>
|}




{{Civ5 API Footer}}
[[Category:Civ5 Types|Events]]