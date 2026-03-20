=CIV5Improvements.xml=
*The CIV5Improvements.xml file contains definitions for the Improvements.
*The reference field in the tables below indicates the table and column the entry is linked to.
*This information is taken from the CIV5Improvements.xml file itself.
==Improvements==
*[[CIV5IconTextureAtlases]] contains the definitions of the IconTextureAtlases referenced in this table.
{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"
|+Improvements Table
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
| Civilopedia || text|| || || 
|-
| ArtDefineTag || text|| || || 
|-
| WorldSoundscapeAudioScript || text|| || || 
|-
| ImprovementPillage || text|| Improvements(Type)|| NULL|| 
|-
| ImprovementUpgrade || text|| Improvements(Type)|| NULL|| 
|-
| HillsMakesValid || boolean|| || false|| 
|-
| FreshWaterMakesValid || boolean|| || false|| 
|-
| RiverSideMakesValid || boolean|| || false|| 
|-
| NoFreshWater || boolean|| || false|| 
|-
| RequiresFlatlands || boolean|| || false|| 
|-
| RequiresFlatlandsOrFreshWater || boolean|| || false|| 
|-
| RequiresFeature || boolean|| || false|| 
|-
| Water || boolean|| || false|| 
|-
| DestroyedWhenPillaged || boolean|| || false|| 
|-
| BuildableOnResources || boolean|| || false|| 
|-
| BarbarianCamp || boolean|| || false|| 
|-
| Goody || boolean|| || false|| 
|-
| Permanent || boolean|| || false|| 
|-
| OutsideBorders || boolean|| || false|| 
|-
| GraphicalOnly || boolean|| || false|| 
|-
| CreatedByGreatPerson || boolean|| || false|| 
|-
| Culture || integer|| || 0|| 
|-
| TilesPerGoody || integer|| || 0|| 
|-
| GoodyRange || integer|| || 0|| 
|-
| FeatureGrowth || integer|| || 0|| 
|-
| UpgradeTime || integer|| || 0|| 
|-
| RiverSideUpgradeMod || integer|| || 0|| 
|-
| CoastalLandUpgradeMod || integer|| || 0|| 
|-
| HillsUpgradeMod || integer|| || 0|| 
|-
| FreshWaterUpgradeMod || integer|| || 0|| 
|-
| DefenseModifier || integer|| || 0|| 
|-
| NearbyEnemyDamage || integer|| || 0|| 
|-
| PillageGold || integer|| || 0|| 
|-
| ResourceExtractionMod || integer|| || 0|| 
|-
| GoldMaintenance || integer|| || 0|| 
|-
| PortraitIndex || integer|| || -1|| 
|-
| IconAtlas || text|| IconTextureAtlases(Atlas)|| NULL|| 
|}
==Improvement_Flavors==
*[[CIV5Flavors]] contains the definitions of the Flavors referenced in this table.
{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"
|+Improvement_Flavors Table
! scope="col" style="background: #efefef;" | Name
! scope="col" style="background: #efefef;" | Type
! scope="col" style="background: #efefef;" | Reference
! scope="col" style="background: #efefef;" | Notes
|-
| ImprovementType || text|| Improvements(Type)|| 
|-
| FlavorType || text|| Flavors(Type)|| 
|-
| Flavor || integer|| || Not Null
|}
==Improvement_Yields==
*[[CIV5Yields]] contains the definitions of the Yields referenced in this table.
{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"
|+Improvement_Yields Table
! scope="col" style="background: #efefef;" | Name
! scope="col" style="background: #efefef;" | Type
! scope="col" style="background: #efefef;" | Reference
! scope="col" style="background: #efefef;" | Default
|-
| ImprovementType || text|| Improvements(Type)|| 
|-
| YieldType || text|| Yields(Type)|| 
|-
| Yield || integer|| || 0
|}
==Improvement_AdjacentCityYields==
*[[CIV5Yields]] contains the definitions of the Yields referenced in this table.
{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"
|+Improvement_AdjacentCityYields Table
! scope="col" style="background: #efefef;" | Name
! scope="col" style="background: #efefef;" | Type
! scope="col" style="background: #efefef;" | Reference
! scope="col" style="background: #efefef;" | Default
|-
| ImprovementType || text|| Improvements(Type)|| 
|-
| YieldType || text|| Yields(Type)|| 
|-
| Yield || integer|| || 0
|}
==Improvement_CoastalLandYields==
*[[CIV5Yields]] contains the definitions of the Yields referenced in this table.
{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"
|+Improvement_CoastalLandYields Table
! scope="col" style="background: #efefef;" | Name
! scope="col" style="background: #efefef;" | Type
! scope="col" style="background: #efefef;" | Reference
! scope="col" style="background: #efefef;" | Default
|-
| ImprovementType || text|| Improvements(Type)|| 
|-
| YieldType || text|| Yields(Type)|| 
|-
| Yield || integer|| || 0
|}
==Improvement_FreshWaterYields==
*[[CIV5Yields]] contains the definitions of the Yields referenced in this table.
{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"
|+Improvement_FreshWaterYields Table
! scope="col" style="background: #efefef;" | Name
! scope="col" style="background: #efefef;" | Type
! scope="col" style="background: #efefef;" | Reference
! scope="col" style="background: #efefef;" | Default
|-
| ImprovementType || text|| Improvements(Type)|| 
|-
| YieldType || text|| Yields(Type)|| 
|-
| Yield || integer|| || 0
|}
==Improvement_HillsYields==
*[[CIV5Yields]] contains the definitions of the Yields referenced in this table.
{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"
|+Improvement_HillsYields Table
! scope="col" style="background: #efefef;" | Name
! scope="col" style="background: #efefef;" | Type
! scope="col" style="background: #efefef;" | Reference
! scope="col" style="background: #efefef;" | Default
|-
| ImprovementType || text|| Improvements(Type)|| 
|-
| YieldType || text|| Yields(Type)|| 
|-
| Yield || integer|| || 0
|}
==Improvement_PrereqNatureYields==
*[[CIV5Yields]] contains the definitions of the Yields referenced in this table.
{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"
|+Improvement_PrereqNatureYields Table
! scope="col" style="background: #efefef;" | Name
! scope="col" style="background: #efefef;" | Type
! scope="col" style="background: #efefef;" | Reference
! scope="col" style="background: #efefef;" | Default
|-
| ImprovementType || text|| Improvements(Type)|| 
|-
| YieldType || text|| Yields(Type)|| 
|-
| Yield || integer|| || 0
|}
==Improvement_RiverSideYields==
*[[CIV5Yields]] contains the definitions of the Yields referenced in this table.
{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"
|+Improvement_RiverSideYields Table
! scope="col" style="background: #efefef;" | Name
! scope="col" style="background: #efefef;" | Type
! scope="col" style="background: #efefef;" | Reference
! scope="col" style="background: #efefef;" | Default
|-
| ImprovementType || text|| Improvements(Type)|| 
|-
| YieldType || text|| Yields(Type)|| 
|-
| Yield || integer|| || 0
|}
==Improvement_ValidTerrains==
*[[CIV5Terrains]] contains the definitions of the Terrains referenced in this table.
{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"
|+Improvement_ValidTerrains Table
! scope="col" style="background: #efefef;" | Name
! scope="col" style="background: #efefef;" | Type
! scope="col" style="background: #efefef;" | Reference
|-
| ImprovementType || text|| Improvements(Type)
|-
| TerrainType || text|| Terrains(Type)
|}
==Improvement_ValidFeatures==
*[[CIV5Features]] contains the definitions of the Features referenced in this table.
{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"
|+Improvement_ValidFeatures Table
! scope="col" style="background: #efefef;" | Name
! scope="col" style="background: #efefef;" | Type
! scope="col" style="background: #efefef;" | Reference
|-
| ImprovementType || text|| Improvements(Type)
|-
| FeatureType || text|| Features(Type)
|}
==Improvement_ResourceTypes==
*[[CIV5Resources]] contains the definitions of the Resources referenced in this table.
{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"
|+Improvement_ResourceTypes Table
! scope="col" style="background: #efefef;" | Name
! scope="col" style="background: #efefef;" | Type
! scope="col" style="background: #efefef;" | Reference
! scope="col" style="background: #efefef;" | Default
|-
| ImprovementType || text|| Improvements(Type)|| 
|-
| ResourceType || text|| Resources(Type)|| 
|-
| ResourceMakesValid || boolean|| || true
|-
| ResourceTrade || boolean|| || true
|-
| DiscoveryRand || integer|| || 0
|-
| QuantityRequirement || integer|| || 0
|}
==Improvement_ResourceType_Yields==
*[[CIV5Resources]] contains the definitions of the Resources referenced in this table.
*[[CIV5Yields]] contains the definitions of the Yields referenced in this table.
{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"
|+Improvement_ResourceType_Yields Table
! scope="col" style="background: #efefef;" | Name
! scope="col" style="background: #efefef;" | Type
! scope="col" style="background: #efefef;" | Reference
! scope="col" style="background: #efefef;" | Default
|-
| ImprovementType || text|| Improvements(Type)|| 
|-
| ResourceType || text|| Resources(Type)|| 
|-
| YieldType || text|| Yields(Type)|| 
|-
| Yield || integer|| || 0
|}
==Improvement_RouteYieldChanges==
*[[CIV5Routes]] contains the definitions of the Routes referenced in this table.
*[[CIV5Yields]] contains the definitions of the Yields referenced in this table.
{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"
|+Improvement_RouteYieldChanges Table
! scope="col" style="background: #efefef;" | Name
! scope="col" style="background: #efefef;" | Type
! scope="col" style="background: #efefef;" | Reference
|-
| ImprovementType || text|| Improvements(Type)
|-
| RouteType || text|| Routes(Type)
|-
| YieldType || text|| Yields(Type)
|-
| Yield || integer|| 
|}
==Improvement_TechYieldChanges==
*[[CIV5Technologies]] contains the definitions of the Technologies referenced in this table.
*[[CIV5Yields]] contains the definitions of the Yields referenced in this table.
{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"
|+Improvement_TechYieldChanges Table
! scope="col" style="background: #efefef;" | Name
! scope="col" style="background: #efefef;" | Type
! scope="col" style="background: #efefef;" | Reference
|-
| ImprovementType || text|| Improvements(Type)
|-
| TechType || text|| Technologies(Type)
|-
| YieldType || text|| Yields(Type)
|-
| Yield || integer|| 
|}
==Improvement_TechNoFreshWaterYieldChanges==
*[[CIV5Technologies]] contains the definitions of the Technologies referenced in this table.
*[[CIV5Yields]] contains the definitions of the Yields referenced in this table.
{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"
|+Improvement_TechNoFreshWaterYieldChanges Table
! scope="col" style="background: #efefef;" | Name
! scope="col" style="background: #efefef;" | Type
! scope="col" style="background: #efefef;" | Reference
|-
| ImprovementType || text|| Improvements(Type)
|-
| TechType || text|| Technologies(Type)
|-
| YieldType || text|| Yields(Type)
|-
| Yield || integer|| 
|}
==Improvement_TechFreshWaterYieldChanges==
*[[CIV5Technologies]] contains the definitions of the Technologies referenced in this table.
*[[CIV5Yields]] contains the definitions of the Yields referenced in this table.
{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"
|+Improvement_TechFreshWaterYieldChanges Table
! scope="col" style="background: #efefef;" | Name
! scope="col" style="background: #efefef;" | Type
! scope="col" style="background: #efefef;" | Reference
|-
| ImprovementType || text|| Improvements(Type)
|-
| TechType || text|| Technologies(Type)
|-
| YieldType || text|| Yields(Type)
|-
| Yield || integer|| 
|}
{{Civ5_XML_Files}}