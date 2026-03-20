Up: [[Lua Game Objects]]


List on the official wiki: http://wiki.2kgames.com/civ5/index.php/Lua_Game_Objects/Player (parameters are listed for many methods).


==Player Info==
===Self===
*[[GetCivilizationType]]() - returns a civilization type value for a major civ player.
*[[GetID]]
*[[GetLeaderType]]
*[[GetPersonality]]
*[[GetPersonalityType]]
*[[GetQueuePosition]]
*[[GetTeam]]
*[[IsAlive]]
*[[IsBarbarian]]
*[[IsEverAlive]]
*[[IsHuman]]
*[[IsMinorCiv]]() - returns true if this is a ciy-state.
*[[IsPlayable]]
*[[SetPersonalityType]]
*[[SetPlayable]]
===Misc===
*[[GetCurrentEra]]
*[[GetTotalTimePlayed]]
*[[GetWorkerSpeedModifier]]
*[[IsFoundedFirstCity]]
*[[IsHasLostCapital]]
===Yields===
*[[CalculateTotalYield]](eYield)
*[[GetExtraYieldThreshold]](YieldTypes eIndex)
*[[GetSpecialistExtraYield]]
*[[GetYieldRateModifier]](YieldTypes eIndex)
*[[SpecialistYield]](eSpecialist, eYield)
===Combat Experience===
*[[ChangeCombatExperience]]
*[[GetCombatExperience]]
*[[SetCombatExperience]](int iExperience)
===Score===
*[[GetLandScore]]
*[[GetPopScore]]
*[[GetScore]]
*[[GetScoreFromCities]]
*[[GetScoreFromFutureTech]]
*[[GetScoreFromLand]]
*[[GetScoreFromPopulation]]
*[[GetScoreFromTechs]]
*[[GetScoreFromWonders]]
*[[GetScoreHistory]]
*[[GetTechScore]]
*[[GetTotalLandScored]]
*[[GetWondersScore]]
===Demographics===
*[[GetEconomyHistory]]
*[[GetIndustryHistory]]
*[[GetMilitaryMight]]
*[[GetPower]]
*[[GetPowerHistory]]
*[[GetTotalLand]]
===Script Data===
*[[GetScriptData]]
*[[SetScriptData]]

==Other Players / Diplomacy==
===City States===
*[[ChangeJONSCulturePerTurnFromMinorCivs]]
*[[ChangeMinorCivFriendshipWithMajor]]
*[[DoMinorLiberationByMajor]]
*[[GetAlly]]
*[[GetCurrentSpawnEstimate]] - military units spawning.
*[[GetFriendshipChangePerTurnTimes100]]
*[[GetFriendshipFromGoldGift]]
*[[GetFriendshipNeededForNextLevel]]
*[[GetHappinessFromMinor]]
*[[GetMinorCivCultureFriendshipBonus]]
*[[GetMinorCivFavoriteMajor]]
*[[GetMinorCivFriendshipLevelWithMajor]]
*[[GetMinorCivFriendshipWithMajor]]
*[[GetMinorCivHappinessFriendshipBonus]]
*[[GetMinorCivScienceFriendshipBonus]]
*[[GetMinorCivTrait]]
*[[GetMinorCivType]]() - returns a civilization type value for a city-state civ player.
*[[GetMinorWarQuestWithMajorRemainingCount]]
*[[GetNumMinorCivsMet]]
*[[GetOtherPlayerNumProtectedMinorsKilled]]
*[[GetQuestData1]]
*[[GetQuestData2]]
*[[GetResourceFromMinors]]
*[[IsAllies]]
*[[IsFriends]]
*[[IsMinorCiv]]() - returns true if this is a city-state.
*[[IsMinorCivRouteEstablishedWithMajor]]
*[[IsMinorCivUnitSpawningDisabled]]
*[[IsMinorPermanentWar]]
*[[IsMinorWarQuestWithMajorActive]]
*[[IsPlayerBrokenCityStatePromise]]
*[[IsPlayerIgnoredCityStatePromise]]
*[[IsProtectingMinor]]
===Dispute level===
*[[GetLandDisputeLevel]]
*[[GetMinorCivDisputeLevel]]
*[[GetVictoryDisputeLevel]]
*[[GetWonderDisputeLevel]]
===Get===
*[[CanContact]]
*[[CanStopTradingWithTeam]]
*[[CanTradeWith]]
*[[GetApproachTowardsUsGuess]](PlayerTypes ePlayer)
*[[GetCoopWarAcceptedState]]
*[[GetNumCiviliansReturned]]
*[[GetProximityToPlayer]]
*[[GetVotes]]
*[[GetWarmongerThreat]]
*[[GetWorstEnemyName]]
*[[IsDemandEverMade]]
*[[IsDenouncedPlayer]]
*[[IsDontSettleMessageTooSoon]]
*[[IsPeaceBlocked]]
*[[IsPlayerBrokenBorderPromise]]
*[[IsPlayerBrokenCityStatePromise]]
*[[IsPlayerBrokenCoopWarPromise]]
*[[IsPlayerBrokenExpansionPromise]]
*[[IsPlayerBrokenMilitaryPromise]]
*[[IsPlayerHasOpenBorders]]
*[[IsPlayerHasOpenBordersAutomatically]]
*[[IsPlayerIgnoredBorderPromise]]
*[[IsPlayerIgnoredCityStatePromise]]
*[[IsPlayerIgnoredExpansionPromise]]
*[[IsPlayerIgnoredMilitaryPromise]]
*[[IsPlayerNoSettleRequestEverAsked]]
*[[IsPlayerRecklessExpander]]
*[[IsWhiteFlag]]
*[[IsWillAcceptPeaceWithPlayer]]
*[[IsWorkingAgainstPlayerAccepted]]
*[[IsWorkingWithPlayer]]
*[[IsWorkingWithPlayerMessageTooSoon]]
===Set===
*[[Contact]]
*[[DoBeginDiploWithHuman]]
*[[DoForceDenounce]]
*[[DoForceDoF]]
*[[DoTradeScreenClosed]]
*[[DoTradeScreenOpened]]
*[[ForcePeace]](int iPlayer)
*[[StopTradingWithTeam]]

