=Civ5buildings.xml=
*The Civ5buildings.xml file contains definitions for the Buildings.
*The reference field in the tables below indicates the table and column the entry is linked to.
*This information is taken from the Civ5buildings.xml file itself.
==Buildings==
*[[CIV5BuildingClasses]] contains the definitions of the BuildingClasses referenced in this table.
*[[CIV5Terrains]] contains the definitions of the Terrains referenced in this table.
*[[CIV5Victories]] contains the definitions of the Victories referenced in this table.
*[[CIV5Eras]] contains the definitions of the Eras referenced in this table.
*[[CIV5Technologies]] contains the definitions of the Technologies referenced in this table.
*[[CIV5UnitPromotions]] contains the definitions of the UnitPromotions referenced in this table.
*[[CIV5Specialists]] contains the definitions of the Specialists referenced in this table.
*[[CIV5IconTextureAtlases]] contains the definitions of the IconTextureAtlases referenced in this table.
{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"
|+Buildings Table
! scope="col" style="background: #efefef;" | Name
! scope="col" style="background: #efefef;" | Type
! scope="col" style="background: #efefef;" | Reference
! scope="col" style="background: #efefef;" | Default
! scope="col" style="background: #efefef;" | Notes
|-
| ID || integer|| || || Primary Key,Autoincrement
|-
| Type || text|| || || Not Null,Unique
|-
| Description || text|| Language_en_US(Tag)|| || 
|-
| Civilopedia || text|| Language_en_US(Tag)|| || 
|-
| Strategy || text|| Language_en_US(Tag)|| || 
|-
| Help || text|| Language_en_US(Tag)|| || 
|-
| Quote || text|| Language_en_US(Tag)|| || 
|-
| GoldMaintenance || integer|| || 0|| The ammout of gold the building deducts from your income each turn
|-
| MutuallyExclusiveGroup || integer|| || -1|| 
|-
| TeamShare || boolean|| || false|| 
|-
| Water || boolean|| || false|| 
|-
| River || boolean|| || false|| Requires that the city be built next to a river
|-
| FreshWater || boolean|| || false|| Requires that the city be built next to a river or fresh water lake
|-
| Mountain || boolean|| || false|| Requires that the city be built next to a mountain
|-
| NearbyMountainRequired || boolean|| || false|| Requires that a mountain be within the city's borders
|-
| Hill || boolean|| || false|| Requires that the city be built on a hill
|-
| Flat || boolean|| || false|| Requires that the city not be built on a hill
|-
| FoundsReligion || boolean|| || false|| 
|-
| IsReligious || boolean|| || false|| 
|-
| BorderObstacle || boolean|| || false|| The owner's territory costs 1 more movement point for enemy units (global effect)
|-
| Capital || boolean|| || false|| The Building can only be built in the capital if True
|-
| GoldenAge || boolean|| || false|| 
|-
| MapCentering || boolean|| || false|| 
|-
| NeverCapture || boolean|| || false|| 
|-
| NukeImmune || boolean|| || false|| 
|-
| AllowsWaterRoutes || boolean|| || false|| Allows trade routes over water
|-
| ExtraLuxuries || boolean|| || false|| 
|-
| DiplomaticVoting || boolean|| || false|| 
|-
| Cost || integer|| || 0|| 
|-
| NumCityCostMod || integer|| || 0|| 
|-
| HurryCostModifier || integer|| || 0|| 
|-
| MinAreaSize || integer|| || 0|| 
|-
| ConquestProb || integer|| || 0|| 
|-
| CitiesPrereq || integer|| || 0|| 
|-
| LevelPrereq || integer|| || 0|| 
|-
| Culture || integer|| || 0|| 
|-
| CultureRateModifier || integer|| || 0|| 
|-
| GlobalCultureRateModifier || integer|| || 0|| 
|-
| GreatPeopleRateModifier || integer|| || 0|| 
|-
| GlobalGreatPeopleRateModifier || integer|| || 0|| 
|-
| GreatGeneralRateModifier || integer|| || 0|| 
|-
| GoldenAgeModifier || integer|| || 0|| 
|-
| UnitUpgradeCostMod || integer|| || 0|| 
|-
| Experience || integer|| || 0|| 
|-
| GlobalExperience || integer|| || 0|| 
|-
| FoodKept || integer|| || 0|| 
|-
| Airlift || integer|| || 0|| 
|-
| AirModifier || integer|| || 0|| 
|-
| NukeModifier || integer|| || 0|| 
|-
| NukeExplosionRand || integer|| || 0|| 
|-
| HealRateChange || integer|| || 0|| 
|-
| Happiness || integer|| || 0|| 
|-
| HappinessPerCity || integer|| || 0|| 
|-
| CityCountUnhappinessMod || integer|| || 0|| 
|-
| NoOccupiedUnhappiness || boolean|| || false|| 
|-
| WorkerSpeedModifier || integer|| || 0|| 
|-
| MilitaryProductionModifier || integer|| || 0|| 
|-
| SpaceProductionModifier || integer|| || 0|| 
|-
| BuildingProductionModifier || integer|| || 0|| 
|-
| WonderProductionModifier || integer|| || 0|| 
|-
| TradeRouteModifier || integer|| || 0|| 
|-
| CapturePlunderModifier || integer|| || 0|| 
|-
| PolicyCostModifier || integer|| || 0|| 
|-
| PlotCultureCostModifier || integer|| || 0|| 
|-
| GlobalPopulationChange || integer|| || 0|| 
|-
| TechShare || integer|| || 0|| 
|-
| FreeTechs || integer|| || 0|| 
|-
| FreePolicies || integer|| || 0|| 
|-
| Gold || integer|| || 0|| 
|-
| AllowsRangeStrike || boolean|| || false|| 
|-
| Defense || integer|| || 0|| 
|-
| GlobalDefenseMod || integer|| || 0|| 
|-
| MinorFriendshipChange || integer|| || 0|| 
|-
| VictoryPoints || integer|| || 0|| 
|-
| BuildingClass || text|| BuildingClasses(Type)|| NULL|| 
|-
| ArtDefineTag || text|| || NULL|| 
|-
| NearbyTerrainRequired || text|| Terrains(Type)|| NULL|| The specified terrain must exist within the city's borders
|-
| VictoryPrereq || text|| Victories(Type)|| NULL|| 
|-
| FreeStartEra || text|| Eras(Type)|| NULL|| 
|-
| MaxStartEra || text|| Eras(Type)|| NULL|| 
|-
| ObsoleteTech || text|| Technologies(Type)|| NULL|| 
|-
| EnhancedYieldTech || text|| Technologies(Type)|| NULL|| 
|-
| FreeBuilding || text|| BuildingClasses(Type)|| NULL|| 
|-
| FreePromotion || text|| UnitPromotions(Type)|| NULL|| 
|-
| TrainedFreePromotion || text|| UnitPromotions(Type)|| NULL|| 
|-
| ReplacementBuildingClass || text|| BuildingClasses(Type)|| NULL|| 
|-
| PrereqTech || text|| Technologies(Type)|| NULL|| 
|-
| SpecialistType || text|| Specialists(Type)|| NULL|| 
|-
| SpecialistCount || integer|| || 0|| 
|-
| SpecialistExtraCulture || integer|| || 0|| |Attention: Seems to be broken in 1.0.1.141, see [http://forums.civfanatics.com/showthread.php?t=404816| here]
|-
| GreatPeopleRateChange || integer|| || 0|| 
|-
| CityWall || boolean|| || false|| 
|-
| DisplayPosition || integer|| || 0|| 
|-
| PortraitIndex || integer|| || -1|| 
|-
| WonderSplashImage || text|| || NULL|| 
|-
| WonderSplashAnchor || text|| || R,T|| 
|-
| WonderSplashAudio || text|| || || 
|-
| IconAtlas || text|| IconTextureAtlases(Atlas)|| NULL|| 
|-
| ArtInfoCulturalVariation || boolean|| || false|| 
|-
| ArtInfoEraVariation || boolean|| || false|| 
|-
| ArtInfoRandomVariation || boolean|| || false|| 
|}

==Building_AreaYieldModifiers==
*[[CIV5Yields]] contains the definitions of the Yields referenced in this table.
{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"
|+Building_AreaYieldModifiers Table
! scope="col" style="background: #efefef;" | Name
! scope="col" style="background: #efefef;" | Type
! scope="col" style="background: #efefef;" | Reference
|-
| BuildingType || text|| Buildings(Type)
|-
| YieldType || text|| Yields(Type)
|-
| Yield || integer|| 
|}
==Building_ClassesNeededInCity==
*[[CIV5BuildingClasses]] contains the definitions of the BuildingClasses referenced in this table.
{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"
|+Building_ClassesNeededInCity Table
! scope="col" style="background: #efefef;" | Name
! scope="col" style="background: #efefef;" | Type
! scope="col" style="background: #efefef;" | Reference
|-
| BuildingType || text|| Buildings(Type)
|-
| BuildingClassType || text|| BuildingClasses(Type)
|}
==Building_FreeUnits==
*[[CIV5Units]] contains the definitions of the Units referenced in this table.
{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"
|+Building_FreeUnits Table
! scope="col" style="background: #efefef;" | Name
! scope="col" style="background: #efefef;" | Type
! scope="col" style="background: #efefef;" | Reference
|-
| BuildingType || text|| Buildings(Type)
|-
| UnitType || text|| Units(Type)
|-
| NumUnits || integer|| 
|}
==Building_DomainFreeExperiences==
*[[CIV5Domains]] contains the definitions of the Domains referenced in this table.
{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"
|+Building_DomainFreeExperiences Table
! scope="col" style="background: #efefef;" | Name
! scope="col" style="background: #efefef;" | Type
! scope="col" style="background: #efefef;" | Reference
|-
| BuildingType || text|| Buildings(Type)
|-
| DomainType || text|| Domains(Type)
|-
| Experience || integer|| 
|}
==Building_DomainProductionModifiers==
*[[CIV5Domains]] contains the definitions of the Domains referenced in this table.
{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"
|+Building_DomainProductionModifiers Table
! scope="col" style="background: #efefef;" | Name
! scope="col" style="background: #efefef;" | Type
! scope="col" style="background: #efefef;" | Reference
|-
| BuildingType || text|| Buildings(Type)
|-
| DomainType || text|| Domains(Type)
|-
| Modifier || integer|| 
|}
==Building_FreeSpecialistCounts==
*[[CIV5Specialists]] contains the definitions of the Specialists referenced in this table. Attention: Seems to be not functional in 1.0.1.141, see [http://forums.civfanatics.com/showthread.php?t=404816| here]
{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"
|+Building_FreeSpecialistCounts Table
! scope="col" style="background: #efefef;" | Name
! scope="col" style="background: #efefef;" | Type
! scope="col" style="background: #efefef;" | Reference
|-
| BuildingType || text|| Buildings(Type)
|-
| SpecialistType || text|| Specialists(Type)
|-
| Count || integer|| 
|}

==Building_Flavors==
*[[CIV5Flavors]] contains the definitions of the Flavors referenced in this table.
{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"
|+Building_Flavors Table
! scope="col" style="background: #efefef;" | Name
! scope="col" style="background: #efefef;" | Type
! scope="col" style="background: #efefef;" | Reference
|-
| BuildingType || text|| Buildings(Type)
|-
| FlavorType || text|| Flavors(Type)
|-
| Flavor || integer|| 
|}
==Building_GlobalYieldModifiers==
*[[CIV5Yields]] contains the definitions of the Yields referenced in this table.
{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"
|+Building_GlobalYieldModifiers Table
! scope="col" style="background: #efefef;" | Name
! scope="col" style="background: #efefef;" | Type
! scope="col" style="background: #efefef;" | Reference
|-
| BuildingType || text|| Buildings(Type)
|-
| YieldType || text|| Yields(Type)
|-
| Yield || integer|| 
|}
==Building_HurryModifiers==
*[[CIV5HurryInfos]] contains the definitions of the HurryInfos referenced in this table.
{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"
|+Building_HurryModifiers Table
! scope="col" style="background: #efefef;" | Name
! scope="col" style="background: #efefef;" | Type
! scope="col" style="background: #efefef;" | Reference
|-
| BuildingType || text|| Buildings(Type)
|-
| HurryType || text|| HurryInfos(Type)
|-
| HurryCostModifier || integer|| 
|}
==Building_LocalResourceAnds==
*[[CIV5Resources]] contains the definitions of the Resources referenced in this table.
{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"
|+Building_LocalResourceAnds Table
! scope="col" style="background: #efefef;" | Name
! scope="col" style="background: #efefef;" | Type
! scope="col" style="background: #efefef;" | Reference
|-
| BuildingType || text|| Buildings(Type)
|-
| ResourceType || text|| Resources(Type)
|}
==Building_LocalResourceOrs==
*[[CIV5Resources]] contains the definitions of the Resources referenced in this table.
{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"
|+Building_LocalResourceOrs Table
! scope="col" style="background: #efefef;" | Name
! scope="col" style="background: #efefef;" | Type
! scope="col" style="background: #efefef;" | Reference
|-
| BuildingType || text|| Buildings(Type)
|-
| ResourceType || text|| Resources(Type)
|}
==Building_LockedBuildingClasses==
*[[CIV5BuildingClasses]] contains the definitions of the BuildingClasses referenced in this table.
{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"
|+Building_LockedBuildingClasses Table
! scope="col" style="background: #efefef;" | Name
! scope="col" style="background: #efefef;" | Type
! scope="col" style="background: #efefef;" | Reference
|-
| BuildingType || text|| Buildings(Type)
|-
| BuildingClassType || text|| BuildingClasses(Type)
|}
==Building_PrereqBuildingClasses==
*[[CIV5BuildingClasses]] contains the definitions of the BuildingClasses referenced in this table.
{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"
|+Building_PrereqBuildingClasses Table
! scope="col" style="background: #efefef;" | Name
! scope="col" style="background: #efefef;" | Type
! scope="col" style="background: #efefef;" | Reference
|-
| BuildingType || text|| Buildings(Type)
|-
| BuildingClassType || text|| BuildingClasses(Type)
|-
| NumBuildingNeeded || integer|| 
|}
==Building_ResourceQuantityRequirements==
*[[CIV5Resources]] contains the definitions of the Resources referenced in this table.
{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"
|+Building_ResourceQuantityRequirements Table
! scope="col" style="background: #efefef;" | Name
! scope="col" style="background: #efefef;" | Type
! scope="col" style="background: #efefef;" | Reference
|-
| BuildingType || text|| Buildings(Type)
|-
| ResourceType || text|| Resources(Type)
|-
| Cost || integer|| 
|}
==Building_ResourceYieldModifiers==
*[[CIV5Resources]] contains the definitions of the Resources referenced in this table.
*[[CIV5Yields]] contains the definitions of the Yields referenced in this table.
{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"
|+Building_ResourceYieldModifiers Table
! scope="col" style="background: #efefef;" | Name
! scope="col" style="background: #efefef;" | Type
! scope="col" style="background: #efefef;" | Reference
|-
| BuildingType || text|| Buildings(Type)
|-
| ResourceType || text|| Resources(Type)
|-
| YieldType || text|| Yields(Type)
|-
| Yield || integer|| 
|}
==Building_ResourceCultureChanges==
*[[CIV5Resources]] contains the definitions of the Resources referenced in this table.
{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"
|+Building_ResourceCultureChanges Table
! scope="col" style="background: #efefef;" | Name
! scope="col" style="background: #efefef;" | Type
! scope="col" style="background: #efefef;" | Reference
|-
| BuildingType || text|| Buildings(Type)
|-
| ResourceType || text|| Resources(Type)
|-
| CultureChange || integer|| 
|}
==Building_RiverPlotYieldChanges==
*[[CIV5Yields]] contains the definitions of the Yields referenced in this table.
{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"
|+Building_RiverPlotYieldChanges Table
! scope="col" style="background: #efefef;" | Name
! scope="col" style="background: #efefef;" | Type
! scope="col" style="background: #efefef;" | Reference
|-
| BuildingType || text|| Buildings(Type)
|-
| YieldType || text|| Yields(Type)
|-
| Yield || integer|| 
|}
==Building_SeaPlotYieldChanges==
*[[CIV5Yields]] contains the definitions of the Yields referenced in this table.
{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"
|+Building_SeaPlotYieldChanges Table
! scope="col" style="background: #efefef;" | Name
! scope="col" style="background: #efefef;" | Type
! scope="col" style="background: #efefef;" | Reference
|-
| BuildingType || text|| Buildings(Type)
|-
| YieldType || text|| Yields(Type)
|-
| Yield || integer|| 
|}
==Building_LakePlotYieldChanges==
*[[CIV5Yields]] contains the definitions of the Yields referenced in this table.
{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"
|+Building_LakePlotYieldChanges Table
! scope="col" style="background: #efefef;" | Name
! scope="col" style="background: #efefef;" | Type
! scope="col" style="background: #efefef;" | Reference
|-
| BuildingType || text|| Buildings(Type)
|-
| YieldType || text|| Yields(Type)
|-
| Yield || integer|| 
|}
==Building_SeaResourceYieldChanges==
*[[CIV5Yields]] contains the definitions of the Yields referenced in this table.
{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"
|+Building_SeaResourceYieldChanges Table
! scope="col" style="background: #efefef;" | Name
! scope="col" style="background: #efefef;" | Type
! scope="col" style="background: #efefef;" | Reference
|-
| BuildingType || text|| Buildings(Type)
|-
| YieldType || text|| Yields(Type)
|-
| Yield || integer|| 
|}
==Building_ResourceYieldChanges==
*[[CIV5Resources]] contains the definitions of the Resources referenced in this table.
*[[CIV5Yields]] contains the definitions of the Yields referenced in this table.
{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"
|+Building_ResourceYieldChanges Table
! scope="col" style="background: #efefef;" | Name
! scope="col" style="background: #efefef;" | Type
! scope="col" style="background: #efefef;" | Reference
|-
| BuildingType || text|| Buildings(Type)
|-
| ResourceType || text|| Resources(Type)
|-
| YieldType || text|| Yields(Type)
|-
| Yield || integer|| 
|}
==Building_FeatureYieldChanges==
*[[CIV5Features]] contains the definitions of the Features referenced in this table.
*[[CIV5Yields]] contains the definitions of the Yields referenced in this table.
{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"
|+Building_FeatureYieldChanges Table
! scope="col" style="background: #efefef;" | Name
! scope="col" style="background: #efefef;" | Type
! scope="col" style="background: #efefef;" | Reference
|-
| BuildingType || text|| Buildings(Type)
|-
| FeatureType || text|| Features(Type)
|-
| YieldType || text|| Yields(Type)
|-
| Yield || integer|| 
|}
==Building_SpecialistYieldChanges==
*[[CIV5Specialists]] contains the definitions of the Specialists referenced in this table.
*[[CIV5Yields]] contains the definitions of the Yields referenced in this table.
{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"
|+Building_SpecialistYieldChanges Table
! scope="col" style="background: #efefef;" | Name
! scope="col" style="background: #efefef;" | Type
! scope="col" style="background: #efefef;" | Reference
|-
| BuildingType || text|| Buildings(Type)
|-
| SpecialistType || text|| Specialists(Type)
|-
| YieldType || text|| Yields(Type)
|-
| Yield || integer|| 
|}
==Building_UnitCombatFreeExperiences==
*[[CIV5UnitCombatInfos]] contains the definitions of the UnitCombatInfos referenced in this table.
{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"
|+Building_UnitCombatFreeExperiences Table
! scope="col" style="background: #efefef;" | Name
! scope="col" style="background: #efefef;" | Type
! scope="col" style="background: #efefef;" | Reference
|-
| BuildingType || text|| Buildings(Type)
|-
| UnitCombatType || text|| UnitCombatInfos(Type)
|-
| Experience || integer|| 
|}
==Building_UnitCombatProductionModifiers==
*[[CIV5UnitCombatInfos]] contains the definitions of the UnitCombatInfos referenced in this table.
{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"
|+Building_UnitCombatProductionModifiers Table
! scope="col" style="background: #efefef;" | Name
! scope="col" style="background: #efefef;" | Type
! scope="col" style="background: #efefef;" | Reference
|-
| BuildingType || text|| Buildings(Type)
|-
| UnitCombatType || text|| UnitCombatInfos(Type)
|-
| Modifier || integer|| 
|}
==Building_TechAndPrereqs==
*[[CIV5Technologies]] contains the definitions of the Technologies referenced in this table.
{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"
|+Building_TechAndPrereqs Table
! scope="col" style="background: #efefef;" | Name
! scope="col" style="background: #efefef;" | Type
! scope="col" style="background: #efefef;" | Reference
|-
| BuildingType || text|| Buildings(Type)
|-
| TechType || text|| Technologies(Type)
|}
==Building_YieldChanges==
*[[CIV5Yields]] contains the definitions of the Yields referenced in this table.
{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"
|+Building_YieldChanges Table
! scope="col" style="background: #efefef;" | Name
! scope="col" style="background: #efefef;" | Type
! scope="col" style="background: #efefef;" | Reference
|-
| BuildingType || text|| Buildings(Type)
|-
| YieldType || text|| Yields(Type)
|-
| Yield || integer|| 
|}
==Building_YieldChangesPerPop==
*[[CIV5Yields]] contains the definitions of the Yields referenced in this table.
{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"
|+Building_YieldChangesPerPop Table
! scope="col" style="background: #efefef;" | Name
! scope="col" style="background: #efefef;" | Type
! scope="col" style="background: #efefef;" | Reference
|-
| BuildingType || text|| Buildings(Type)
|-
| YieldType || text|| Yields(Type)
|-
| Yield || integer|| 
|}
==Building_TechEnhancedYieldChanges==
*[[CIV5Yields]] contains the definitions of the Yields referenced in this table.
{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"
|+Building_TechEnhancedYieldChanges Table
! scope="col" style="background: #efefef;" | Name
! scope="col" style="background: #efefef;" | Type
! scope="col" style="background: #efefef;" | Reference
|-
| BuildingType || text|| Buildings(Type)
|-
| YieldType || text|| Yields(Type)
|-
| Yield || integer|| 
|}
==Building_YieldModifiers==
*[[CIV5Yields]] contains the definitions of the Yields referenced in this table.
{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"
|+Building_YieldModifiers Table
! scope="col" style="background: #efefef;" | Name
! scope="col" style="background: #efefef;" | Type
! scope="col" style="background: #efefef;" | Reference
|-
| BuildingType || text|| Buildings(Type)
|-
| YieldType || text|| Yields(Type)
|-
| Yield || integer|| 
|}
{{Civ5_XML_Files}}