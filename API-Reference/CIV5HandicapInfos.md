=civ5handicapinfos.xml=
*The civ5handicapinfos.xml file contains definitions for the HandicapInfos.
*The reference field in the tables below indicates the table and column the entry is linked to.
*This information is taken from the civ5handicapinfos.xml file itself.
==HandicapInfos==
*[[CIV5IconTextureAtlases]] contains the definitions of the IconTextureAtlases referenced in this table.
{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"
|+HandicapInfos Table
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
| Description || text|| || || 
|-
| Help || text|| || || 
|-
| StartingLocPercent || integer|| || 0|| 
|-
| AdvancedStartPointsMod || integer|| || 0|| 
|-
| StartingPolicyPoints || integer|| || 0|| 
|-
| HappinessDefault || integer|| || 0|| 
|-
| ExtraHappinessPerLuxury || integer|| || 0|| 
|-
| NumCitiesUnhappinessMod || integer|| || 0|| 
|-
| PopulationUnhappinessMod || integer|| || 0|| 
|-
| Gold || integer|| || 0|| 
|-
| GoldFreeUnits || integer|| || 0|| 
|-
| ProductionFreeUnits || integer|| || 0|| 
|-
| ProductionFreeUnitsPerCity || integer|| || 0|| 
|-
| ProductionFreeUnitsPopulationPercent || integer|| || 0|| 
|-
| RouteCostPercent || integer|| || 0|| 
|-
| UnitCostPercent || integer|| || 0|| 
|-
| BuildingCostPercent || integer|| || 0|| 
|-
| ResearchPercent || integer|| || 0|| 
|-
| PolicyPercent || integer|| || 0|| 
|-
| ImprovementCostPercent || integer|| || 0|| 
|-
| CityProductionNumOptionsConsidered || integer|| || 0|| 
|-
| TechNumOptionsConsidered || integer|| || 0|| 
|-
| PolicyNumOptionsConsidered || integer|| || 0|| 
|-
| InflationPercent || integer|| || 0|| 
|-
| FreeCulturePerTurn || integer|| || 0|| 
|-
| AttitudeChange || integer|| || 0|| 
|-
| NoTechTradeModifier || integer|| || 0|| 
|-
| TechTradeKnownModifier || integer|| || 0|| 
|-
| BarbCampGold || integer|| || 0|| 
|-
| BarbSpawnMod || integer|| || 0|| 
|-
| BarbarianBonus || integer|| || 0|| 
|-
| AIBarbarianBonus || integer|| || 0|| 
|-
| EarliestBarbarianReleaseTurn || integer|| || 0|| 
|-
| BarbarianLandTargetRange || integer|| || 0|| 
|-
| BarbarianSeaTargetRange || integer|| || 0|| 
|-
| StartingDefenseUnits || integer|| || 0|| 
|-
| StartingWorkerUnits || integer|| || 0|| 
|-
| StartingExploreUnits || integer|| || 0|| 
|-
| AIStartingUnitMultiplier || integer|| || 0|| 
|-
| AIStartingDefenseUnits || integer|| || 0|| 
|-
| AIStartingWorkerUnits || integer|| || 0|| 
|-
| AIStartingExploreUnits || integer|| || 0|| 
|-
| AIDeclareWarProb || integer|| || 0|| 
|-
| AIWorkRateModifier || integer|| || 0|| 
|-
| AIUnhappinessPercent || integer|| || 0|| 
|-
| AIGrowthPercent || integer|| || 0|| 
|-
| AITrainPercent || integer|| || 0|| 
|-
| AIWorldTrainPercent || integer|| || 0|| 
|-
| AIConstructPercent || integer|| || 0|| 
|-
| AIWorldConstructPercent || integer|| || 0|| 
|-
| AICreatePercent || integer|| || 0|| 
|-
| AIWorldCreatePercent || integer|| || 0|| 
|-
| AIBuildingCostPercent || integer|| || 0|| 
|-
| AIUnitCostPercent || integer|| || 0|| 
|-
| AIUnitSupplyPercent || integer|| || 0|| 
|-
| AIUnitUpgradePercent || integer|| || 0|| 
|-
| AIInflationPercent || integer|| || 0|| 
|-
| AIPerEraModifier || integer|| || 0|| 
|-
| AIAdvancedStartPercent || integer|| || 0|| 
|-
| PortraitIndex || integer|| || -1|| 
|-
| IconAtlas || text|| IconTextureAtlases(Atlas)|| NULL|| 
|}
==HandicapInfo_Goodies==
*[[CIV5GoodyHuts]] contains the definitions of the GoodyHuts referenced in this table.
{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"
|+HandicapInfo_Goodies Table
! scope="col" style="background: #efefef;" | Name
! scope="col" style="background: #efefef;" | Type
! scope="col" style="background: #efefef;" | Reference
|-
| HandicapType || text|| HandicapInfos(Type)
|-
| GoodyType || text|| GoodyHuts(Type)
|}
==HandicapInfo_FreeTechs==
*[[CIV5Technologies]] contains the definitions of the Technologies referenced in this table.
{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"
|+HandicapInfo_FreeTechs Table
! scope="col" style="background: #efefef;" | Name
! scope="col" style="background: #efefef;" | Type
! scope="col" style="background: #efefef;" | Reference
|-
| HandicapType || text|| HandicapInfos(Type)
|-
| TechType || text|| Technologies(Type)
|}
==HandicapInfo_AIFreeTechs==
*[[CIV5Technologies]] contains the definitions of the Technologies referenced in this table.
{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"
|+HandicapInfo_AIFreeTechs Table
! scope="col" style="background: #efefef;" | Name
! scope="col" style="background: #efefef;" | Type
! scope="col" style="background: #efefef;" | Reference
|-
| HandicapType || text|| HandicapInfos(Type)
|-
| TechType || text|| Technologies(Type)
|}
{{Civ5_XML_Files}}