==Units==
*[[CanTrain]](eUnit, boolean bContinue, boolean bTestVisible)
===Experience===
*[[GetExpInBorderModifier]]
*[[GetFreeExperience]]
*[[GetHighestUnitLevel]]
===Cost/Supply===
*[[CalculateUnitCost]]
*[[CalculateUnitSupply]]
*[[GetExtraUnitCost]]
*[[GetNumMaintenanceFreeUnits]]
*[[GetNumUnitsOutOfSupply]]
*[[GetNumUnitsSupplied]]
*[[GetNumUnitsSuppliedByCities]]
*[[GetNumUnitsSuppliedByHandicap]]
*[[GetNumUnitsSuppliedByPopulation]]
*[[GetUnitProductionMaintenanceMod]]
===Combat===
*[[GetAttackBonusTurns]]
*[[GetBarbarianCombatBonus]]
*[[GetTraitCityStateCombatModifier]]
*[[GetTraitGoldenAgeCombatModifier]]
*[[SetBarbarianCombatBonus]]
===Numbers===
*[[GetNumMilitaryUnits]]
*[[GetNumNukeUnits]]
*[[GetNumOutsideUnits]]
*[[GetNumUnitGoldenAges]]
*[[GetNumUnits]]
*[[GetUnitClassCount]]
*[[GetUnitClassCountPlusMaking]]
*[[GetUnitClassMaking]]
*[[UnitsGoldenAgeCapable]]
*[[UnitsGoldenAgeReady]]
===Get===
*[[GetFirstReadyUnit]]
*[[GetFirstReadyUnitPlot]]
*[[GetUnitByID]]
*[[GetUnitProductionNeeded]](iUnitTypeUpgrade)
*[[HasBusyMovingUnit]]
*[[HasBusyUnit]]
*[[HasReadyUnit]]
*[[IsProductionMaxedUnitClass]]
*[[IsUnitClassMaxedOut]]
*[[Units]]
*[[UnitsRequiredForGoldenAge]]
===Set===
*[[AddFreeUnit]]
*[[ChangeNumUnitGoldenAges]]
*[[DisbandUnit]]
*[[InitUnit]]
*[[KillUnits]]

