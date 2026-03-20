The Game namespace represents the currently active CvGame instance.<br>
Back to [[Lua Game Objects]]<br>
=Static Methods=

==AddPlayer==
''<summary>''

'''Usage'''

void Game.addPlayer([[Lua Game Objects/PlayerTypes|PlayerTypes]] eNewPlayer, [[Lua Game Objects/LeaderHeadTypes|LeaderHeadTypes]] eLeader, [[Lua Game Objects/CivilizationTypes|CivilizationTypes]] eCiv);

'''Parameters'''

:eNewPlayer
::No Description Available
:eLeader
::No Description Available
:eCiv
::No Description Available

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==CalculateOptionsChecksum==
''<summary>''

'''Usage'''

int Game.calculateOptionsChecksum();

'''Parameters'''

None

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==CalculateSyncChecksum==
''<summary>''

'''Usage'''

int Game.calculateSyncChecksum();

'''Parameters'''

None

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==CanHandleAction==
''<summary>''

'''Usage'''

boolean Game.CanHandleAction(int iAction, [[Lua Game Objects/Plot|<Plot>]] pPlot, boolean bTestVisible);

'''Parameters'''

:iAction
::No Description Available
:pPlot
::No Description Available
:bTestVisible
::No Description Available

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==CanHaveSecretaryGeneral==
''<summary>''

'''Usage'''

boolean Game.canHaveSecretaryGeneral([[Lua Game Objects/VoteSourceTypes|VoteSourceTypes]] eVoteSource);

'''Parameters'''

:eVoteSource
::No Description Available

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==CanTrainNukes==
''<summary>''

'''Usage'''

boolean Game.canTrainNukes();

'''Parameters'''

None

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==ChangeDiploVote==
''<summary>''

'''Usage'''

void Game.changeDiploVote([[Lua Game Objects/VoteSourceTypes|VoteSourceTypes]] eVoteSource, int iChange);

'''Parameters'''

:eVoteSource
::No Description Available
:iChange
::No Description Available

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==ChangeMaxTurns==
''<summary>''

'''Usage'''

void Game.changeMaxTurns(int iChange);

'''Parameters'''

:iChange
::No Description Available

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==ChangeNoNukesCount==
''<summary>''

'''Usage'''

void Game.changeNoNukesCount(int iChange);

'''Parameters'''

:iChange
::No Description Available

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==ChangeNukesExploded==
''<summary>''

'''Usage'''

void Game.changeNukesExploded(int iChange);

'''Parameters'''

:iChange
::No Description Available

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==ChangePlotExtraCost==
''<summary>''

'''Usage'''

void Game.changePlotExtraCost(int iX, int iY, int iExtraCost);

'''Parameters'''

:iX
::No Description Available
:iY
::No Description Available
:iExtraCost
::No Description Available

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==CityPurchaseBuilding==
''<summary>''

'''Usage'''

void Game.cityPurchase([[Lua Game Objects/City|<City>]] pCity, [[Lua Game Objects/UnitTypes|UnitTypes]] eUnitType, [[Lua Game Objects/BuildingTypes|BuildingTypes]] eBuildingType, [[Lua Game Objects/ProjectTypes|ProjectTypes]] [[Lua Game Objects/eProjectTypes|eProjectTypes]]);

'''Parameters'''

:pCity
::No Description Available
:eUnitType
::No Description Available
:eBuildingType
::No Description Available
:eProjectTypes
::No Description Available

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==CityPurchaseProject==
''<summary>''

'''Usage'''

void Game.cityPurchase([[Lua Game Objects/City|<City>]] pCity, [[Lua Game Objects/UnitTypes|UnitTypes]] eUnitType, [[Lua Game Objects/BuildingTypes|BuildingTypes]] eBuildingType, [[Lua Game Objects/ProjectTypes|ProjectTypes]] [[Lua Game Objects/eProjectTypes|eProjectTypes]]);

'''Parameters'''

:pCity
::No Description Available
:eUnitType
::No Description Available
:eBuildingType
::No Description Available
:eProjectTypes
::No Description Available

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==CityPurchaseUnit==
''<summary>''

'''Usage'''

void Game.cityPurchase([[Lua Game Objects/City|<City>]] pCity, [[Lua Game Objects/UnitTypes|UnitTypes]] eUnitType, [[Lua Game Objects/BuildingTypes|BuildingTypes]] eBuildingType, [[Lua Game Objects/ProjectTypes|ProjectTypes]] [[Lua Game Objects/eProjectTypes|eProjectTypes]]);

'''Parameters'''

:pCity
::No Description Available
:eUnitType
::No Description Available
:eBuildingType
::No Description Available
:eProjectTypes
::No Description Available

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==CityPushOrder==
''<summary>''

'''Usage'''

void Game.cityPushOrder([[Lua Game Objects/City|<City>]] pCity, [[Lua Game Objects/OrderTypes|OrderTypes]] eOrder, int iData, boolean bAlt, boolean bShift, boolean bCtrl);

'''Parameters'''

:pCity
::No Description Available
:eOrder
::No Description Available
:iData
::No Description Available
:bAlt
::No Description Available
:bShift
::No Description Available
:bCtrl
::No Description Available

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==CountCivPlayersAlive==
''<summary>''

