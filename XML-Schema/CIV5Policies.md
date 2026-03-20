=CIV5Policies.xml=
*The CIV5Policies.xml file contains definitions for the Policies.
*The reference field in the tables below indicates the table and column the entry is linked to.
*This information is taken from the CIV5Policies.xml file itself.
==Policies==
*[[CIV5PolicyBranchTypes]] contains the definitions of the PolicyBranchTypes referenced in this table.
*[[CIV5Technologies]] contains the definitions of the Technologies referenced in this table.
*[[CIV5IconTextureAtlases]] contains the definitions of the IconTextureAtlases referenced in this table.
{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"
|+Policies Table
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
| Description || text|| Language_en_US(Tag)|| write a bug on this|| 
|-
| Civilopedia || text|| Language_en_US(Tag)|| || 
|-
| Strategy || text|| Language_en_US(Tag)|| || 
|-
| Help || text|| Language_en_US(Tag)|| || 
|-
| PolicyBranchType || text|| PolicyBranchTypes(Type)|| NULL|| 
|-
| NumExtraBranches || integer|| || 0|| 
|-
| CultureCost || integer|| || 0|| 
|-
| GridX || integer|| || 0|| 
|-
| GridY || integer|| || 0|| 
|-
| PolicyCostModifier || integer|| || 0|| 
|-
| CulturePerCity || integer|| || 0|| 
|-
| CulturePerWonder || integer|| || 0|| 
|-
| CultureWonderMultiplier || integer|| || 0|| 
|-
| CulturePerTechResearched || integer|| || 0|| 
|-
| AttackBonusTurns || integer|| || 0|| 
|-
| GoldenAgeTurns || integer|| || 0|| 
|-
| GoldenAgeMeterMod || integer|| || 0|| 
|-
| NumFreeTechs || integer|| || 0|| 
|-
| NumFreePolicies || integer|| || 0|| 
|-
| StrategicResourceMod || integer|| || 0|| 
|-
| ReligionProductionModifier || integer|| || 0|| 
|-
| WonderProductionModifier || integer|| || 0|| 
|-
| BuildingProductionModifier || integer|| || 0|| 
|-
| GreatPeopleRateModifier || integer|| || 0|| 
|-
| GreatGeneralRateModifier || integer|| || 0|| 
|-
| DomesticGreatGeneralRateModifier || integer|| || 0|| 
|-
| ExtraHappiness || integer|| || 0|| 
|-
| ExtraHappinessPerCity || integer|| || 0|| 
|-
| UnhappinessMod || integer|| || 0|| 
|-
| CityCountUnhappinessMod || integer|| || 0|| 
|-
| OccupiedPopulationUnhappinessMod || integer|| || 0|| 
|-
| CapitalUnhappinessMod || integer|| || 0|| 
|-
| FreeExperience || integer|| || 0|| 
|-
| WorkerSpeedModifier || integer|| || 0|| 
|-
| AllFeatureProduction || integer|| || 0|| 
|-
| ImprovementCostModifier || integer|| || 0|| 
|-
| ImprovementUpgradeRateModifier || integer|| || 0|| 
|-
| SpecialistProductionModifier || integer|| || 0|| 
|-
| SpecialistUpgradeModifier || integer|| || 0|| 
|-
| MilitaryProductionModifier || integer|| || 0|| 
|-
| BaseFreeUnits || integer|| || 0|| 
|-
| BaseFreeMilitaryUnits || integer|| || 0|| 
|-
| FreeUnitsPopulationPercent || integer|| || 0|| 
|-
| FreeMilitaryUnitsPopulationPercent || integer|| || 0|| 
|-
| HappinessPerGarrisonedUnit || integer|| || 0|| 
|-
| HappinessPerTradeRoute || integer|| || 0|| 
|-
| ExtraHappinessPerLuxury || integer|| || 0|| 
|-
| UnhappinessFromUnitsMod || integer|| || 0|| 
|-
| NumExtraBuilders || integer|| || 0|| 
|-
| PlotGoldCostMod || integer|| || 0|| 
|-
| PlotCultureCostModifier || integer|| || 0|| 
|-
| UnitPurchaseCostModifier || integer|| || 0|| 
|-
| TradeRouteGoldModifier || integer|| || 0|| 
|-
| GoldPerUnit || integer|| || 0|| 
|-
| GoldPerMilitaryUnit || integer|| || 0|| 
|-
| RouteGoldMaintenanceMod || integer|| || 0|| 
|-
| BuildingGoldMaintenanceMod || integer|| || 0|| 
|-
| UnitGoldMaintenanceMod || integer|| || 0|| 
|-
| UnitSupplyMod || integer|| || 0|| 
|-
| UnitUpgradeCostMod || integer|| || 0|| 
|-
| CityStrengthMod || integer|| || 0|| 
|-
| CityGrowthMod || integer|| || 0|| 
|-
| CapitalGrowthMod || integer|| || 0|| 
|-
| SettlerProductionModifier || integer|| || 0|| 
|-
| NewCityExtraPopulation || integer|| || 0|| 
|-
| FreeFoodBox || integer|| || 0|| 
|-
| HappyPerMilitaryUnit || integer|| || 0|| 
|-
| MilitaryFoodProduction || boolean|| || false|| 
|-
| HappinessToCulture || integer|| || 0|| 
|-
| HappinessToScience || integer|| || 0|| 
|-
| HalfSpecialistUnhappiness || boolean|| || false|| 
|-
| HalfSpecialistFood || boolean|| || false|| 
|-
| MaxConscript || integer|| || 0|| 
|-
| UnitSightRangeChange || integer|| || 0|| 
|-
| WoundedUnitDamageMod || integer|| || 0|| 
|-
| BarbarianCombatBonus || integer|| || 0|| 
|-
| AlwaysSeeBarbCamps || boolean|| || false|| 
|-
| RevealAllCapitals || boolean|| || false|| 
|-
| FreeSpecialist || integer|| || 0|| 
|-
| ExpModifier || integer|| || 0|| 
|-
| ExpInBorderModifier || integer|| || 0|| 
|-
| MinorQuestFriendshipMod || integer|| || 0|| 
|-
| MinorGoldFriendshipMod || integer|| || 0|| 
|-
| MinorFriendshipMinimum || integer|| || 0|| 
|-
| MinorFriendshipDecayMod || integer|| || 0|| 
|-
| OtherPlayersMinorFriendshipDecayMod || integer|| || 0|| 
|-
| MinorGreatPeopleAllies || boolean|| || false|| 
|-
| MinorScienceAllies || boolean|| || false|| 
|-
| MinorResourceBonus || boolean|| || false|| 
|-
| OneShot || boolean|| || false|| 
|-
| WeLoveTheKing || text|| || NULL|| 
|-
| TechPrereq || text|| Technologies(Type)|| NULL|| 
|-
| PortraitIndex || integer|| || 0|| 
|-
| IconAtlas || text|| IconTextureAtlases(Atlas)|| NULL|| 
|-
| IconAtlasAchieved || text|| IconTextureAtlases(Atlas)|| NULL|| 
|}
==Policy_CityYieldChanges==
*[[CIV5Yields]] contains the definitions of the Yields referenced in this table.
{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"
|+Policy_CityYieldChanges Table
! scope="col" style="background: #efefef;" | Name
! scope="col" style="background: #efefef;" | Type
! scope="col" style="background: #efefef;" | Reference
! scope="col" style="background: #efefef;" | Notes
|-
| PolicyType || text|| Policies(Type)|| 
|-
| YieldType || text|| Yields(Type)|| 
|-
| Yield || integer|| || Not Null
|}
==Policy_CoastalCityYieldChanges==
*[[CIV5Yields]] contains the definitions of the Yields referenced in this table.
{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"
|+Policy_CoastalCityYieldChanges Table
! scope="col" style="background: #efefef;" | Name
! scope="col" style="background: #efefef;" | Type
! scope="col" style="background: #efefef;" | Reference
! scope="col" style="background: #efefef;" | Notes
|-
| PolicyType || text|| Policies(Type)|| 
|-
| YieldType || text|| Yields(Type)|| 
|-
| Yield || integer|| || Not Null
|}
==Policy_CapitalYieldChanges==
*[[CIV5Yields]] contains the definitions of the Yields referenced in this table.
{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"
|+Policy_CapitalYieldChanges Table
! scope="col" style="background: #efefef;" | Name
! scope="col" style="background: #efefef;" | Type
! scope="col" style="background: #efefef;" | Reference
! scope="col" style="background: #efefef;" | Notes
|-
| PolicyType || text|| Policies(Type)|| 
|-
| YieldType || text|| Yields(Type)|| 
|-
| Yield || integer|| || Not Null
|}
==Policy_CapitalYieldModifiers==
*[[CIV5Yields]] contains the definitions of the Yields referenced in this table.
{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"
|+Policy_CapitalYieldModifiers Table
! scope="col" style="background: #efefef;" | Name
! scope="col" style="background: #efefef;" | Type
! scope="col" style="background: #efefef;" | Reference
! scope="col" style="background: #efefef;" | Notes
|-
| PolicyType || text|| Policies(Type)|| 
|-
| YieldType || text|| Yields(Type)|| 
|-
| Yield || integer|| || Not Null
|}
==Policy_Disables==
{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"
|+Policy_Disables Table
! scope="col" style="background: #efefef;" | Name
! scope="col" style="background: #efefef;" | Type
! scope="col" style="background: #efefef;" | Reference
|-
| PolicyType || text|| Policies(Type)
|-
| PolicyDisable || text|| Policies(Type)
|}
==Policy_Flavors==
*[[CIV5Flavors]] contains the definitions of the Flavors referenced in this table.
{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"
|+Policy_Flavors Table
! scope="col" style="background: #efefef;" | Name
! scope="col" style="background: #efefef;" | Type
! scope="col" style="background: #efefef;" | Reference
! scope="col" style="background: #efefef;" | Notes
|-
| PolicyType || text|| Policies(Type)|| 
|-
| FlavorType || text|| Flavors(Type)|| 
|-
| Flavor || integer|| || Not Null
|}
==Policy_HurryModifiers==
*[[CIV5HurryInfos]] contains the definitions of the HurryInfos referenced in this table.
{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"
|+Policy_HurryModifiers Table
! scope="col" style="background: #efefef;" | Name
! scope="col" style="background: #efefef;" | Type
! scope="col" style="background: #efefef;" | Reference
|-
| PolicyType || text|| Policies(Type)
|-
| HurryType || text|| HurryInfos(Type)
|-
| HurryCostModifier || integer|| 
|}
==Policy_PrereqPolicies==
{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"
|+Policy_PrereqPolicies Table
! scope="col" style="background: #efefef;" | Name
! scope="col" style="background: #efefef;" | Type
! scope="col" style="background: #efefef;" | Reference
|-
| PolicyType || text|| Policies(Type)
|-
| PrereqPolicy || text|| Policies(Type)
|}
==Policy_PrereqORPolicies==
{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"
|+Policy_PrereqORPolicies Table
! scope="col" style="background: #efefef;" | Name
! scope="col" style="background: #efefef;" | Type
! scope="col" style="background: #efefef;" | Reference
|-
| PolicyType || text|| Policies(Type)
|-
| PrereqPolicy || text|| Policies(Type)
|}
==Policy_SpecialistExtraYields==
*[[CIV5Yields]] contains the definitions of the Yields referenced in this table.
{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"
|+Policy_SpecialistExtraYields Table
! scope="col" style="background: #efefef;" | Name
! scope="col" style="background: #efefef;" | Type
! scope="col" style="background: #efefef;" | Reference
! scope="col" style="background: #efefef;" | Notes
|-
| PolicyType || text|| Policies(Type)|| 
|-
| YieldType || text|| Yields(Type)|| 
|-
| Yield || integer|| || Not Null
|}
==Policy_BuildingClassYieldModifiers==
*[[CIV5BuildingClasses]] contains the definitions of the BuildingClasses referenced in this table.
*[[CIV5Yields]] contains the definitions of the Yields referenced in this table.
{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"
|+Policy_BuildingClassYieldModifiers Table
! scope="col" style="background: #efefef;" | Name
! scope="col" style="background: #efefef;" | Type
! scope="col" style="background: #efefef;" | Reference
|-
| PolicyType || text|| Policies(Type)
|-
| BuildingClassType || text|| BuildingClasses(Type)
|-
| YieldType || text|| Yields(Type)
|-
| YieldMod || integer|| 
|}
==Policy_BuildingClassCultureChanges==
*[[CIV5BuildingClasses]] contains the definitions of the BuildingClasses referenced in this table.
{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"
|+Policy_BuildingClassCultureChanges Table
! scope="col" style="background: #efefef;" | Name
! scope="col" style="background: #efefef;" | Type
! scope="col" style="background: #efefef;" | Reference
|-
| PolicyType || text|| Policies(Type)
|-
| BuildingClassType || text|| BuildingClasses(Type)
|-
| CultureChange || integer|| 
|}
==Policy_BuildingClassHappiness==
*[[CIV5BuildingClasses]] contains the definitions of the BuildingClasses referenced in this table.
{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"
|+Policy_BuildingClassHappiness Table
! scope="col" style="background: #efefef;" | Name
! scope="col" style="background: #efefef;" | Type
! scope="col" style="background: #efefef;" | Reference
|-
| PolicyType || text|| Policies(Type)
|-
| BuildingClassType || text|| BuildingClasses(Type)
|-
| Happiness || integer|| 
|}
==Policy_ImprovementYieldChanges==
*[[CIV5Improvements]] contains the definitions of the Improvements referenced in this table.
*[[CIV5Yields]] contains the definitions of the Yields referenced in this table.
{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"
|+Policy_ImprovementYieldChanges Table
! scope="col" style="background: #efefef;" | Name
! scope="col" style="background: #efefef;" | Type
! scope="col" style="background: #efefef;" | Reference
|-
| PolicyType || text|| Policies(Type)
|-
| ImprovementType || text|| Improvements(Type)
|-
| YieldType || text|| Yields(Type)
|-
| Yield || integer|| 
|}
==Policy_ValidSpecialists==
*[[CIV5Specialists]] contains the definitions of the Specialists referenced in this table.
{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"
|+Policy_ValidSpecialists Table
! scope="col" style="background: #efefef;" | Name
! scope="col" style="background: #efefef;" | Type
! scope="col" style="background: #efefef;" | Reference
|-
| PolicyType || text|| Policies(Type)
|-
| SpecialistType || text|| Specialists(Type)
|}
==Policy_YieldModifiers==
*[[CIV5Yields]] contains the definitions of the Yields referenced in this table.
{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"
|+Policy_YieldModifiers Table
! scope="col" style="background: #efefef;" | Name
! scope="col" style="background: #efefef;" | Type
! scope="col" style="background: #efefef;" | Reference
! scope="col" style="background: #efefef;" | Notes
|-
| PolicyType || text|| Policies(Type)|| 
|-
| YieldType || text|| Yields(Type)|| 
|-
| Yield || integer|| || Not Null
|}
==Policy_FreePromotions==
*[[CIV5UnitPromotions]] contains the definitions of the UnitPromotions referenced in this table.
{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"
|+Policy_FreePromotions Table
! scope="col" style="background: #efefef;" | Name
! scope="col" style="background: #efefef;" | Type
! scope="col" style="background: #efefef;" | Reference
|-
| PolicyType || text|| Policies(Type)
|-
| PromotionType || text|| UnitPromotions(Type)
|}
==Policy_UnitCombatFreeExperiences==
*[[CIV5UnitCombatInfos]] contains the definitions of the UnitCombatInfos referenced in this table.
{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"
|+Policy_UnitCombatFreeExperiences Table
! scope="col" style="background: #efefef;" | Name
! scope="col" style="background: #efefef;" | Type
! scope="col" style="background: #efefef;" | Reference
|-
| PolicyType || text|| Policies(Type)
|-
| UnitCombatType || text|| UnitCombatInfos(Type)
|-
| FreeExperience || integer|| 
|}
==Policy_FreePromotionUnitCombats==
*[[CIV5UnitCombatInfos]] contains the definitions of the UnitCombatInfos referenced in this table.
*[[CIV5UnitPromotions]] contains the definitions of the UnitPromotions referenced in this table.
{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"
|+Policy_FreePromotionUnitCombats Table
! scope="col" style="background: #efefef;" | Name
! scope="col" style="background: #efefef;" | Type
! scope="col" style="background: #efefef;" | Reference
|-
| PolicyType || text|| Policies(Type)
|-
| UnitCombatType || text|| UnitCombatInfos(Type)
|-
| PromotionType || text|| UnitPromotions(Type)
|}
==Policy_UnitCombatProductionModifiers==
*[[CIV5UnitCombatInfos]] contains the definitions of the UnitCombatInfos referenced in this table.
{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"
|+Policy_UnitCombatProductionModifiers Table
! scope="col" style="background: #efefef;" | Name
! scope="col" style="background: #efefef;" | Type
! scope="col" style="background: #efefef;" | Reference
|-
| PolicyType || text|| Policies(Type)
|-
| UnitCombatType || text|| UnitCombatInfos(Type)
|-
| ProductionModifier || integer|| 
|}
==Policy_FreeUnitClasses==
*[[CIV5UnitClasses]] contains the definitions of the UnitClasses referenced in this table.
{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"
|+Policy_FreeUnitClasses Table
! scope="col" style="background: #efefef;" | Name
! scope="col" style="background: #efefef;" | Type
! scope="col" style="background: #efefef;" | Reference
! scope="col" style="background: #efefef;" | Notes
|-
| PolicyType || text|| Policies(Type)|| 
|-
| UnitClassType || text|| UnitClasses(Type)|| 
|-
| Count || integer|| || Not Null
|}
{{Civ5_XML_Files}}