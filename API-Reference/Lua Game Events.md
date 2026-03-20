Up: [[Lua and UI Reference]]

[http://forums.civfanatics.com/showthread.php?t=385612 Lua Events List] or the same [http://wiki.2kgames.com/civ5/index.php/Lua_Game_Events in the official wiki]


==Game==
*[[LoadScreenClose]]
*[[PreGameDirty]]
*[[SerialEventEndTurnDirty]]
*[[SequenceGameInitComplete]]
*[[SerialEventGameDataDirty]]
*[[SerialEventStartGame]]


*[[GameEvents.PreGameStart]] - called before most items in the game are initialized.


==Team==
*[[GameEvents.TeamSetHasTech(teamID, techID)]]
*[[GameEvents.TeamTechResearched(eTeam, eTech, iChange)]] - triggered when a team researches a tech.


==Player==
*[[ActivePlayerTurnEnd]]
*[[ActivePlayerTurnStart]] - fired on the start of the human player's turn (not fired for AIs).
*[[EventPoliciesDirty]]
*[[GameplaySetActivePlayer]]
*[[SerialEventEraChanged]]
*[[SerialEventResearchDirty]]
*[[SerialEventScoreDirty]]
*[[TeamMet]]
*[[TechAcquired]]
*[[WarStateChanged]]


*[[GameEvents.CanDeclareWar(team1, team2)]] - allows provision of criteria for the ability of team1 to declare war on team2. As this is a TestAll event, all listeners must return true for the action to be permitted.
*[[GameEvents.PlayerAdoptPolicy(playerID, policyTypeID)]]
*[[GameEvents.PlayerAdoptPolicyBranch(playerID, policyBranchTypeID)]]
*[[GameEvents.PlayerCanAdoptPolicy(playerID, policyTypeID)]]
*[[GameEvents.PlayerCanAdoptPolicyBranch(playerID, policyBranchTypeID)]]
*[[GameEvents.PlayerCanConstruct(playerID, buildingTypeID)]]
*[[GameEvents.PlayerCanCreate(playerID, projectTypeID)]]
*[[GameEvents.PlayerCanEverReseearch(playerID, techtypeID)]]
*[[GameEvents.PlayerCanMaintain(playerID, processTypeID)]]
*[[GameEvents.PlayerCanPrepare(playerID, specialistTypeID)]]
*[[GameEvents.PlayerCanResearch(playerID, techTypeID)]]
*[[GameEvents.PlayerCanTrain(playerID, unitTypeID)]]
*[[GameEvents.PlayerDoTurn()]] - fired once per turn for each player (not just active/human player), at the start of turn; also, it seems not to run for the first turn of the game (for all players), runs only for human player on the second turn, and thereafter it runs for all players.
*[[GameEvents.PlayerPreAIUnitUpdate(playerId)]]
*[[GameEvents.SetAlly(iCSPlayer, iOldAlly, iNewAlly)]] - triggered when the ally of a City-State changes (whether it changes from none or from another player). 
*[[GameEvents.TeamMeet(playerActive, playerMet)]] - presumably called when players meet, but referring to teams.


==City==
*[[CityHandleCreated]]
*[[CityRuinsCreated]]
*[[InitCityRangeStrike]]
*[[SerialEventCityCaptured]] - fired when city is captured '''or traded to an another civ'''.
*[[SerialEventCityContinentChanged]]
*[[SerialEventCityCreated]] - fired when city is created.
*[[SerialEventCityCultureChanged]]
*[[SerialEventCityDestroyed]] - fired when city is destroyed.
*[[SerialEventCityHexHighlightDirty]]
*[[SerialEventCityInfoDirty]]
*[[SerialEventCityPopulationChanged]] - fired when a population of a particular city was changed.
*[[SerialEventCityScreenDirty]]
*[[SerialEventCitySetDamage]]
*[[SerialEventEnterCityScreen]]
*[[SerialEventExitCityScreen]]
*[[SpecificCityInfoDirty]] - fired when something in a particular city was changed.


*[[GameEvents.CityCanBuyAnyPlot(ownerID, cityID)]]
*[[GameEvents.CityCanBuyPlot(ownerID, cityID, plotX, plotY)]]
*[[GameEvents.CityCanConstruct(iPlayer, iCity, iBuildingType)]] - this allows provision of critera for the ability to construct a particular building (including Wonders, presumably) in a particular city. Based on the behaviour in the 1066 scenario, it seems that returns of false lead to the building not appearing in the list of buildings available to construct, rather than being greyed out, but this hasn't been specifically checked. It makes some sense, though, as there's no way to provide a tooltip to explain the greying out under this mechanism.
*[[GameEvents.CityCanCreate(ownerID, cityID, projectTypeID)]]
*[[GameEvents.CityCanMaintain(ownerID, cityID, processTypeID)]]
*[[GameEvents.CityCanPrepare(ownerID, cityID, specialistTypeID)]]
*[[GameEvents.CityCanTrain(ownerID, cityID, unitTypeID)]]
*[[GameEvents.CityCaptureComplete(playerID, bCapital, iX, iY, newPlayerID)]]
*[[GameEvents.SetPopulation(iX, iY, oldPopulation, newPopulation)]]


==Unit==
*[[AddUnitMoveHexRangeHex]]
*[[ClearUnitMoveHexRange]]
*[[EndUnitMoveHexRange]]
*[[GlobalUnitScale]]
*[[LocalMachineUnitPositionChanged]]
*[[SerialEventUnitCreated]]
*[[SerialEventUnitDestroyed]]
*[[SerialEventUnitFacingChanged]]
*[[SerialEventUnitFlagSelected]]
*[[SerialEventUnitInfoDirty]]
*[[SerialEventUnitMove]]
*[[SerialEventUnitMoveToHexes]]
*[[SerialEventUnitSetDamage]]
*[[SerialEventUnitTeleportedToHex]]
*[[StartUnitMoveHexRange]]
*[[ToggleDisplayUnits]]
*[[UnitActionChanged]]
*[[UnitDataEdited]]
*[[UnitDataRequested]]
*[[UnitDebugFSM]]
*[[UnitEmbark]]
*[[UnitFlagUpdated]]
*[[UnitGarrison]]
*[[UnitHandleCreated]]
*[[UnitHexHighlight]]
*[[UnitHexHighlight]]
*[[UnitLibrarySwap]]
*[[UnitMarkThreatening]]
*[[UnitMemberCombatStateChanged]]
*[[UnitMemberCombatTargetChanged]]
*[[UnitMemberOverlayAdd]]
*[[UnitMemberOverlayMessage]]
*[[UnitMemberOverlayRemove]]
*[[UnitMemberOverlayShowHide]]
*[[UnitMemberOverlayTargetColor]]
*[[UnitMemberPositionChanged]]
*[[UnitMoveQueueChanged]]
*[[UnitSelectionChanged]]
*[[UnitSelectionCleared]]
*[[UnitShouldDimFlag]]
*[[UnitStateChangeDetected]]
*[[UnitTypeChanged]]
*[[UnitVisibilityChanged]]
===CombatSim===
*[[RunCombatSim]]
*[[EndCombatSim]]


*[[GameEvents.UnitGetSpecialExploreTarget(iPlayerID, iUnitID)]] - appears to be triggered when the 'explore' order is given, or some subset thereof. The unit structure for the relevant unit is manipulated to set the explore target. 
*[[GameEvents.UnitSetXY(iPlayer, iUnitID, iX, iY)]] - triggered whenever any unit moves by any means, for every tile they move into. 


==Map objects==
*[[NaturalWonderRevealed]]
===Improvements===
*[[SerialEventImprovementCreated]]
*[[SerialEventImprovementDestroyed]]
*[[SerialEventImprovementIconCreated]]
*[[SerialEventImprovementIconDestroyed]]
*[[SerialEventRoadCreated]]
*[[SerialEventRoadDestroyed]]
===Features===
*[[SerialEventFeatureCreated]]
*[[SerialEventFeatureDestroyed]]
*[[SerialEventForestCreated]]
*[[SerialEventForestRemoved]]
*[[SerialEventJungleCreated]]
*[[SerialEventJungleRemoved]]


==Hex==
*[[AddUnitMoveHexRangeHex]]
*[[ClearHexHighlights]]
*[[ClearHexHighlightStyle]]
*[[ClearUnitMoveHexRange]]
*[[EndUnitMoveHexRange]]
*[[HexFOWStateChanged]]
*[[HexYieldMightHaveChanged]]
*[[SerialEventCityHexHighlightDirty]]
*[[SerialEventHexCultureChanged]]
*[[SerialEventHexDeSelected]]
*[[SerialEventHexGridOff]]
*[[SerialEventHexGridOn]]
*[[SerialEventHexHighlight]]
*[[SerialEventHexSelected]]
*[[SerialEventMouseOverHex]]
*[[SerialEventUnitMoveToHexes]]
*[[SerialEventUnitTeleportedToHex]]
*[[ShowHexYield]]
*[[StartUnitMoveHexRange]]
*[[UnitHexHighlight]]
*[[UnitHexHighlight]]


===Mods===
*[[AfterModsActivate]]
*[[AfterModsDeactivate]]
*[[BeforeModsActivate]]
*[[BeforeModsDeactivate]]
*[[InstalledModsUpdated]]
*[[ModDownloadComplete]]
*[[ModDownloadStarted]]


==Interface==
*[[AddPopupTextEvent]]
*[[FrontEndPopup]]
*[[MinimapClickedEvent]]
*[[OpenInfoCorner]]
*[[SerialEventGameMessagePopup]]
*[[SerialEventGameMessagePopupProcessed]]
*[[SerialEventGameMessagePopupShown]]
*[[SerialEventInfoPaneDirty]]
*[[ToolTipEvent]]
===Advisor===
*[[AdvisorDisplayHide]]
*[[AdvisorDisplayShow]]
===Dawn of Man===
*[[SerialEventDawnOfManHide]]
*[[SerialEventDawnOfManShow]]
===Diplomacy===
*[[ClearDiplomacyTradeTable]]
*[[OpenPlayerDealScreenEvent]]
===Menus===
*[[EventOpenOptionsScreen]]
*[[ExitToMainMenu]]
*[[PlayerChoseToLoadGame]]
*[[PlayerChoseToLoadMap]]
===Notifications===
*[[NotificationActivated]]
*[[NotificationAdded]]
*[[NotificationRemoved]]


==Game Systems==
===Animation===
*[[AnimationSamplingChanged]]
*[[ParticleEffectReloadRequested]]
*[[ParticleEffectStatsRequested]]
*[[ParticleEffectStatsResponse]]
*[[RemoveAllArrowsEvent]]
*[[SerialEventTestAnimations]]
*[[SpawnArrowEvent]]
===Audio===
*[[AudioDebugChangeMusic]]
*[[AudioPlay2DSound]]
*[[AudioVolumeChanged]]
===Camera===
*[[CameraProjectionChanged]]
*[[CameraStartPitchingDown]]
*[[CameraStartPitchingUp]]
*[[CameraStartRotatingCCW]]
*[[CameraStartRotatingCW]]
*[[CameraStopPitchingDown]]
*[[CameraStopPitchingUp]]
*[[CameraStopRotatingCCW]]
*[[CameraStopRotatingCW]]
*[[CameraViewChanged]]
*[[DragCamera]]
*[[SerialEventCameraBack]]
*[[SerialEventCameraForward]]
*[[SerialEventCameraIn]]
*[[SerialEventCameraLeft]]
*[[SerialEventCameraOut]]
*[[SerialEventCameraRight]]
*[[SerialEventCameraSetCenterAndZoom]]
*[[SerialEventCameraStartMovingBack]]
*[[SerialEventCameraStartMovingForward]]
*[[SerialEventCameraStartMovingLeft]]
*[[SerialEventCameraStartMovingRight]]
*[[SerialEventCameraStopMovingBack]]
*[[SerialEventCameraStopMovingForward]]
*[[SerialEventCameraStopMovingLeft]]
*[[SerialEventCameraStopMovingRight]]
===Multiplayer===
*[[ConnectedToNetworkHost]]
*[[MultiplayerConnectionComplete]]
*[[MultiplayerConnectionFailed]]
*[[MultiplayerGameAbandoned]]
*[[MultiplayerGameLaunched]]
*[[MultiplayerGameListClear]]
*[[MultiplayerGameListComplete]]
*[[MultiplayerGameListUpdated]]
*[[MultiplayerGamePlayerDisconnected]]
*[[MultiplayerGamePlayerUpdated]]
*[[MultiplayerJoinRoomAttempt]]
*[[MultiplayerJoinRoomComplete]]
*[[MultiplayerJoinRoomFailed]]
*[[MultiplayerProfileDisconnected]]
*[[MultiplayerProfileFailed]]
*[[RemotePlayerTurnEnd]]


==Other (unsorted)==
*[[AppInitComplete]]
*[[AILeaderMessage]]
*[[BuildingLibrarySwap]]
*[[DisplayMovementIndicator]]
*[[DontRecordCommandStreams]]
*[[EndTurnTimerUpdate]]
*[[GenericWorldAnchor]]
*[[GraphicsOptionsChanged]]
*[[InterfaceModeChanged]]
*[[KeyUpEvent]]
*[[LandmarkLibrarySwap]]
*[[LanguageChanging]]
*[[LeavingLeaderViewMode]]
*[[LocalMachineAppUpdate]]
*[[MinimapTextureBroadcastEvent]]
*[[RecordCommandStreams]]
*[[RequestYieldDisplay]]
*[[SearchForPediaEntry GoToPediaHomePage]]
*[[SerialEventBuildingSizeChanged]]
*[[SerialEventLeaderToggleDebugCam]]
*[[SerialEventRawResourceCreated]]
*[[SerialEventRawResourceDestroyed]]
*[[SerialEventRawResourceIconCreated]]
*[[SerialEventRawResourceIconDestroyed]]
*[[SerialEventScreenShot]]
*[[SerialEventTerrainDecalCreated]]
*[[SerialEventTerrainOverlayMod]]
*[[SerialEventTest]]
*[[SerialEventTurnTimerDirty]]
*[[ShowAttackTargets]]
*[[ShowMovementRange]]
*[[StateMachineDumpStates]]
*[[StateMachineRequestStates]]
*[[StrategicViewStateChanged]]
*[[SystemUpdateUI]]
*[[TaskListUpdate]]
*[[UIPathFinderUpdate]]
*[[UserRequestClose]]
*[[VisibilityUpdated]]
*[[WonderStateChanged]]
*[[WonderTogglePlacement]]
*[[WonderTypeChanged]]
*[[WorldMouseOver]]