'''Usage'''

int Game.CountCivPlayersAlive();

'''Parameters'''

None

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==CountCivPlayersEverAlive==
''<summary>''

'''Usage'''

int Game.CountCivPlayersEverAlive();

'''Parameters'''

None

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==CountCivTeamsAlive==
''<summary>''

'''Usage'''

int Game.CountCivTeamsAlive();

'''Parameters'''

None

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==CountCivTeamsEverAlive==
''<summary>''

'''Usage'''

int Game.CountCivTeamsEverAlive();

'''Parameters'''

None

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==CountHumanPlayersAlive==
''<summary>''

'''Usage'''

int Game.countHumanPlayersAlive();

'''Parameters'''

None

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==CountHumanPlayersEverAlive==
''<summary>''

'''Usage'''

int Game.countHumanPlayersEverAlive();

'''Parameters'''

None

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==CountKnownTechNumTeams==
''<summary>''

'''Usage'''

int Game.countKnownTechNumTeams([[Lua Game Objects/TechTypes|TechTypes]] eTech);

'''Parameters'''

:eTech
::No Description Available

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==CountNumHumanGameTurnActive==
''<summary>''

'''Usage'''

int Game.countNumHumanGameTurnActive();

'''Parameters'''

None

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==CountPossibleVote==
''<summary>''

'''Usage'''

int Game.countPossibleVote([[Lua Game Objects/VoteTypes|VoteTypes]] eVote, [[Lua Game Objects/VoteSourceTypes|VoteSourceTypes]] eVoteSource);

'''Parameters'''

:eVote
::No Description Available
:eVoteSource
::No Description Available

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==CountTotalCivPower==
''<summary>''

'''Usage'''

int Game.countTotalCivPower();

'''Parameters'''

None

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==CountTotalNukeUnits==
''<summary>''

'''Usage'''

int Game.countTotalNukeUnits();

'''Parameters'''

None

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==CycleCities==
''<summary>''

'''Usage'''

void Game.cycleCities(boolean bForward, boolean bAdd);

'''Parameters'''

:bForward
::No Description Available
:bAdd
::No Description Available

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==CyclePlotUnits==
''<summary>''

'''Usage'''

boolean Game.cyclePlotUnits([[Lua Game Objects/Plot|<Plot>]] pPlot, boolean bForward, boolean bAuto, int iCount);

'''Parameters'''

:pPlot
::No Description Available
:bForward
::No Description Available
:bAuto
::No Description Available
:iCount
::No Description Available

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==CycleUnits==
''<summary>''

'''Usage'''

void Game.cycleUnits(boolean bClear, boolean bForward, boolean bWorkers);

'''Parameters'''

:bClear
::No Description Available
:bForward
::No Description Available
:bWorkers
::No Description Available

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==DoControl==
''<summary>''

'''Usage'''

void Game.DoControl([[Lua Game Objects/ControlTypes|ControlTypes]] eControl);

'''Parameters'''

:eControl
::No Description Available

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==DoFromUIDiploEvent==
''<summary>''

'''Usage'''

void Game.DoFromUIDiploEvent([[Lua Game Objects/FromUIDiploEventTypes|FromUIDiploEventTypes]] eEvent, [[Lua Game Objects/PlayerTypes|PlayerTypes]] eAIPlayer, int iArg1, int iArg2, int iArg3);

'''Parameters'''

:eEvent
::No Description Available
:eAIPlayer
::No Description Available
:iArg1
::No Description Available
:iArg2
::No Description Available
:iArg3
::No Description Available

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==DoMinorGoldGift==
''<summary>''

'''Usage'''

void Game.DoMinorGoldGift(int iGold);

'''Parameters'''