==Cities==
*[[CanMaintain]](eProcess, boolean bContinue)
*[[CanPrepare]](eSpecialist, boolean bContinue)
===Get===
*[[CanFound]](int iX, int iY)
*[[CanRaze]](pCity)
*[[Cities]]
*[[CountCityFeatures]]
*[[GetCapitalCity]]
*[[GetCapitalYieldRateModifier]](YieldTypes eIndex)
*[[GetCitiesLost]]
*[[GetCityByID]]
*[[GetCityConnectionGold]]
*[[GetCityConnectionGoldTimes100]]
*[[GetCityCountUnhappinessMod]]
*[[GetCityDefenseModifier]]
*[[GetCityName]]
*[[GetCultureCityModifier]]
*[[GetCurrentOtherCityFoodBonus]]
*[[GetNewCityName]]
*[[GetNextCity]]
*[[GetNumCities]]
*[[GetNumCityNames]]
*[[GetPrevCity]]
*[[IsCapitalConnectedToCity]]
===Set===
*[[AcquireCity]]
*[[AddCityName]]
*[[Disband]](pCity)
*[[FindNewCapital]]
*[[InitCity]]
*[[KillCities]]
*[[Raze]](pCity)

==Population==
*[[GetAveragePopulation]]
*[[GetRealPopulation]]
*[[GetTotalPopulation]]

==Buildings==
*[[CanBuild]]
*[[CanConstruct]](BuildingTypes eBuilding, boolean bContinue, boolean bTestVisible, boolean bIgnoreCost)
===Get===
*[[CountNumBuildings]](eBuilding)
*[[GetAdvancedStartBuildingCost]]
*[[GetBuildingClassCount]]
*[[GetBuildingClassCountPlusMaking]]
*[[GetBuildingClassMaking]]
*[[GetBuildingClassPrereqBuilding]]
*[[GetBuildingGoldMaintenance]]
*[[GetBuildingProductionNeeded]]
*[[GetEverTrainedBuilder]]
*[[GetHappinessFromBuildings]]
*[[GetMaxGlobalBuildingProductionModifier]]
*[[GetMaxPlayerBuildingProductionModifier]]
*[[GetMaxTeamBuildingProductionModifier]]
*[[GetNumWorldWonders]]
*[[IsBuildBlockedByFeature]](eBuild, FeatureTypes eFeature)
*[[IsBuildingClassMaxedOut]]
*[[IsBuildingFree]]
*[[IsProductionMaxedBuildingClass]]
===Set===
*[[ChangeBaseBuildingGoldMaintenance]]
*[[RemoveBuildingClass]]
*[[SetBaseBuildingGoldMaintenance]]

==Food==
*[[GetCurrentCapitalFoodBonus]]
*[[GetCurrentOtherCityFoodBonus]]
*[[IsMilitaryFoodProduction]]

==Production==
*[[GetBuildingProductionNeeded]]
*[[GetFeatureProductionModifier]]
*[[GetMaxGlobalBuildingProductionModifier]]
*[[GetMaxPlayerBuildingProductionModifier]]
*[[GetMaxTeamBuildingProductionModifier]]
*[[GetMilitaryProductionModifier]]
*[[GetProductionModifier]]
*[[GetProjectProductionNeeded]]
*[[GetSettlerProductionModifier]]
*[[GetSpaceProductionModifier]]
*[[GetUnitProductionMaintenanceMod]]
*[[GetUnitProductionNeeded]]
*[[GetWonderProductionModifier]]
*[[IsMilitaryFoodProduction]]
*[[IsProductionMaxedBuildingClass]]
*[[IsProductionMaxedProject]]
*[[IsProductionMaxedUnitClass]]

==Gold==
===Get===
*[[CalculateGoldRate]]
*[[CalculateGoldRateTimes100]]
*[[CalculateGrossGold]]
*[[CalculateGrossGoldTimes100]]
*[[GetBuildingGoldMaintenance]]
*[[GetCityConnectionGold]]
*[[GetCityConnectionGoldTimes100]]
*[[GetGold]]
*[[GetGoldFromCitiesTimes100]]
*[[GetGoldPerMilitaryUnit]]
*[[GetGoldPerTurnFromDiplomacy]]
*[[GetGoldPerUnit]]
*[[GetHurryGoldCost]]
*[[GetImprovementGoldMaintenance]]
*[[GetRouteGoldTimes100]]
===Set===
*[[ChangeBaseBuildingGoldMaintenance]]
*[[ChangeGold]]
*[[ChangeGoldPerUnitTimes100]]
*[[SetBaseBuildingGoldMaintenance]]
*[[SetGold]]

