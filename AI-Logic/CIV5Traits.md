=CIV5Traits.xml=
*The CIV5Traits.xml file contains definitions for the Traits.
*The reference field in the tables below indicates the table and column the entry is linked to.
*This information is taken from the CIV5Traits.xml file itself.
==Traits==
*[[CIV5UnitClasses]] contains the definitions of the UnitClasses referenced in this table.
*[[CIV5Technologies]] contains the definitions of the Technologies referenced in this table.
{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"
|+Traits Table
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
| ShortDescription || text|| || || 
|-
| LevelExperienceModifier || integer|| || 0|| 
|-
| GreatPeopleRateModifier || integer|| || 0|| 
|-
| GreatScientistRateModifier || integer|| || 0|| 
|-
| GreatGeneralRateModifier || integer|| || 0|| 
|-
| GreatGeneralExtraBonus || integer|| || 0|| 
|-
| MaxGlobalBuildingProductionModifier || integer|| || 0|| 
|-
| MaxTeamBuildingProductionModifier || integer|| || 0|| 
|-
| MaxPlayerBuildingProductionModifier || integer|| || 0|| 
|-
| CityUnhappinessModifier || integer|| || 0|| 
|-
| PopulationUnhappinessModifier || integer|| || 0|| 
|-
| CityStateBonusModifier || integer|| || 0|| 
|-
| CityStateFriendshipModifier || integer|| || 0|| 
|-
| CityStateCombatModifier || integer|| || 0|| 
|-
| LandBarbarianConversionPercent || integer|| || 0|| 
|-
| SeaBarbarianConversionPercent || integer|| || 0|| 
|-
| CapitalBuildingModifier || integer|| || 0|| 
|-
| PlotBuyCostModifier || integer|| || 0|| 
|-
| PlotCultureCostModifier || integer|| || 0|| 
|-
| CultureFromKills || integer|| || 0|| 
|-
| CityCultureBonus || integer|| || 0|| 
|-
| PolicyCostModifier || integer|| || 0|| 
|-
| TradeRouteChange || integer|| || 0|| 
|-
| WonderProductionModifier || integer|| || 0|| 
|-
| PlunderModifier || integer|| || 0|| 
|-
| GoldenAgeDurationModifier || integer|| || 0|| 
|-
| GoldenAgeMoveChange || integer|| || 0|| 
|-
| GoldenAgeCombatModifier || integer|| || 0|| 
|-
| ExtraEmbarkMoves || integer|| || 0|| 
|-
| FightWellDamaged || boolean|| || false|| 
|-
| MoveFriendlyWoodsAsRoad || boolean|| || false|| 
|-
| FasterAlongRiver || boolean|| || false|| 
|-
| EmbarkedNotCivilian || boolean|| || false|| 
|-
| FreeUnit || text|| UnitClasses(Type)|| NULL|| 
|-
| FreeUnitPrereqTech || text|| Technologies(Type)|| NULL|| 
|-
| ObsoleteTech || text|| Technologies(Type)|| NULL|| 
|}
==Trait_ExtraYieldThresholds==
*[[CIV5Yields]] contains the definitions of the Yields referenced in this table.
{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"
|+Trait_ExtraYieldThresholds Table
! scope="col" style="background: #efefef;" | Name
! scope="col" style="background: #efefef;" | Type
! scope="col" style="background: #efefef;" | Reference
|-
| TraitType || text|| Traits(Type)
|-
| YieldType || text|| Yields(Type)
|-
| Yield || integer|| 
|}
==Trait_YieldChanges==
*[[CIV5Yields]] contains the definitions of the Yields referenced in this table.
{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"
|+Trait_YieldChanges Table
! scope="col" style="background: #efefef;" | Name
! scope="col" style="background: #efefef;" | Type
! scope="col" style="background: #efefef;" | Reference
|-
| TraitType || text|| Traits(Type)
|-
| YieldType || text|| Yields(Type)
|-
| Yield || integer|| 
|}
==Trait_YieldChangesStrategicResources==
*[[CIV5Yields]] contains the definitions of the Yields referenced in this table.
{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"
|+Trait_YieldChangesStrategicResources Table
! scope="col" style="background: #efefef;" | Name
! scope="col" style="background: #efefef;" | Type
! scope="col" style="background: #efefef;" | Reference
|-
| TraitType || text|| Traits(Type)
|-
| YieldType || text|| Yields(Type)
|-
| Yield || integer|| 
|}
==Trait_YieldModifiers==
*[[CIV5Yields]] contains the definitions of the Yields referenced in this table.
{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"
|+Trait_YieldModifiers Table
! scope="col" style="background: #efefef;" | Name
! scope="col" style="background: #efefef;" | Type
! scope="col" style="background: #efefef;" | Reference
|-
| TraitType || text|| Traits(Type)
|-
| YieldType || text|| Yields(Type)
|-
| Yield || integer|| 
|}
==Trait_FreePromotions==
*[[CIV5UnitPromotions]] contains the definitions of the UnitPromotions referenced in this table.
{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"
|+Trait_FreePromotions Table
! scope="col" style="background: #efefef;" | Name
! scope="col" style="background: #efefef;" | Type
! scope="col" style="background: #efefef;" | Reference
|-
| TraitType || text|| Traits(Type)
|-
| PromotionType || text|| UnitPromotions(Type)
|}
==Trait_FreePromotionUnitCombats==
*[[CIV5UnitCombatInfos]] contains the definitions of the UnitCombatInfos referenced in this table.
*[[CIV5UnitPromotions]] contains the definitions of the UnitPromotions referenced in this table.
{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"
|+Trait_FreePromotionUnitCombats Table
! scope="col" style="background: #efefef;" | Name
! scope="col" style="background: #efefef;" | Type
! scope="col" style="background: #efefef;" | Reference
|-
| TraitType || text|| Traits(Type)
|-
| UnitCombatType || text|| UnitCombatInfos(Type)
|-
| PromotionType || text|| UnitPromotions(Type)
|}
==Trait_MovesChangeUnitCombats==
*[[CIV5UnitCombatInfos]] contains the definitions of the UnitCombatInfos referenced in this table.
{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"
|+Trait_MovesChangeUnitCombats Table
! scope="col" style="background: #efefef;" | Name
! scope="col" style="background: #efefef;" | Type
! scope="col" style="background: #efefef;" | Reference
|-
| TraitType || text|| Traits(Type)
|-
| UnitCombatType || text|| UnitCombatInfos(Type)
|-
| MovesChange || int|| 
|}
==Trait_Terrains==
{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"
|+Trait_Terrains Table
! scope="col" style="background: #efefef;" | Name
! scope="col" style="background: #efefef;" | Type
! scope="col" style="background: #efefef;" | Reference
! scope="col" style="background: #efefef;" | Default
|-
| TraitType || text|| Traits(Type)|| 
|-
| TerrainType || text|| || 
|-
| StrategicResourceQuantityModifier || integer|| || 0
|}
==Trait_ResourceQuantityModifiers==
*[[CIV5Resources]] contains the definitions of the Resources referenced in this table.
{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"
|+Trait_ResourceQuantityModifiers Table
! scope="col" style="background: #efefef;" | Name
! scope="col" style="background: #efefef;" | Type
! scope="col" style="background: #efefef;" | Reference
! scope="col" style="background: #efefef;" | Default
|-
| TraitType || text|| Traits(Type)|| 
|-
| ResourceType || text|| Resources(Type)|| 
|-
| ResourceQuantityModifier || integer|| || 0
|}
{{Civ5_XML_Files}}