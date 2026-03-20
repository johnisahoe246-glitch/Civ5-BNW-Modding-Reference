=civ5terrains.xml=
*The civ5terrains.xml file contains definitions for the Terrains.
*The reference field in the tables below indicates the table and column the entry is linked to.
*This information is taken from the civ5terrains.xml file itself.
==Terrains==
*[[CIV5IconTextureAtlases]] contains the definitions of the IconTextureAtlases referenced in this table.
{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"
|+Terrains Table
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
| Water || boolean|| || false|| 
|-
| Impassable || boolean|| || false|| 
|-
| Found || boolean|| || false|| 
|-
| FoundCoast || boolean|| || false|| 
|-
| FoundFreshWater || boolean|| || false|| 
|-
| Movement || integer|| || 1|| 
|-
| SeeFrom || integer|| || 1|| 
|-
| SeeThrough || integer|| || 1|| 
|-
| BuildModifier || integer|| || 0|| 
|-
| Defense || integer|| || 0|| 
|-
| InfluenceCost || integer|| || 0|| 
|-
| Button || text|| || || 
|-
| WorldSoundscapeAudioScript || text|| || || 
|-
| GraphicalOnly || boolean|| || false|| 
|-
| PortraitIndex || integer|| || -1|| 
|-
| EffectTypeTag || text|| || || 
|-
| IconAtlas || text|| IconTextureAtlases(Atlas)|| NULL|| 
|}
==Terrain_Yields==
*[[CIV5Yields]] contains the definitions of the Yields referenced in this table.
{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"
|+Terrain_Yields Table
! scope="col" style="background: #efefef;" | Name
! scope="col" style="background: #efefef;" | Type
! scope="col" style="background: #efefef;" | Reference
! scope="col" style="background: #efefef;" | Default
|-
| TerrainType || text|| [[Terrains(Type)]]|| 
|-
| YieldType || text|| [[Yields(Type)]]|| 
|-
| Yield || integer|| || 0
|}

==Terrain_RiverYieldChanges==
*[[CIV5Yields]] contains the definitions of the Yields referenced in this table.
{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"
|+Terrain_RiverYieldChanges Table
! scope="col" style="background: #efefef;" | Name
! scope="col" style="background: #efefef;" | Type
! scope="col" style="background: #efefef;" | Reference
! scope="col" style="background: #efefef;" | Default
|-
| TerrainType || text|| [[Terrains(Type)]]|| 
|-
| YieldType || text|| [[Yields|Yields(Type)]]|| 
|-
| Yield || integer|| || 0
|}

==Terrain_HillsYieldChanges==
*[[CIV5Yields]] contains the definitions of the Yields referenced in this table.
{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"
|+Terrain_HillsYieldChanges Table
! scope="col" style="background: #efefef;" | Name
! scope="col" style="background: #efefef;" | Type
! scope="col" style="background: #efefef;" | Reference
! scope="col" style="background: #efefef;" | Default
|-
| TerrainType || text|| Terrains(Type)|| 
|-
| YieldType || text|| Yields(Type)|| 
|-
| Yield || integer|| || 0
|}
{{Civ5_XML_Files}}