==Science==
===Get===
*[[CalculateResearchModifier]]
*[[CanEverResearch]]
*[[CanResearch]]
*[[FindPathLength]](eTech, boolean bCost)
*[[GetCurrentResearch]]
*[[GetCurrentScienceFriendshipBonusTimes100]] - science from city states.
*[[GetLengthResearchQueue]]
*[[GetMinorCivScienceFriendshipBonus]]
*[[GetNumFreeTechs]]
*[[GetOverflowResearch]]
*[[GetResearchTurnsLeft]]
*[[GetScience]]
*[[GetScienceFromBudgetDeficitTimes100]]
*[[GetScienceFromCitiesTimes100]]
*[[GetScienceFromHappinessTimes100]]
*[[GetScienceFromOtherPlayersTimes100]]
*[[GetScienceFromResearchAgreementsTimes100]]
*[[GetScienceTimes100]]
*[[GetTraitGreatScientistRateModifier]]
*[[IsCurrentResearchRepeat]]
*[[IsNoResearchAvailable]]
*[[IsResearch]]
*[[IsResearchingTech]]
===Set===
*[[ChooseTech]]
*[[ClearResearchQueue]]
*[[PopResearch]]
*[[PushResearch]]
*[[SetNumFreeTechs]]
*[[SetResearchingTech]]

==Culture==
===Get===
*[[GetCultureBombTimer]]
*[[GetCultureCityModifier]]
*[[GetCultureWonderMultiplier]]
*[[GetCurrentCultureBonus]]
*[[GetJONSCulture]]
*[[GetJONSCulturePerTurnForFree]]
*[[GetJONSCulturePerTurnFromCities]]
*[[GetJONSCulturePerTurnFromExcessHappiness]]
*[[GetJONSCulturePerTurnFromMinorCivs]]
*[[GetMinorCivCultureFriendshipBonus]]
*[[GetNumTimesCultureBombed]]
*[[GetTotalJONSCulturePerTurn]]
===Set===
*[[ChangeJONSCulture]]
*[[ChangeJONSCulturePerTurnForFree]]
*[[ChangeJONSCulturePerTurnFromMinorCivs]]
*[[SetJONSCulture]]

==Policies==
===Get===
*[[CanAdoptPolicy]]
*[[CanUnlockPolicyBranch]]
*[[ChangeNumFreePolicies]]
*[[GetHappinessFromPolicies]]
*[[GetNextPolicyCost]]
*[[GetNumFreePolicies]]
*[[GetNumPolicies]]
*[[GetNumPolicyBranchesAllowed]]
*[[GetNumPolicyBranchesFinished]]
*[[GetNumPolicyBranchesUnlocked]]
*[[GetPolicyBranchChosen]]
*[[HasPolicy]](policyID) - returns true if a player has a specified policy. 
*[[IsPolicyBlocked]]
*[[IsPolicyBranchBlocked]]
*[[IsPolicyBranchFinished]]
*[[IsPolicyBranchUnlocked]]
===Set===
*[[DoAdoptPolicy]]
*[[SetHasPolicy]](policyID, bNewValue) - sets player having a specified policy. Increases next policy cost.
*[[SetNumFreePolicies]]
*[[SetPolicyBranchUnlocked]]

