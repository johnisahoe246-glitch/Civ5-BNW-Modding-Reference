The '''CvEventManager''' file controls what happens during events that occur in the game. These aren't events like Beyond the Sword random events but rather events like a unit moving, a turn beginning, or a nuclear explosion occuring. Some of the functions in this file are disabled in Beyond the Sword with [[PythonCallbackDefines]].xml- for a list of which functions, see that page.

The Python files are written in the python programming language.  They can be edited in a text editor such as notepad or in a programming editor like Python's IDLE.

<font color=red>This page is missing information. Do not remove this notice until it is complete.</font>

==Functions==

Below is a list of all the functions in the file. Each function has a quick description attached to it. Note that there are comments strewn throughout some of these files, direct from the developers in order to aid the potential modders. All these functions are in the class CvEventManager.
{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"
|-
! style="background:#efefef;" | Function 
! style="background:#efefef;" | Parameters
! style="background:#efefef;" | Description
|-
!def _init_()
|self
|Initializes variables in file
|-
!def handleEvent()
|self, argsList
|Event Manager entry point
|-
!def beginEvent()
|self, context, argsList=-1
|Begins an event
|-
!def applyEvent()
|self, argsList (context, playerID, netUserData, popupReturn)
|Applies the effects of an event
|-
!def reportEvent()
|self, entry, context, argsList
|Records an event to Events.log
|-
!def onKdbEvent()
|self, argsList (eventType, key, mx, my, px, py)
|Handles the pressing of a key
|-
!def onModNetMessage()
|self, argsList (iData1, iData2, iData3, iData4, iData5)
|Called whenever CyMessageControl().sendModNetMessage is called
|-
!def onInit()
|self, argsList
|Called whenever Civilization starts up
|-
!def onUpdate()
|self, argsList (fDeltaTime)
|Called every frame
|-
!def onWindowActivation()
|self, argsList (bActive)
|Called when the game window activates or deactivates
|-
!def onUnInit()
|self, argsList
|Called before Civ shuts down
|-
!def onPreSave()
|self, argsList
|Called before the game is saved
|-
!def onSaveGame()
|self, argsList
|Returns the name of the save game
|-
!def onLoadGame()
|self, argsList
|Called on the loading of the game
|-
!def onGameStart()
|self, argsList
|Called on the start of the game
|-
!def onGameEnd()
|self, argsList
|Called at the end of the game
|-
!def onBeginGameTurn()
|self, argsList (iGameTurn)
|Called at the beginning of the end of each turn
|-
!def onEndGameTurn()
|self, argsList (iGameTurn)
|Called at the end of the end of each turn
|-
!def onBeginPlayerTurn()
|self, argsList (iGameTurn, iPlayer)
|Called at the beginning of a player's turn
|-
!def onEndPlayerTurn()
|self, argsList (iGameTurn, iPlayer)
|Called at the end of a player's turn
|-
!def onEndTurnReady()
|self, argsList (iGameTurn)
|Called when the turn is ready to end
|-
!def onFirstContact()
|self, argsList (iTeamX, iHasMetTeamY)
|Called when one team meets another team
|-
!def onCombatResult()
|self, argsList (iWinner, iLoser)
|Called after combat
|-
!def onCombatLogCalc()
|self, argsList (genericArgs)
|Not sure
|-
!def onCombatLogHit()
|self, argsList (genericArgs)
|Not sure
|-
!def onImprovementBuilt()
|self, argsList (iImprovement, iX, iY)
|Called when an improvement is built
|-
!def onImprovementDestroyed()
|self, argsList (iImprovement, iOwner, iX, iY)
|Called when an improvement is destroyed
|-
!def onRouteBuilt()
|self, argsList (iRoute, iX, iY)
|Called when a route is built
|-
!def onPlotRevealed()
|self, argsList (pPlot, iTeam)
|Called when a plot is revealed to a team
|-
!def onPlotFeatureRemoved()
|self, argsList (pPlot, iFeatureType, pCity)
|Called when a feature is removed on a plot
|-
!def onPlotPicked()
|self, argsList (pPlot)
|Called when a plot is picked
|-
!def onNukeExplosion()
|self, argsList (pPlot, pNukeUnit)
|Called when a nuke explodes or a meltdown occurs
|-
!def onGotoPlotSet()
|self, argsList (pPlot, iPlayer)
|Not sure
|-
!def onBuildingBuilt()
|self, argsList (pCity, iBuildingType)
|Called when a building is built
|-
!def onProjectBuilt()
|self, argsList (pCity, iProjectType)
|Called when a project is completed
|-
!def onSelectionGroupPushMission()
|self, argsList (eOwner, eMission, iNumUnits, listUnitIDs)
|Called when a mission is pushed for a unit or group of units
|-
!def onUnitMove()
|self, argsList (pPlot, pUnit, pOldPlot)
|Called when a unit moves onto a new plot
|-
!def onUnitSetXY()
|self, argsList (pPlot, pUnit)
|Called when a unit's coords are set manually
|-
!def onUnitCreated()
|self, argsList (unit)
|Called when a unit is created
|-
!def onUnitBuilt()
|self, argsList (city, unit, player)
|Called when a unit is built in a city
|-
!def onUnitKilled()
|self, argsList (unit, iAttacker)
|Called when a unit is killed by another unit
|-
!def onUnitLost()
|self, argsList (unit)
|Called when a unit dies
|-
!def onUnitPromoted()
|self, argsList (pUnit, iPromotion)
|Called when a unit is promoted
|-
!def onUnitSelected()
|self, argsList (unit)
|Called when a unit is selected
|-
!def onUnitRename()
|self, argsList (unit)
|Called when a unit is renamed
|-
!def onUnitPillage()
|self, argsList(pUnit, iImprovement, iRoute, iOwner)
|Called when a unit pillages an improvement or route
|-
!def onUnitSpreadReligionAttempt()
|self, argsList(pUnit, iReligion, bSuccess)
|Called when a unit attempts to spread a religion to a city
|-
!def onUnitGifted()
|self, argsList(pUnit, iGiftingPlayer, pPlotLocation)
|Called when a unit is gifted from a player to another
|-
!def onUnitBuildImprovement()
|self, argsList(pUnit, iBuild, bFinished)
|Called when a unit begins to build an improvement
|-
!def onGoodyReceived()
|self, argsList(iPlayer, pPlot, pUnit, iGoodyType)
|Called when a unit gets something at a goody hut
|-
!def onGreatPersonBorn()
|self, argsList(pUnit, iPlayer, pCity)
|Called when a Great Person is born in a city
|-
!def onTechAcquired()
|self, argsList(iTechType, iTeam, iPlayer, bAnnounce)
|Called when a player acquires a tech
|-
!def onTechSelected()
|self, argsList(iTechType, iPlayer)
|Called when a player selects a tech to research
|-
!def onReligionFounded()
|self, argsList(iReligion, iFounder)
|Called when a player founds a religion
|-
!def onReligionSpread()
|self, argsList(iReligion, iOwner, pSpreadCity)
|Called when a religion spreads to a city
|-
!def onReligionRemove()
|self, argsList(iReligion, iOwner, pRemoveCity)
|Called when a religion is removed from a city
|-
!def onCorporationFounded()
|self, argsList(iCorporation, iFounder)
|Called when a player founds a corporation
|-
!def onCorporatationSpread()
|self, argsList(iCorporation, iOwner, pSpreadCity)
|Called when a corporation spreads to a city
|-
!def onCorporationRemove()
|self, argsList(iCorporation, iOwner, pRemoveCity)
|Called when a corporation is removed from a city
|-
!def onGoldenAge()
|self, argsList(iPlayer)
|Called when a player begins a golden age
|-
!def onEndGoldenAge()
|self, argsList(iPlayer)
|Called when a player ends a golden age
|-
!def onChangeWar()
|self, argsList(bIsWar, iTeam, iRivalTeam)
|Called when either war or peace is declared between two teams
|-
!def onChat()
|self, argsList(chatMessage)
|Called when a chat message is sent
|-
!def onSetPlayerAlive()
|self, argsList(iPlayerID, bNewValue)
|Called when a player's status is set to "alive"
|-
!def onPlayerChangeStateReligion
|self, argsList(iPlayer, iNewReligion, iOldReligion)
|Called when a player changes the state religion
|-
!def onPlayerGoldTrade
|self, argsList(iFromPlayer, iToPlayer, iGoldAmount)
|Called when a player trades gold with another player
|-
!def onCityBuilt
|self, argsList(city)
|Called when a player builds a city
|-
!def onCityRazed
|self, argsList(city, iPlayer)
|Called when a player razes a city
|-
!def onCityAcquired
|self, argsList(iPreviousOwner, iNewOwner, pCity, bConquest, bTrade)
|Called when a player acquires a city through any means
|-
!def onCityAcquiredAndKept
|self, argsList(iOwner, pCity)
|Called when a player acquires a city and keeps it
|-
!def onCityLost
|self, argsList(city, player)
|Called when a player loses a city
|-
!def onCultureExpansion
|self, argsList(pCity, iPlayer)
|Called when a city's culture expands
|-
!def onCityGrowth
|self, argsList(pCity, iPlayer)
|Called when a city grows
|-
!def onCityDoTurn
|self, argsList(pCity, iPlayer)
|Called every turn for every city
|-
!def onCityBuildingUnit
|self, argsList(pCity, iUnitType)
|Called when a city begins building a unit
|-
!def onCityBuildingBuilding
|self, argsList(pCity, iBuildingType)
|Called when a city begins building a building
|-
!def onCityRename
|self, argsList(pCity)
|Called when a city is renamed
|-
!def onCityHurry
|self, argsList(pCity, iHurryType)
|Called when a city hurries production
|-
!def onVictory
|self, argsList(iTeam, iVictory)
|Called when a team wins the game
|-
!def onVassalState
|self, argsList(iMaster, iVassal, bVassal)
|Called when a team is vassalized or gains independence
|-
!def onGameUpdate
|self, argsList(genericArgs[turnSlice])
|Called on every "game turn slice"
|-
!def onMouseEvent
|self, argsList(eventType, mx, my, px, py, interfaceConsumed, screens)
|Not sure
|-
!def _eventEventCityNameBegin
|self, city, bRename
|Creates a popup to name or rename a city
|-
!def _eventEventCityNameApply
|self, playerID, userData(iCityID, bRename), popupReturn
|Changes the name of a city
|-
!def _eventEditCityBegin
|self, argsList(px, py)
|Begins the editing of a city in Worldbuilder
|-
!def _eventEditCityApply
|self, playerID, userData, popupReturn
|The edit city event in Worldbuilder
|-
!def _eventPlaceObjectBegin
|self, argsList
|Begins the place object function in Worldbuilder
|-
!def _eventPlaceObjectApply
|self, playerID, userData, popupReturn
|The place object event in Worldbuilder
|-
!def _eventAwardTechsAndGoldBegin
|self, argsList
|An event that awards gold and technologies
|-
!def _eventAwardTechsAndGoldApply
|self, playerId, netUserData, popupReturn
|An event that awards gold and technologies
|-
!def _eventShowWonderBegin
|self, argsList
|Shows the wonder movie after building a wonder
|-
!def _eventShowWonderApply
|self, playerID, netUserData, popupReturn)
|Shows the wonder movie after building a wonder
|-
!def _eventEditUnitNameBegin
|self, argsList(pUnit)
|Creates a popup to rename a unit
|-
!def _eventEditUnitNameApply
|self, playerID, userData, popupReturn
|The event to let you rename a unit
|-
!def _eventWBAllPlotsPopupBegin
|self, argsList
|An event that reveals all plots in Worldbuilder
|-
!def _eventWBAllPlotsPopupApply
|self, playerID, userData, popupReturn
|An event that reveals all plots in Worldbuilder
|-
!def _eventWBLandmarkPopupBegin
|self, argsList
|Creates a popup to label a plot with a landmark tag
|-
!def _eventWBLandmarkPopupApply
|self, playerID, userData, popupReturn
|Labels a plot with a landmark tag
|-
!def _eventWBScriptPopupBegin
|self, argsList
|Not sure
|-
!def _eventWBScriptPopupApply
|self, playerID, userData, popupReturn
|Not sure
|-
!def _eventWBStartYearPopupBegin
|self, argsList
|Not sure
|-
!def _eventWBStartYearPopupApply
|self, playerID, userData, popupReturn
|Not sure
|-
|}

==Example==

This example is a quick idea of what you can do with functions in this file. It causes the "Do you want to change civics" popup to occur.

 	def onEndPlayerTurn(self, argsList):
 		'Called at the end of a players turn'
 		iGameTurn, iPlayer = argsList
 		
 		if (gc.getGame().getElapsedGameTurns() == 1):
 			if (gc.getPlayer(iPlayer).isHuman()):
 				if (gc.getPlayer(iPlayer).canRevolution(0)):
 					popupInfo = CyPopupInfo()
 					popupInfo.setButtonPopupType(ButtonPopupTypes.BUTTONPOPUP_CHANGECIVIC)
 					popupInfo.addPopup(iPlayer)

{{Civ4_Python_Files}}