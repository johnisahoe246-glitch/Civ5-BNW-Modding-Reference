Up: [[Lua Game Objects]]


For the related events, see [[Lua Game Events#City|Lua Game Events (City)]]

Methods:

==Ownership==
*[[GetOriginalOwner]]
*[[GetOwner]]
*[[GetPreviousOwner]]
*[[GetTeam]]
*[[IsEverOwned]]
*[[IsNeverLost]]
*[[SetNeverLost]]

==State==
*[[IsOccupied]]
*[[IsPuppet]]
*[[SetOccupied]]
*[[SetPuppet]]
===Razing===
*[[ChangeRazingTurns]]
*[[GetRazingTurns]]
*[[IsRazing]]
===Resistance===
*[[ChangeResistanceTurns]]
*[[GetResistanceTurns]]
*[[IsResistance]]
===We Love The King Day===
*[[GetWeLoveTheKingDayCounter]]
*[[ChangeWeLoveTheKingDayCounter]]
*[[SetWeLoveTheKingDayCounter]]

==Misc==
===Get===
*[[GetArtStyleType]]
*[[GetCivilizationType]]
*[[GetFocusType]]
*[[GetGameTurnAcquired]]
*[[GetGameTurnFounded]]
*[[GetGameTurnLastExpanded]]
*[[GetID]]
*[[GetName]]
*[[GetNameKey]]
*[[GetPersonalityType]]
*[[IsBarbarian]]
*[[IsBlockaded]]
*[[IsCapital]]
*[[IsCoastal]]
*[[IsHuman]]
*[[IsNoOccupiedUnhappiness]]
*[[IsRevealed]](TeamTypes eIndex, boolean bDebug)
*[[IsVisible]](TeamTypes eTeam, boolean bDebug)
===Set===
*[[Kill]]
*[[SetFocusType]]
*[[SetName]]
*[[SetRevealed]](TeamTypes eIndex, boolean bNewValue)
*[[SetScriptData]]

==Population==
===Get===
*[[FindPopulationRank]]
*[[GetHighestPopulation]]
*[[GetPopulation]]()
*[[GetRealPopulation]]
*[[GetYieldPerPopTimes100]]
===Set===
*[[ChangePopulation]]
*[[SetHighestPopulation]]
*[[SetPopulation]](int iNewValue, bool flag)

==Buildings==
===Wonders/Projects===
*[[CanCreate]](int iProject, boolean bContinue, boolean bTestVisible)
*[[CreateApolloProgram]]
*[[GetNumNationalWonders]]
*[[GetNumTeamWonders]]
*[[GetNumWorldWonders]]
*[[IsNationalWondersMaxed]]
*[[IsTeamWondersMaxed]]
*[[IsWorldWondersMaxed]]
===Get===
*[[CanConstruct]](int iBuilding, boolean bContinue, boolean bTestVisible, boolean bIgnoreCost)
*[[CanConstructTooltip]]
*[[GetBuildingDefense]]
*[[GetBuildingOriginalOwner]]
*[[GetBuildingOriginalTime]]
*[[GetBuildingProduction]]
*[[GetBuildingProductionNeeded]]
*[[GetBuildingProductionTime]]
*[[GetBuildingProductionTurnsLeft]]
*[[GetNumActiveBuilding]]
*[[GetNumBuilding]]
*[[GetNumBuildings]]
*[[GetNumFreeBuilding]]
*[[GetNumRealBuilding]]
*[[GetNumSpecialistsAllowedByBuilding]]
*[[GetNumSpecialistsInBuilding]]
*[[GetProductionBuilding]]
*[[GetSellBuildingRefund]]
*[[GetTotalBaseBuildingMaintenance]]
*[[IsBuildingLocalResourceValid]]
*[[IsBuildingSellable]]
*[[IsBuildingsMaxed]]
*[[IsCanAddSpecialistToBuilding]]
*[[IsHasBuilding]](buildingID) - returns true if a subject city has a building with a specified ID 
*[[IsProductionBuilding]]
===Set===
*[[ChangeBuildingProduction]]
*[[ChangeBuildingProductionTime]]
*[[SetBuildingProduction]]
*[[SetBuildingProductionTime]]
*[[SetNumRealBuilding]]

==Yields==
===Get===
*[[FindBaseYieldRateRank]]
*[[FindYieldRateRank]]
*[[GetBaseYieldRate]]
*[[GetBaseYieldRateFromBuildings]]
*[[GetBaseYieldRateFromMisc]]
*[[GetBaseYieldRateFromSpecialists]]
*[[GetBaseYieldRateFromTerrain]]
*[[GetBaseYieldRateModifier]]
*[[GetBuildingYieldChange]]
*[[GetExtraSpecialistYield]]
*[[GetExtraSpecialistYieldOfType]]
*[[GetLakePlotYield]]
*[[GetResourceYieldRateModifier]]
*[[GetRiverPlotYield]]
*[[GetSeaPlotYield]]
*[[GetSpecialistYield]]
*[[GetYieldModifierTooltip]]
*[[GetYieldPerPopTimes100]]
*[[GetYieldRate]]
*[[GetYieldRateModifier]]
*[[GetYieldRateTimes100]]
===Set===
*[[ChangeBaseYieldRateFromBuildings]]
*[[ChangeBaseYieldRateFromMisc]]
*[[ChangeBaseYieldRateFromSpecialists]]
*[[ChangeBaseYieldRateFromTerrain]]
*[[SetBuildingYieldChange]]

==Food==
===Growth===
*[[GrowthThreshold]]
*[[IsForcedAvoidGrowth]]
===Get===
*[[FoodConsumption]]
*[[FoodDifference]]
*[[FoodDifferenceTimes100]]
*[[GetFood]]
*[[GetFoodKept]]
*[[GetFoodTimes100]]
*[[GetFoodTurnsLeft]]
*[[GetMaxFoodKeptPercent]]
*[[IsFoodProduction]]
*[[IsUnitFoodProduction]]
===Set===
*[[ChangeFood]]
*[[SetFood]]

==Production==
*[[CanMaintain]](int iProcess, boolean bContinue)
===Modifiers===
*[[ChangeWonderProductionModifier]]
*[[GetBuildingProductionModifier]]
*[[GetDomainProductionModifier]]
*[[GetMilitaryProductionModifier]]
*[[GetProductionModifier]]
*[[GetProjectProductionModifier]]
*[[GetSpaceProductionModifier]]
*[[GetUnitProductionModifier]]
*[[GetWonderProductionModifier]]
===Production Queue===
*[[GetFirstBuildingOrder]]
*[[GetFirstProjectOrder]]
*[[GetFirstSpecialistOrder]]
*[[GetFirstUnitOrder]]
*[[GetOrderFromQueue]]
*[[GetOrderQueueLength]]
*[[ClearOrderQueue]]
*[[PopOrder]]
*[[PushOrder]]
===Get===
*[[CanContinueProduction]]
*[[GetBuildingProduction]]
*[[GetBuildingProductionModifier]]
*[[GetBuildingProductionNeeded]]
*[[GetBuildingProductionTime]]
*[[GetBuildingProductionTurnsLeft]]
*[[GetCurrentProductionDifference]]
*[[GetCurrentProductionDifferenceTimes100]]
*[[GetDomainProductionModifier]]
*[[GetExtraProductionDifference]]
*[[GetFeatureProduction]]
*[[GetGeneralProductionTurnsLeft]]
*[[GetLocalResourceWonderProductionMod]]
*[[GetMilitaryProductionModifier]]
*[[GetOverflowProduction]]
*[[GetProduction]]
*[[GetProductionBuilding]]
*[[GetProductionExperience]]
*[[GetProductionModifier]]
*[[GetProductionNameKey]]
*[[GetProductionNeeded]]
*[[GetProductionProcess]]
*[[GetProductionProject]]
*[[GetProductionSpecialist]]
*[[GetProductionTimes100]]
*[[GetProductionTurnsLeft]]
*[[GetProductionUnit]]
*[[GetProductionUnitAI]]
*[[GetProjectProductionModifier]]
*[[GetProjectProductionNeeded]]
*[[GetProjectProductionTurnsLeft]]
*[[GetSpaceProductionModifier]]
*[[GetSpecialistProductionModifier]]
*[[GetSpecialistProductionTurnsLeft]]
*[[GetUnitProduction]]
*[[GetUnitProductionModifier]]
*[[GetUnitProductionNeeded]]
*[[GetUnitProductionTurnsLeft]]
*[[GetWonderProductionModifier]]
*[[IsFoodProduction]]
*[[IsProduction]]
*[[IsProductionAutomated]]
*[[IsProductionBuilding]]
*[[IsProductionLimited]]
*[[IsProductionProcess]]
*[[IsProductionProject]]
*[[IsProductionSpecialist]]
*[[IsProductionUnit]]
*[[IsUnitFoodProduction]]
*[[ProductionLeft]]
===Set===
*[[AddProductionExperience]]
*[[ChangeBuildingProduction]]
*[[ChangeBuildingProductionTime]]
*[[ChangeProduction]]
*[[ChangeUnitProduction]]
*[[ChangeWonderProductionModifier]]
*[[ChooseProduction]]
*[[SetBuildingProduction]]
*[[SetBuildingProductionTime]]
*[[SetFeatureProduction]]
*[[SetOverflowProduction]]
*[[SetProduction]]
*[[SetProductionAutomated]]
*[[SetUnitProduction]]

==Purchase==
*[[GetBuildingPurchaseCost]]
*[[GetPurchaseBuildingTooltip]]
*[[GetPurchaseUnitTooltip]]
*[[GetProjectPurchaseCost]]
*[[GetUnitPurchaseCost]]
*[[IsCanPurchase]]

==Hurry==
*[[CanHurry]](HurryTypes iHurry, boolean bTestVisible)
*[[Hurry]]
*[[HurryCost]]
*[[HurryGold]]
*[[HurryPopulation]]
*[[HurryProduction]]
*[[MaxHurryPopulation]]

==Culture==
===Get===
*[[GetBaseJONSCulturePerTurn]]
*[[GetCultureFromSpecialist]]
*[[GetCultureRateModifier]]
*[[GetCultureUpdateTimer]]
*[[GetJONSCultureLevel]]
*[[GetJONSCulturePerTurn]]
*[[GetJONSCulturePerTurnFromBuildings]]
*[[GetJONSCulturePerTurnFromPolicies]]
*[[GetJONSCulturePerTurnFromSpecialists]]
*[[GetJONSCulturePerTurnFromTerrain]]
*[[GetJONSCulturePerTurnFromTraits]]
*[[GetJONSCultureStored]]
*[[GetJONSCultureThreshold]]
===Set===
*[[ChangeCultureRateModifier]]
*[[ChangeCultureUpdateTimer]]
*[[ChangeJONSCultureLevel]]
*[[ChangeJONSCulturePerTurnFromBuildings]]
*[[ChangeJONSCulturePerTurnFromPolicies]]
*[[ChangeJONSCulturePerTurnFromSpecialists]]
*[[ChangeJONSCulturePerTurnFromTerrain]]
*[[ChangeJONSCultureStored]]
*[[DoJONSCultureLevelIncrease]]
*[[SetJONSCultureLevel]]
*[[SetJONSCultureStored]]

==Plots==
===Location===
*[[Area]]
*[[At]](int iX, int iY)
*[[AtPlot]](pPlot) - returns boolean.
*[[GetCityIndexPlot]](int iIndex)
*[[GetCityPlotIndex]]
*[[GetX]]
*[[GetY]]
*[[IsCoastal]]
*[[Plot]]
*[[WaterArea]]
===Get===
*[[CanBuyAnyPlot]]
*[[CanBuyPlot]]
*[[CanBuyPlotAt]]
*[[CanWork]](pPlot)
*[[CountNumImprovedPlots]]
*[[CountNumRiverPlots]]
*[[CountNumWaterPlots]]
*[[GetBuyPlotCost]]
*[[GetLakePlotYield]]
*[[GetNextBuyablePlot]]
*[[GetNumCityPlots]]
*[[GetNumForcedWorkingPlots]]
*[[GetRallyPlot]]
*[[GetRiverPlotYield]]
*[[GetSeaPlotYield]]
*[[IsForcedWorkingPlot]]
*[[IsPlotBlockaded]]
*[[IsWorkingPlot]]
===Set===
*[[AlterWorkingPlot]]
*[[DoReallocateCitizens]]()
*[[DoVerifyWorkingPlots]]

==Resources==
*[[DoPickResourceDemanded]]
*[[GetResourceDemanded]]
*[[IsHasResourceLocal]]
*[[SetResourceDemanded]]

==Specialists==
*[[CanPrepare]](int iSpecialist, boolean bContinue)
===Get===
*[[GetBaseYieldRateFromSpecialists]]
*[[GetCultureFromSpecialist]]
*[[GetExtraSpecialistYield]]
*[[GetExtraSpecialistYieldOfType]]
*[[GetJONSCulturePerTurnFromSpecialists]]
*[[GetNumSpecialistsAllowedByBuilding]]
*[[GetNumSpecialistsInBuilding]]
*[[GetProductionSpecialist]]
*[[GetSpecialistCount]]
*[[GetSpecialistFreeExperience]]
*[[GetSpecialistGreatPersonProgress]]
*[[GetSpecialistGreatPersonProgressTimes100]]
*[[GetSpecialistProductionModifier]]
*[[GetSpecialistProductionTurnsLeft]]
*[[GetSpecialistUpgradeThreshold]]
*[[GetSpecialistYield]]
===Set===
*[[ChangeBaseYieldRateFromSpecialists]]
*[[ChangeJONSCulturePerTurnFromSpecialists]]
*[[ChangeSpecialistGreatPersonProgressTimes100]]
*[[IsCanAddSpecialistToBuilding]]
*[[IsNoAutoAssignSpecialists]]
*[[IsProductionSpecialist]]

==Great People==
===Get===
*[[GetBaseGreatPeopleRate]]
*[[GetGreatPeopleProgress]]
*[[GetGreatPeopleRate]]
*[[GetGreatPeopleRateModifier]]
*[[GetGreatPeopleUnitProgress]]
*[[GetGreatPeopleUnitRate]]
*[[GetNumGreatPeople]]
*[[GetSpecialistGreatPersonProgress]]
*[[GetSpecialistGreatPersonProgressTimes100]]
*[[GetTotalGreatPeopleRateModifier]]
===Set===
*[[ChangeBaseGreatPeopleRate]]
*[[ChangeGreatPeopleProgress]]
*[[ChangeGreatPeopleUnitProgress]]
*[[ChangeSpecialistGreatPersonProgressTimes100]]
*[[CreateGreatGeneral]]
*[[SetGreatPeopleUnitProgress]]

==Units==
*[[CanTrain]](int iUnit, boolean bContinue, boolean bTestVisible, boolean bIgnoreCost, boolean bIgnoreUpgrades)
*[[CanTrainTooltip]]
===Get===
*[[AllUpgradesAvailable]](UnitTypes eUnit, int iUpgradeCount = 0)
*[[GetGarrisonedUnit]]
*[[GetNumTrainUnitAI]]
*[[GetProductionUnit]]
*[[GetProductionUnitAI]]
*[[GetUnitProduction]]
*[[GetUnitProductionModifier]]
*[[GetUnitProductionNeeded]]
*[[GetUnitProductionTurnsLeft]]
*[[GetRallyPlot]]
*[[IsProductionUnit]]
*[[IsUnitFoodProduction]]
===Set===
*[[ChangeUnitProduction]]
*[[SetUnitProduction]]
===Experience===
*[[GetDomainFreeExperience]]
*[[GetFreeExperience]]
*[[GetFreePromotionCount]]
*[[GetSpecialistFreeExperience]]
*[[GetUnitCombatFreeExperience]]
*[[IsFreePromotion]]

==Combat==
*[[GetAirModifier]]
*[[GetNukeModifier]]
*[[GetStrengthValue]]
*[[UpdateStrengthValue]]
===Ranged Strike===
*[[CanRangeStrike]]
*[[CanRangeStrikeAt]](int x, int y)
*[[CanRangeStrikeNow]]
*[[HasPerformedRangedStrikeThisTurn]]
===Hit Points===
*[[ChangeDamage]]
*[[ChangeHealRate]]
*[[GetDamage]]
*[[SetDamage]]

==Air Lift==
*[[GetCurrAirlift]]
*[[GetMaxAirlift]]
*[[IsAirliftTargeted]]
*[[SetAirliftTargeted]]

==Conscription==
*[[CanConscript]]
*[[Conscript]]
*[[ConscriptMinCityPopulation]]
*[[GetConscriptPopulation]]
*[[GetConscriptUnit]]
*[[IsDrafted]]
*[[SetDrafted]]

==Unsorted==
*[[CanJoin]]
*[[ClearWorkingOverride]](int iIndex)
*[[DoTask]](TaskTypes eTask, int iData1, int iData2, boolean bOption)
*[[GetCitySizeType]]
*[[GetHandicapType]]
*[[IsNone]]
*[[SetCitySizeBoost]](int iBoost)