==Happiness==
===Get===
*[[GetCapitalUnhappinessMod]]
*[[GetCityCountUnhappinessMod]]
*[[GetExcessHappiness]]() - returns happiness minus unhappiness (whats shown to player on the top panel). If empire is unhappy, it will return a negative value. Otherwise positive or zero.
*[[GetExtraHappinessPerCity]]
*[[GetExtraHappinessPerLuxury]]
*[[GetHappiness]]
*[[GetHappinessFromBuildings]]
*[[GetHappinessFromGarrisonedUnits]]
*[[GetHappinessFromMinor]]
*[[GetHappinessFromNaturalWonders]]
*[[GetHappinessFromPolicies]]
*[[GetHappinessFromReligion]]
*[[GetHappinessFromResources]]
*[[GetHappinessFromResourceVariety]]
*[[GetHappinessFromTradeRoutes]]
*[[GetHappinessPerGarrisonedUnit]]
*[[GetHappinessPerTradeRoute]]
*[[GetHappyPerMilitaryUnit]]
*[[GetMinorCivHappinessFriendshipBonus]]
*[[GetOccupiedPopulationUnhappinessMod]]
*[[GetTraitCityUnhappinessMod]]
*[[GetTraitPopUnhappinessMod]]
*[[GetUnhappiness]]
*[[GetUnhappinessForecast]]
*[[GetUnhappinessFromCapturedCityCount]]
*[[GetUnhappinessFromCityCount]]
*[[GetUnhappinessFromCityForUI]]
*[[GetUnhappinessFromCityPopulation]]
*[[GetUnhappinessFromOccupiedCities]]
*[[GetUnhappinessFromUnits]]
*[[GetUnhappinessMod]]
*[[IsEmpireUnhappy]]
*[[IsEmpireVeryUnhappy]]
*[[IsHalfSpecialistUnhappiness]]
===Set===
*[[ChangeExtraHappinessPerCity]]
*[[ChangeHappinessFromBuildings]]
*[[ChangeHappinessFromGarrisonedUnits]]
*[[ChangeHappinessPerGarrisonedUnit]]
*[[ChangeHappinessPerTradeRoute]]
*[[ChangeUnhappinessFromUnits]]
*[[SetHappiness]](iHappiness) - supposed to set player's happiness, but '''does not work'''
*[[SetHappinessPerGarrisonedUnit]]
*[[SetHappinessPerTradeRoute]]

==GoldenAge==
===Get===
*[[GetGoldenAgeLength]]
*[[GetGoldenAgeModifier]]
*[[GetGoldenAgeProgressMeter]]
*[[GetGoldenAgeProgressThreshold]]
*[[GetGoldenAgeTurns]]
*[[GetNumGoldenAges]]
*[[GetNumUnitGoldenAges]]
*[[GetTraitGoldenAgeCombatModifier]]
*[[IsGoldenAge]]
*[[UnitsGoldenAgeCapable]]
*[[UnitsGoldenAgeReady]]
*[[UnitsRequiredForGoldenAge]]
===Set===
*[[ChangeGoldenAgeProgressMeter]]
*[[ChangeGoldenAgeTurns]]
*[[ChangeNumGoldenAges]]
*[[ChangeNumUnitGoldenAges]]
*[[SetGoldenAgeProgressMeter]]
*[[SetNumGoldenAges]]

==Great People==
===Great General===
*[[GetDomesticGreatGeneralRateModifier]]
*[[GetGreatGeneralRateModifier]]
*[[GetGreatGeneralsCreated]]
*[[GetGreatGeneralsThresholdModifier]]
*[[GetTraitGreatGeneralExtraBonus]]
*[[GreatGeneralThreshold]]
===Get===
*[[GetGreatPeopleCreated]]
*[[GetGreatPeopleRateModifier]]
*[[GetGreatPeopleThresholdModifier]]
*[[GetTraitGreatScientistRateModifier]]
===Set===
*[[CreateGreatGeneral]]
*[[DoGreatPersonChoice]]

==Resources==
===Get===
*[[GetHappinessFromResources]]
*[[GetHappinessFromResourceVariety]]
*[[GetNumResourceAvailable]]
*[[GetNumResourceTotal]]
*[[GetNumResourceUsed]]
*[[GetNumTradeResourceImports]]
*[[GetResourceExport]]
*[[GetResourceFromMinors]]
*[[GetResourceImport]]
*[[GetUnimprovedAvailableLuxuryResource]]
===Set===
*[[ChangeNumResourceTotal]]

==Improvements==
*[[GetImprovementCount]]
*[[GetImprovementGoldMaintenance]]
*[[GetImprovementUpgradeRate]]
*[[GetImprovementUpgradeRateModifier]]
*[[GetUnimprovedAvailableLuxuryResource]]
*[[GetWorkerSpeedModifier]]
*[[IsAnyPlotImproved]]

==Plots==
===Get===
*[[GetBuyPlotCost]]
*[[GetNumPlots]]
*[[GetNumPlotsBought]]
*[[GetPlotDanger]]
*[[GetPlotHasOrder]]
*[[GetRecommendedFoundCityPlots]]
*[[GetRecommendedWorkerPlots]]
*[[GetSeaPlotYield]]
*[[GetStartingPlot]]
===Set===
*[[ChangeNumPlotsBought]]
*[[SetNumPlotsBought]]
*[[SetStartingPlot]]

==Barbarians==
===Get===
*[[GetBarbarianCombatBonus]]
*[[GetTurnsSinceThreatenedByBarbarians]]
*[[IsAlwaysSeeBarbCamps]]
*[[IsBarbarian]]
===Set===
*[[ChangeAlwaysSeeBarbCampsCount]]
*[[ChangeBarbarianCombatBonus]]
*[[SetAlwaysSeeBarbCampsCount]]
*[[SetBarbarianCombatBonus]]

==Goodies==
*[[CanReceiveGoody]]
*[[DoGoody]](pPlot, pUnit)
*[[GetClosestGoodyPlot]]
*[[GetEverPoppedGoody]]
*[[IsAnyGoodyPlotAccessible]]
*[[ReceiveGoody]]

==UI==
===Text===
*[[GetCivilizationAdjective]]
*[[GetCivilizationAdjectiveKey]]
*[[GetCivilizationDescription]]
*[[GetCivilizationDescriptionKey]]
*[[GetCivilizationShortDescription]]
*[[GetCivilizationShortDescriptionKey]]
*[[GetDominantPolicyBranchForTitle]]
*[[GetName]]
*[[GetNameKey]]
*[[GetNickName]]
===Get===
*[[GetArtStyleType]]
*[[GetEndTurnBlockingNotificationIndex]]
*[[GetEndTurnBlockingType]]
*[[GetNotificationDismissed]]
*[[GetNotificationIndex]]
*[[GetNotificationStr]]
*[[GetNotificationSummaryStr]]
*[[GetNotificationTurn]]
*[[GetNumNotifications]]
===Set===
*[[AddNotification]]

==AI==
*[[AI_foundValue]]
*[[AI_updateFoundValues]]

==AdvancedStart==
===Get===
*[[GetAdvancedStartBuildingCost]]
*[[GetAdvancedStartCityCost]]
*[[GetAdvancedStartPoints]]
*[[GetAdvancedStartPopCost]]
*[[GetAdvancedStartRouteCost]]
*[[GetAdvancedStartTechCost]]
*[[GetAdvancedStartUnitCost]]
*[[GetAdvancedStartVisibilityCost]]
===Set===
*[[ChangeAdvancedStartPoints]]
*[[SetAdvancedStartPoints]]

==Unsorted==
*[[CalculateInflatedCosts]]
*[[CanBuild]]
*[[CanCreate]]
*[[Found]](int iX, int iY)
*[[GetBestRoute]](pPlot)
*[[GetBranchPicked1]]
*[[GetBranchPicked2]]
*[[GetBranchPicked3]]
*[[GetConversionTimer]]
*[[GetEverTrainedBuilder]]
*[[GetHandicapType]]
*[[HasReceivedNetTurnComplete]]
*[[IsExtendedGame]]
*[[IsOption]]
*[[IsTurnActive]]
*[[SetOption]]

==Unused==
===Conscription===
*[[ChangeConscriptCount]]
*[[GetConscriptCount]]
*[[GetMaxConscript]]
*[[SetConscriptCount]]
===Hurry===
*[[GetHurryCount]](eIndex)
*[[GetHurryModifier]]
*[[IsCanHurry]]
*[[IsHasAccessToHurry]]
===Anarchy===
*[[ChangeAnarchyNumTurns]]
*[[GetAnarchyNumTurns]]
*[[IsAnarchy]]
*[[SetAnarchyNumTurns]]
===Religion===
*[[GetStateReligionKey]]
*[[GetStateReligionName]]
===Strike===
*[[GetStrikeTurns]]
*[[IsStrike]]
===UN/AP Resolutions===
*[[IsFullMember]]
*[[IsLoyalMember]]
*[[IsVotingMember]]
*[[SetLoyalMember]]


==Related Events==

See [[Lua Game Events#Player|Lua Game Events (Player)]]