:iGold
::No Description Available

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==func) RegisterMethod(L, l##func, #func==
''<summary>''

'''Usage'''

void Game.DoMinorGoldGift(int iGold);

'''Parameters'''

:iGold
::No Description Available

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==GameplayDiplomacyAILeaderMessage==
''<summary>''

'''Usage'''

Game.();

'''Parameters'''

:
::No Description Available

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==GetActiveCivilizationType==
''<summary>''

'''Usage'''

[[Lua Game Objects/CivilizationTypes|CivilizationTypes]] Game.getActiveCivilizationType();

'''Parameters'''

None

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==GetActivePlayer==
''<summary>''

'''Usage'''

[[Lua Game Objects/PlayerTypes|PlayerTypes]] Game.getActivePlayer();

'''Parameters'''

None

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==GetActiveTeam==
''<summary>''

'''Usage'''

int Game.getActiveTeam();

'''Parameters'''

None

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==GetAdjustedLandPercent==
''<summary>''

'''Usage'''

int Game.getAdjustedLandPercent([[Lua Game Objects/VictoryTypes|VictoryTypes]] eVictory);

'''Parameters'''

:eVictory
::No Description Available

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==GetAdjustedPopulationPercent==
''<summary>''

'''Usage'''

int Game.getAdjustedPopulationPercent([[Lua Game Objects/VictoryTypes|VictoryTypes]] eVictory);

'''Parameters'''

:eVictory
::No Description Available

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==GetAdvisorCheckFlags==
''<summary>''

'''Usage'''

Game.();

'''Parameters'''

:
::No Description Available

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==GetAdvisorCounsel==
''<summary>''

'''Usage'''

Game.();

'''Parameters'''

:
::No Description Available

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==GetAIAutoPlay==
''<summary>''

'''Usage'''

int Game.getAIAutoPlay();

'''Parameters'''

None

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==GetAllowRClickMovementWhileScrolling==
''<summary>''

'''Usage'''

Game.();

'''Parameters'''

:
::No Description Available

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==GetBestGreatPeoplePlayer==
''<summary>''

'''Usage'''

void Game.GetBestGreatPeoplePlayer();

'''Parameters'''

None

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==GetBestLandUnit==
''<summary>''

'''Usage'''

[[Lua Game Objects/UnitTypes|UnitTypes]] Game.getBestLandUnit();

'''Parameters'''

None

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==GetBestLandUnitCombat==
''<summary>''

'''Usage'''

int Game.getBestLandUnitCombat();

'''Parameters'''

None

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==GetBestPoliciesPlayer==
''<summary>''

'''Usage'''

void Game.GetBestPoliciesPlayer();

'''Parameters'''

None

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==GetBestWondersPlayer==
''<summary>''

'''Usage'''

void Game.GetBestWondersPlayer();

'''Parameters'''

None

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==GetBuildingClassCreatedCount==
''<summary>''

'''Usage'''

int Game.getBuildingClassCreatedCount([[Lua Game Objects/BuildingClassTypes|BuildingClassTypes]] eIndex);

'''Parameters'''

:eIndex
::No Description Available

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==GetCalendar==
''<summary>''

'''Usage'''

[[Lua Game Objects/CalendarTypes|CalendarTypes]] Game.getCalendar();

'''Parameters'''

None

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==GetCurrentEra==
''<summary>''

'''Usage'''

[[Lua Game Objects/EraTypes|EraTypes]] Game.getCurrentEra();

'''Parameters'''

None

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==GetCustomOption==
''<summary>''

'''Usage'''

Game.();

'''Parameters'''

:
::No Description Available

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==GetDiploResponse==
''<summary>''

'''Usage'''

string Game.GetDiploResponse( leaderType,  responseType);

'''Parameters'''

:leaderType
::No Description Available
:responseType
::No Description Available

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==GetElapsedGameTurns==
''<summary>''

'''Usage'''

int Game.getElapsedGameTurns();

'''Parameters'''

None

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==GetEstimateEndTurn==
''<summary>''

'''Usage'''

int Game.getEstimateEndTurn();

'''Parameters'''

None

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==GetGameSpeedType==
''<summary>''

'''Usage'''

[[Lua Game Objects/GameSpeedTypes|GameSpeedTypes]] Game.getGameSpeedType();

'''Parameters'''

None

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==GetGameState==
''<summary>''

'''Usage'''

[[Lua Game Objects/GameStateTypes|GameStateTypes]] Game.getGameState();

'''Parameters'''

None

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==GetGameTurn==
''<summary>''

'''Usage'''

int Game.getGameTurn();

'''Parameters'''

None

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==GetGameTurnYear==
''<summary>''

'''Usage'''

int Game.getGameTurnYear();

'''Parameters'''

None

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==GetHandicapType==
''<summary>''

'''Usage'''

[[Lua Game Objects/HandicapTypes|HandicapTypes]] Game.getHandicapType();

'''Parameters'''

None

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==GetImprovementUpgradeTime==
''<summary>''

'''Usage'''

int Game.getImprovementUpgradeTime([[Lua Game Objects/ImprovementTypes|ImprovementTypes]] eImprovement, [[Lua Game Objects/Plot|<Plot>]] pPlot);

'''Parameters'''

:eImprovement
::No Description Available
:pPlot
::No Description Available

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==GetInitLand==
''<summary>''

'''Usage'''

int Game.getInitLand();

'''Parameters'''

None

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==GetInitPopulation==
''<summary>''

'''Usage'''

int Game.getInitPopulation();

'''Parameters'''

None

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==GetInitTech==
''<summary>''

'''Usage'''

int Game.getInitTech();

'''Parameters'''

None

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==GetInitWonders==
''<summary>''

'''Usage'''

int Game.getInitWonders();

'''Parameters'''

None

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==GetMaxCityElimination==
''<summary>''

'''Usage'''

int Game.getMaxCityElimination();

'''Parameters'''

None

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==GetMaxLand==
''<summary>''

'''Usage'''

int Game.getMaxLand();

'''Parameters'''

None

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==GetMaxPopulation==
''<summary>''

'''Usage'''

int Game.getMaxPopulation();

'''Parameters'''

None

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==GetMaxTech==
''<summary>''

'''Usage'''

int Game.getMaxTech();

'''Parameters'''

None

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==GetMaxTurns==
''<summary>''

'''Usage'''

int Game.getMaxTurns();

'''Parameters'''

None

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==GetMaxWonders==
''<summary>''

'''Usage'''

int Game.getMaxWonders();

'''Parameters'''

None

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==GetMinutesPlayed==
''<summary>''

'''Usage'''

int Game.getMinutesPlayed();

'''Parameters'''

None

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==GetName==
''<summary>''

'''Usage'''

wstring Game.getName();

'''Parameters'''

None

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==GetNoNukesCount==
''<summary>''

'''Usage'''

int Game.getNoNukesCount();

'''Parameters'''

None

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==GetNukesExploded==
''<summary>''

'''Usage'''

int Game.getNukesExploded();

'''Parameters'''

None

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==GetNumAdvancedStartPoints==
''<summary>''

'''Usage'''

int Game.getNumAdvancedStartPoints();

'''Parameters'''

None

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==GetNumCities==
''<summary>''

'''Usage'''

int Game.getNumCities();

'''Parameters'''

None

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==GetNumCivCities==
''<summary>''

'''Usage'''

int Game.getNumCivCities();

'''Parameters'''

None

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==GetNumGameTurnActive==
''<summary>''

'''Usage'''

int Game.getNumGameTurnActive();

'''Parameters'''

None

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==GetNumHumanPlayers==
''<summary>''

'''Usage'''

int Game.getNumHumanPlayers();

'''Parameters'''

None

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==GetNumReplayMessages==
''<summary>''

'''Usage'''

uint Game.getNumReplayMessages();

'''Parameters'''

None

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==GetNumResourceRequiredForBuilding==
''<summary>''

'''Usage'''

Game.();

'''Parameters'''

:
::No Description Available

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==GetNumResourceRequiredForUnit==
''<summary>''

'''Usage'''

Game.();

'''Parameters'''

:
::No Description Available

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==GetNumVictoryVotesTallied==
''<summary>''

'''Usage'''

int Game.GetNumVictoryVotesTallied();

'''Parameters'''

None

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==GetNumVotesForTeam==
''<summary>''

'''Usage'''

int Game.GetNumVotesForTeam();

'''Parameters'''

None

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==GetNumWorldWonders==
''<summary>''

'''Usage'''

int Game.GetNumWorldWonders();

'''Parameters'''

None

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==GetPausePlayer==
''<summary>''

'''Usage'''

int Game.getPausePlayer();

'''Parameters'''

None

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==GetPitbossTurnTime==
''<summary>''

'''Usage'''

int Game.getPitbossTurnTime();

'''Parameters'''

None

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==GetPlayerRank==
''<summary>''

'''Usage'''

int Game.getPlayerRank([[Lua Game Objects/PlayerTypes|PlayerTypes]] iIndex);

'''Parameters'''

:iIndex
::No Description Available

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==GetPlayerScore==
''<summary>''

'''Usage'''

int Game.getPlayerScore([[Lua Game Objects/PlayerTypes|PlayerTypes]] iIndex);

'''Parameters'''

:iIndex
::No Description Available

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==GetPlayerVote==
''<summary>''

'''Usage'''

int Game.getPlayerVote([[Lua Game Objects/PlayerTypes|PlayerTypes]] eOwnerIndex, int iVoteId);

'''Parameters'''

:eOwnerIndex
::No Description Available
:iVoteId
::No Description Available

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==GetProductionPerPopulation==
''<summary>''

'''Usage'''

int Game.getProductionPerPopulation([[Lua Game Objects/HurryTypes|HurryTypes]] eHurry);

'''Parameters'''

:eHurry
::No Description Available

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==GetProjectCreatedCount==
''<summary>''

'''Usage'''

int Game.getProjectCreatedCount([[Lua Game Objects/ProjectTypes|ProjectTypes]] eIndex);

'''Parameters'''

:eIndex
::No Description Available

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==GetRankPlayer==
''<summary>''

'''Usage'''

[[Lua Game Objects/PlayerTypes|PlayerTypes]] Game.getRankPlayer(int iRank);

'''Parameters'''

:iRank
::No Description Available

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==GetRankTeam==
''<summary>''

'''Usage'''

[[Lua Game Objects/TeamTypes|TeamTypes]] Game.getRankTeam(int iRank);

'''Parameters'''

:iRank
::No Description Available

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==GetReplayInfo==
''<summary>''

'''Usage'''

Game.getReplayInfo();

'''Parameters'''

None

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==GetReplayMessageColor==
''<summary>''

'''Usage'''

[[Lua Game Objects/ColorTypes|ColorTypes]] Game.getReplayMessageColor(int i);

'''Parameters'''

:i
::No Description Available

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==GetReplayMessagePlayer==
''<summary>''

'''Usage'''

int Game.getReplayMessagePlayer(int i);

'''Parameters'''

:i
::No Description Available

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==GetReplayMessagePlotX==
''<summary>''

'''Usage'''

int Game.getReplayMessagePlotX(int i);

'''Parameters'''

:i
::No Description Available

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==GetReplayMessagePlotY==
''<summary>''

'''Usage'''

int Game.getReplayMessagePlotY(int i);

'''Parameters'''

:i
::No Description Available

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==GetReplayMessageText==
''<summary>''

'''Usage'''

wstring Game.getReplayMessageText(int i);

'''Parameters'''

:i
::No Description Available

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==GetReplayMessageTurn==
''<summary>''

'''Usage'''

int Game.getReplayMessageTurn(int i);

'''Parameters'''

:i
::No Description Available

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==GetReplayMessageType==
''<summary>''

'''Usage'''

[[Lua Game Objects/ReplayMessageTypes|ReplayMessageTypes]] Game.getReplayMessageType(int i);

'''Parameters'''

:i
::No Description Available

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==GetResourceUsageType==
''<summary>''

'''Usage'''

Game.();

'''Parameters'''

:
::No Description Available

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==GetScriptData==
''<summary>''

'''Usage'''

string Game.getScriptData();

'''Parameters'''

None

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==GetSecretaryGeneral==
''<summary>''

'''Usage'''

int Game.getSecretaryGeneral([[Lua Game Objects/VoteSourceTypes|VoteSourceTypes]] eVoteSource);

'''Parameters'''

:eVoteSource
::No Description Available

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==GetSecretaryGeneralTimer==
''<summary>''

'''Usage'''

int Game.getSecretaryGeneralTimer(int iVoteSource);

'''Parameters'''

:iVoteSource
::No Description Available

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==GetStartEra==
''<summary>''

'''Usage'''

[[Lua Game Objects/EraTypes|EraTypes]] Game.getStartEra();

'''Parameters'''

None

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==GetStartTurn==
''<summary>''

'''Usage'''

int Game.getStartTurn();

'''Parameters'''

None

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==GetStartYear==
''<summary>''

'''Usage'''

int Game.getStartYear();

'''Parameters'''

None

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==GetTargetScore==
''<summary>''

'''Usage'''

int Game.getTargetScore();

'''Parameters'''

None

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==GetTeamRank==
''<summary>''

'''Usage'''

int Game.getTeamRank([[Lua Game Objects/TeamTypes|TeamTypes]] iIndex);

'''Parameters'''

:iIndex
::No Description Available

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==GetTeamScore==
''<summary>''

'''Usage'''

int Game.getTeamScore([[Lua Game Objects/TeamTypes|TeamTypes]] iIndex);

'''Parameters'''

:iIndex
::No Description Available

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==GetTotalPopulation==
''<summary>''

'''Usage'''

int Game.getTotalPopulation();

'''Parameters'''

None

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==GetTurnSlice==
''<summary>''

'''Usage'''

int Game.getTurnSlice();

'''Parameters'''

None

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==GetTurnYear==
''<summary>''

'''Usage'''

int Game.getTurnYear(int iGameTurn);

'''Parameters'''

:iGameTurn
::No Description Available

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==GetTutorialLevel==
''<summary>''

'''Usage'''

Game.();

'''Parameters'''

:
::No Description Available

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==GetUnitClassCreatedCount==
''<summary>''

'''Usage'''

int Game.getUnitClassCreatedCount([[Lua Game Objects/UnitClassTypes|UnitClassTypes]] eIndex);

'''Parameters'''

:eIndex
::No Description Available

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==GetUnitCreatedCount==
''<summary>''

'''Usage'''

int Game.getUnitCreatedCount([[Lua Game Objects/UnitTypes|UnitTypes]] eIndex);

'''Parameters'''

:eIndex
::No Description Available

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==GetUnitedNationsCountdown==
''<summary>''

'''Usage'''

boolean Game.GetUnitedNationsCountdown();

'''Parameters'''

None

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==GetVictory==
''<summary>''

'''Usage'''

[[Lua Game Objects/VictoryTypes|VictoryTypes]] Game.getVictory();

'''Parameters'''

None

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==GetVoteCast==
''<summary>''

'''Usage'''

[[Lua Game Objects/TeamTypes|TeamTypes]] Game.GetVoteCast();

'''Parameters'''

None

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==GetVoteOutcome==
''<summary>''

'''Usage'''

int Game.getVoteOutcome([[Lua Game Objects/VoteTypes|VoteTypes]] eIndex);

'''Parameters'''

:eIndex
::No Description Available

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==GetVoteRequired==
''<summary>''

'''Usage'''

int Game.getVoteRequired([[Lua Game Objects/VoteTypes|VoteTypes]] eVote, [[Lua Game Objects/VoteSourceTypes|VoteSourceTypes]] eVoteSource);

'''Parameters'''

:eVote
::No Description Available
:eVoteSource
::No Description Available

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==GetVotesNeededForDiploVictory==
''<summary>''

'''Usage'''

int Game.GetVotesNeededForDiploVictory();

'''Parameters'''

None

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==GetVoteTimer==
''<summary>''

'''Usage'''

int Game.getVoteTimer(int iVoteSource);

'''Parameters'''

:iVoteSource
::No Description Available

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==GetWinner==
''<summary>''

'''Usage'''

[[Lua Game Objects/TeamTypes|TeamTypes]] Game.getWinner();

'''Parameters'''

None

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==GetWinningTurn==
''<summary>''

'''Usage'''

int Game.GetWinningTurn();

'''Parameters'''

None

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==GoldenAgeLength==
''<summary>''

'''Usage'''

int Game.goldenAgeLength();

'''Parameters'''

None

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==HandleAction==
''<summary>''

'''Usage'''

void Game.HandleAction( iAction);

'''Parameters'''

:iAction
::No Description Available

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==IsBuildingClassMaxedOut==
''<summary>''

'''Usage'''

boolean Game.isBuildingClassMaxedOut([[Lua Game Objects/BuildingClassTypes|BuildingClassTypes]] eIndex, int iExtra);

'''Parameters'''

:eIndex
::No Description Available
:iExtra
::No Description Available

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==IsBuildingEverActive==
''<summary>''

'''Usage'''

boolean Game.isBuildingEverActive([[Lua Game Objects/BuildingTypes|BuildingTypes]] eBuilding);

'''Parameters'''

:eBuilding
::No Description Available

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==IsBuildingRecommended==
''<summary>''

'''Usage'''

Game.();

'''Parameters'''

:
::No Description Available

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==IsChooseElection==
''<summary>''

'''Usage'''

boolean Game.isChooseElection([[Lua Game Objects/VoteTypes|VoteTypes]] eVote);

'''Parameters'''

:eVote
::No Description Available

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==IsCircumnavigated==
''<summary>''

'''Usage'''

boolean Game.isCircumnavigated();

'''Parameters'''

None

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==IsCivEverActive==
''<summary>''

'''Usage'''

boolean Game.isCivEverActive([[Lua Game Objects/CivilizationTypes|CivilizationTypes]] eCivilization);

'''Parameters'''

:eCivilization
::No Description Available

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==IsCombatWarned==
''<summary>''

'''Usage'''

Game.();

'''Parameters'''

:
::No Description Available

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==IsDebugMode==
''<summary>''

'''Usage'''

boolean Game.isDebugMode();

'''Parameters'''

None

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==IsDiploVote==
''<summary>''

'''Usage'''

boolean Game.isDiploVote([[Lua Game Objects/VoteSourceTypes|VoteSourceTypes]] eVoteSource);

'''Parameters'''

:eVoteSource
::No Description Available

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==IsEverAttackedTutorial==
''<summary>''

'''Usage'''

Game.();

'''Parameters'''

:
::No Description Available

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==IsEverRightClickMoved==
''<summary>''

'''Usage'''

Game.();

'''Parameters'''

:
::No Description Available

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==IsFinalInitialized==
''<summary>''

'''Usage'''

boolean Game.isFinalInitialized();

'''Parameters'''

None

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==IsGameMultiPlayer==
''<summary>''

'''Usage'''

boolean Game.isGameMultiPlayer();

'''Parameters'''

None

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==IsHotSeat==
''<summary>''

'''Usage'''

boolean Game.isHotSeat();

'''Parameters'''

None

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==IsInAdvancedStart==
''<summary>''

'''Usage'''

boolean Game.isInAdvancedStart();

'''Parameters'''

None

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==IsLeaderEverActive==
''<summary>''

'''Usage'''

boolean Game.isLeaderEverActive([[Lua Game Objects/LeaderHeadTypes|LeaderHeadTypes]] eLeader);

'''Parameters'''

:eLeader
::No Description Available

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==IsMPOption==
''<summary>''

'''Usage'''

boolean Game.isMPOption([[Lua Game Objects/MultiplayerOptionTypes|MultiplayerOptionTypes]] eIndex);

'''Parameters'''

:eIndex
::No Description Available

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==IsNetworkMultiPlayer==
''<summary>''

'''Usage'''

boolean Game.isNetworkMultiPlayer();

'''Parameters'''

None

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==IsNoNukes==
''<summary>''

'''Usage'''

boolean Game.isNoNukes();

'''Parameters'''

None

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==IsNukesValid==
''<summary>''

'''Usage'''

boolean Game.isNukesValid();

'''Parameters'''

None

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==IsOption==
''Retrieves the state of a specified Game Option<br>Use with [[Lua_Game_Objects/Game#SetOption|Game.SetOption]]''

'''Usage'''

boolean Game.isOption([[Lua Game Objects/GameOptionTypes|GameOptionTypes]] eIndex);

'''Parameters'''

:eIndex
::No Description Available

''' Returns'''

No Description Available.

'''Example'''

<pre>
Game.IsOption(GameOptionTypes.GAMEOPTION_NO_GOODY_HUTS);
</pre>

==IsPaused==
''<summary>''

'''Usage'''

boolean Game.isPaused();

'''Parameters'''

None

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==IsPbem==
''<summary>''

'''Usage'''

boolean Game.isPbem();

'''Parameters'''

None

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==IsPitboss==
''<summary>''

'''Usage'''

boolean Game.isPitboss();

'''Parameters'''

None

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==IsProjectMaxedOut==
''<summary>''

'''Usage'''

boolean Game.isProjectMaxedOut([[Lua Game Objects/ProjectTypes|ProjectTypes]] eIndex, int iExtra);

'''Parameters'''

:eIndex
::No Description Available
:iExtra
::No Description Available

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==IsProjectRecommended==
''<summary>''

'''Usage'''

Game.();

'''Parameters'''

:
::No Description Available

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==IsScoreDirty==
''<summary>''

'''Usage'''

boolean Game.isScoreDirty();

'''Parameters'''

None

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==IsSimultaneousTeamTurns==
''<summary>''

'''Usage'''

boolean Game.isSimultaneousTeamTurns();

'''Parameters'''

None

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==IsSpecialUnitValid==
''<summary>''

'''Usage'''

boolean Game.isSpecialUnitValid([[Lua Game Objects/SpecialUnitTypes|SpecialUnitTypes]] eSpecialUnitType);

'''Parameters'''

:eSpecialUnitType
::No Description Available

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==IsStaticTutorialActive==
''<summary>''

'''Usage'''

Game.();

'''Parameters'''

:
::No Description Available

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==IsTeamGame==
''<summary>''

'''Usage'''

boolean Game.isTeamGame();

'''Parameters'''

None

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==IsTeamVote==
''<summary>''

'''Usage'''

boolean Game.isTeamVote([[Lua Game Objects/VoteTypes|VoteTypes]] eVote);

'''Parameters'''

:eVote
::No Description Available

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==IsTeamVoteEligible==
''<summary>''

'''Usage'''

boolean Game.isTeamVoteEligible([[Lua Game Objects/TeamTypes|TeamTypes]] eTeam, [[Lua Game Objects/VoteSourceTypes|VoteSourceTypes]] eVoteSource);

'''Parameters'''

:eTeam
::No Description Available
:eVoteSource
::No Description Available

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==IsTechRecommended==
''<summary>''

'''Usage'''

Game.();

'''Parameters'''

:
::No Description Available

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==IsTutorialDebugging==
''<summary>''

'''Usage'''

Game.();

'''Parameters'''

:
::No Description Available

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==IsTutorialLogging==
''<summary>''

'''Usage'''

Game.();

'''Parameters'''

:
::No Description Available

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==IsUnitClassMaxedOut==
''<summary>''

'''Usage'''

boolean Game.isUnitClassMaxedOut([[Lua Game Objects/UnitClassTypes|UnitClassTypes]] eIndex, int iExtra);

'''Parameters'''

:eIndex
::No Description Available
:iExtra
::No Description Available

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==IsUnitEverActive==
''<summary>''

'''Usage'''

boolean Game.isUnitEverActive([[Lua Game Objects/UnitTypes|UnitTypes]] eUnit);

'''Parameters'''

:eUnit
::No Description Available

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==IsUnitRecommended==
''<summary>''

'''Usage'''

Game.();

'''Parameters'''

:
::No Description Available

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==IsVictoryValid==
''<summary>''

'''Usage'''

boolean Game.isVictoryValid([[Lua Game Objects/VictoryTypes|VictoryTypes]] eIndex);

'''Parameters'''

:eIndex
::No Description Available

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==IsVotePassed==
''<summary>''

'''Usage'''

boolean Game.isVotePassed([[Lua Game Objects/VoteTypes|VoteTypes]] eIndex);

'''Parameters'''

:eIndex
::No Description Available

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==MakeCircumnavigated==
''<summary>''

'''Usage'''

void Game.makeCircumnavigated();

'''Parameters'''

None

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==MakeNukesValid==
''<summary>''

'''Usage'''

void Game.makeNukesValid(boolean bValid);

'''Parameters'''

:bValid
::No Description Available

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==MakeSpecialUnitValid==
''<summary>''

'''Usage'''

void Game.makeSpecialUnitValid([[Lua Game Objects/SpecialUnitTypes|SpecialUnitTypes]] eSpecialUnitType);

'''Parameters'''

:eSpecialUnitType
::No Description Available

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==Rand==
''<summary>''

'''Usage'''

int Game.Rand( max_num,  log);

'''Parameters'''

:max_num
::No Description Available
:log
::No Description Available

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==ReviveActivePlayer==
''<summary>''

'''Usage'''

void Game.ReviveActivePlayer();

'''Parameters'''

None

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==SaveReplay==
''<summary>''

'''Usage'''

void Game.saveReplay(int iPlayer);

'''Parameters'''

:iPlayer
::No Description Available

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==SelectedCitiesGameNetMessage==
''<summary>''

'''Usage'''

void Game.selectedCitiesGameNetMessage(int eMessage, int iData2, int iData3, int iData4, boolean bOption, boolean bAlt, boolean bShift, boolean bCtrl);

'''Parameters'''

:eMessage
::No Description Available
:iData2
::No Description Available
:iData3
::No Description Available
:iData4
::No Description Available
:bOption
::No Description Available
:bAlt
::No Description Available
:bShift
::No Description Available
:bCtrl
::No Description Available

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==SelectionListGameNetMessage==
''<summary>''

'''Usage'''

void Game.selectionListGameNetMessage(int eMessage, int iData2 = -1, int iData3 = -1, int iData4 = -1, int iFlags = 0, boolean bAlt = false, boolean bShift = false);

'''Parameters'''

:eMessage
::No Description Available
:iData2
::No Description Available
:iData3
::No Description Available
:iData4
::No Description Available
:iFlags
::No Description Available
:bAlt
::No Description Available
:bShift
::No Description Available

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==SelectionListMove==
''<summary>''

'''Usage'''

void Game.selectionListMove([[Lua Game Objects/Plot|<Plot>]] pPlot, boolean bAlt, boolean bShift, boolean bCtrl);

'''Parameters'''

:pPlot
::No Description Available
:bAlt
::No Description Available
:bShift
::No Description Available
:bCtrl
::No Description Available

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==SetActivePlayer==
''<summary>''

'''Usage'''

void Game.setActivePlayer([[Lua Game Objects/PlayerTypes|PlayerTypes]] eNewValue, boolean bForceHotSeat);

'''Parameters'''

:eNewValue
::No Description Available
:bForceHotSeat
::No Description Available

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==SetAdvisorCheckFlags==
''<summary>''

'''Usage'''

Game.();

'''Parameters'''

:
::No Description Available

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==SetAdvisorRecommenderCity==
''<summary>''

'''Usage'''

Game.();

'''Parameters'''

:
::No Description Available

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==SetAdvisorRecommenderTech==
''<summary>''

'''Usage'''

Game.();

'''Parameters'''

:
::No Description Available

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==SetAIAutoPlay==
''<summary>''

'''Usage'''

void Game.setAIAutoPlay(int iNewValue);

'''Parameters'''

:iNewValue
::No Description Available

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==SetCombatWarned==
''<summary>''

'''Usage'''

Game.();

'''Parameters'''

:
::No Description Available

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==SetDebugMode==
''<summary>''

'''Usage'''

boolean Game.setDebugMode();

'''Parameters'''

None

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==SetEstimateEndTurn==
''<summary>''

'''Usage'''

void Game.setEstimateEndTurn(int iNewValue);

'''Parameters'''

:iNewValue
::No Description Available

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==SetEverRightClickMoved==
''<summary>''

'''Usage'''

Game.();

'''Parameters'''

:
::No Description Available

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==SetGameTurn==
''<summary>''

'''Usage'''

void Game.setGameTurn(int iNewValue);

'''Parameters'''

:iNewValue
::No Description Available

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==SetMaxCityElimination==
''<summary>''

'''Usage'''

void Game.setMaxCityElimination(int iNewValue);

'''Parameters'''

:iNewValue
::No Description Available

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==SetMaxTurns==
''<summary>''

'''Usage'''

void Game.setMaxTurns(int iNewValue);

'''Parameters'''

:iNewValue
::No Description Available

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==SetName==
''<summary>''

'''Usage'''

void Game.setName( szName);

'''Parameters'''

:szName
::No Description Available

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==SetNumAdvancedStartPoints==
''<summary>''

'''Usage'''

void Game.setNumAdvancedStartPoints(int iNewValue);

'''Parameters'''

:iNewValue
::No Description Available

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==SetOption==
''Sets the state of a specified Game Option<br>Can use with [[Lua_Game_Objects/Game#IsOption|Game.IsOption]] to get the state of a Game Option''

'''Usage'''

void Game.setOption([[Lua Game Objects/GameOptionTypes|GameOptionTypes]] eIndex, boolean bEnabled);

'''Parameters'''

:eIndex
::[[Lua Game Objects/GameOptionTypes|GameOptionTypes]] ID
:bEnabled
::Set Game Option on (true) or off (false)

''' Returns'''

No Description Available.

'''Example'''

<pre>
Game.SetOption(GameOptionTypes.GAMEOPTION_NO_GOODY_HUTS, true);
</pre>

==SetPausePlayer==
''<summary>''

'''Usage'''

Game.();

'''Parameters'''

:
::No Description Available

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==SetPitbossTurnTime==
''<summary>''

'''Usage'''

void Game.setPitbossTurnTime(int iHours);

'''Parameters'''

:iHours
::No Description Available

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==SetPlotExtraYield==
''<summary>''

'''Usage'''

void Game.setPlotExtraYield(int iX, int iY, [[Lua Game Objects/YieldTypes|YieldTypes]] eYield, int iExtraYield);

'''Parameters'''

:iX
::No Description Available
:iY
::No Description Available
:eYield
::No Description Available
:iExtraYield
::No Description Available

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==SetScoreDirty==
''<summary>''

'''Usage'''

void Game.setScoreDirty(boolean bNewValue);

'''Parameters'''

:bNewValue
::No Description Available

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==SetScriptData==
''<summary>''

'''Usage'''

void Game.setScriptData(string szNewValue);

'''Parameters'''

:szNewValue
::No Description Available

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==SetStartYear==
''<summary>''

'''Usage'''

void Game.setStartYear(int iNewValue);

'''Parameters'''

:iNewValue
::No Description Available

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==SetStaticTutorialActive==
''<summary>''

'''Usage'''

Game.();

'''Parameters'''

:
::No Description Available

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==SetTargetScore==
''<summary>''

'''Usage'''

void Game.setTargetScore(int iNewValue);

'''Parameters'''

:iNewValue
::No Description Available

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==SetWinner==
''<summary>''

'''Usage'''

void Game.setWinner([[Lua Game Objects/TeamTypes|TeamTypes]] eNewWinner, [[Lua Game Objects/VictoryTypes|VictoryTypes]] eNewVictory);

'''Parameters'''

:eNewWinner
::No Description Available
:eNewVictory
::No Description Available

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==ToggleDebugMode==
''<summary>''

'''Usage'''

void Game.toggleDebugMode();

'''Parameters'''

None

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==UpdateFOW==
''<summary>''

'''Usage'''

void Game.UpdateFOW();

'''Parameters'''

None

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==UpdateScore==
''<summary>''

'''Usage'''

void Game.updateScore(boolean bForce);

'''Parameters'''

:bForce
::No Description Available

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==VictoryDelay==
''<summary>''

'''Usage'''

int Game.victoryDelay([[Lua Game Objects/VictoryTypes|VictoryTypes]] eVictory);

'''Parameters'''

:eVictory
::No Description Available

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>