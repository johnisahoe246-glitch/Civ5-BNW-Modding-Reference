=civ5features.xml=
*The civ5features.xml file contains definitions for the Features.
*The reference field in the tables below indicates the table and column the entry is linked to.
*This information is taken from the civ5features.xml file itself.
==Features==
*[[CIV5Terrains]] contains the definitions of the Terrains referenced in this table.
*[[CIV5IconTextureAtlases]] contains the definitions of the IconTextureAtlases referenced in this table.
{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"
|+Features Table
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
| StartingLocationWeight || integer|| || 0|| 
|-
| Movement || integer|| || 0|| 
|-
| SeeThrough || integer|| || 0|| 
|-
| Defense || integer|| || 0|| 
|-
| InfluenceCost || integer|| || 0|| 
|-
| AppearanceProbability || integer|| || 0|| 
|-
| DisappearanceProbability || integer|| || 0|| 
|-
| Growth || integer|| || 0|| 
|-
| GrowthTerrainType || text|| Terrains(Type)|| || 
|-
| TurnDamage || integer|| || 0|| 
|-
| YieldNotAdditive || boolean|| || false|| 
|-
| NoCoast || boolean|| || false|| 
|-
| NoRiver || boolean|| || false|| 
|-
| NoAdjacent || boolean|| || false|| 
|-
| RequiresFlatlands || boolean|| || false|| 
|-
| RequiresRiver || boolean|| || false|| 
|-
| AddsFreshWater || boolean|| || false|| 
|-
| Impassable || boolean|| || false|| 
|-
| NoCity || boolean|| || false|| 
|-
| NoImprovement || boolean|| || false|| 
|-
| VisibleAlways || boolean|| || false|| 
|-
| NukeImmune || boolean|| || false|| 
|-
| NaturalWonder || boolean|| || false|| 
|-
| Rough || boolean|| || false|| 
|-
| WorldSoundscapeAudioScript || text|| || || 
|-
| EffectType || text|| || || 
|-
| EffectProbability || integer|| || 0|| 
|-
| EffectTypeTag || text|| || || 
|-
| AdvancedStartRemoveCost || integer|| || 0|| 
|-
| PortraitIndex || integer|| || -1|| 
|-
| IconAtlas || text|| IconTextureAtlases(Atlas)|| NULL|| 
|}
==FakeFeatures==
*[[CIV5Terrains]] contains the definitions of the Terrains referenced in this table.
*[[CIV5IconTextureAtlases]] contains the definitions of the IconTextureAtlases referenced in this table.
{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"
|+FakeFeatures Table
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
| StartingLocationWeight || integer|| || 0|| 
|-
| Movement || integer|| || 0|| 
|-
| SeeThrough || integer|| || 0|| 
|-
| Defense || integer|| || 0|| 
|-
| InfluenceCost || integer|| || 0|| 
|-
| AppearanceProbability || integer|| || 0|| 
|-
| DisappearanceProbability || integer|| || 0|| 
|-
| Growth || integer|| || 0|| 
|-
| GrowthTerrainType || text|| Terrains(Type)|| || 
|-
| TurnDamage || integer|| || 0|| 
|-
| YieldNotAdditive || boolean|| || false|| 
|-
| NoCoast || boolean|| || false|| 
|-
| NoRiver || boolean|| || false|| 
|-
| NoAdjacent || boolean|| || false|| 
|-
| RequiresFlatlands || boolean|| || false|| 
|-
| RequiresRiver || boolean|| || false|| 
|-
| AddsFreshWater || boolean|| || false|| 
|-
| Impassable || boolean|| || false|| 
|-
| NoCity || boolean|| || false|| 
|-
| NoImprovement || boolean|| || false|| 
|-
| VisibleAlways || boolean|| || false|| 
|-
| NukeImmune || boolean|| || false|| 
|-
| NaturalWonder || boolean|| || false|| 
|-
| Rough || boolean|| || false|| 
|-
| WorldSoundscapeAudioScript || text|| || || 
|-
| EffectType || text|| || || 
|-
| EffectProbability || integer|| || 0|| 
|-
| EffectTypeTag || text|| || || 
|-
| AdvancedStartRemoveCost || integer|| || 0|| 
|-
| PortraitIndex || integer|| || -1|| 
|-
| IconAtlas || text|| IconTextureAtlases(Atlas)|| NULL|| 
|}
==Feature_YieldChanges==
*[[CIV5Yields]] contains the definitions of the Yields referenced in this table.
{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"
|+Feature_YieldChanges Table
! scope="col" style="background: #efefef;" | Name
! scope="col" style="background: #efefef;" | Type
! scope="col" style="background: #efefef;" | Reference
|-
| FeatureType || text|| Features(Type)
|-
| YieldType || text|| Yields(Type)
|-
| Yield || integer|| 
|}
==Feature_RiverYieldChanges==
*[[CIV5Yields]] contains the definitions of the Yields referenced in this table.
{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"
|+Feature_RiverYieldChanges Table
! scope="col" style="background: #efefef;" | Name
! scope="col" style="background: #efefef;" | Type
! scope="col" style="background: #efefef;" | Reference
|-
| FeatureType || text|| Features(Type)
|-
| YieldType || text|| Yields(Type)
|-
| Yield || integer|| 
|}
==Feature_HillsYieldChanges==
*[[CIV5Yields]] contains the definitions of the Yields referenced in this table.
{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"
|+Feature_HillsYieldChanges Table
! scope="col" style="background: #efefef;" | Name
! scope="col" style="background: #efefef;" | Type
! scope="col" style="background: #efefef;" | Reference
|-
| FeatureType || text|| Features(Type)
|-
| YieldType || text|| Yields(Type)
|-
| Yield || integer|| 
|}
==Feature_TerrainBooleans==
*[[CIV5Terrains]] contains the definitions of the Terrains referenced in this table.
{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"
|+Feature_TerrainBooleans Table
! scope="col" style="background: #efefef;" | Name
! scope="col" style="background: #efefef;" | Type
! scope="col" style="background: #efefef;" | Reference
|-
| FeatureType || text|| Features(Type)
|-
| TerrainType || text|| Terrains(Type)
|}
{{Civ5_XML_Files}}