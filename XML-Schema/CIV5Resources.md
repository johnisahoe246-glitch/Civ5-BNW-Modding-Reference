=civ5resources.xml=
*The civ5resources.xml file contains definitions for the Resources.
*The reference field in the tables below indicates the table and column the entry is linked to.
*This information is taken from the civ5resources.xml file itself.
==Resources==
*[[CIV5IconTextureAtlases]] contains the definitions of the IconTextureAtlases referenced in this table.
{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"
|+Resources Table
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
| Help || text|| || || 
|-
| ResourceClassType || text|| || || 
|-
| ArtDefineTag || text|| || || 
|-
| AltArtDefineTag || text|| || || Art for marsh and water tiles
|-
| ArtDefineTagHeavy || text|| || || Art that is used when there is a large quantity of resources
|-
| AltArtDefineTagHeavy || text|| || || 
|-
| TechReveal || text|| || NULL|| 
|-
| TechCityTrade || text|| || NULL|| 
|-
| TechObsolete || text|| || NULL|| 
|-
| AIStopTradingEra || text|| || NULL|| 
|-
| Happiness || integer|| || 0|| 
|-
| WonderProductionMod || integer|| || 0|| 
|-
| StartingResourceQuantity || integer|| || 0|| 
|-
| AITradeModifier || integer|| || 0|| 
|-
| AIObjective || integer|| || 0|| 
|-
| PlacementOrder || integer|| || 0|| 
|-
| ConstAppearance || integer|| || 0|| 
|-
| MinAreaSize || integer|| || 0|| 
|-
| MinLatitude || integer|| || 0|| 
|-
| MaxLatitude || integer|| || 0|| 
|-
| RandApp1 || integer|| || 0|| 
|-
| RandApp2 || integer|| || 0|| 
|-
| RandApp3 || integer|| || 0|| 
|-
| RandApp4 || integer|| || 0|| 
|-
| Player || integer|| || 0|| 
|-
| TilesPer || integer|| || 0|| 
|-
| MinLandPercent || integer|| || 0|| 
|-
| Unique || integer|| || 0|| 
|-
| GroupRange || integer|| || 0|| 
|-
| GroupRand || integer|| || 0|| 
|-
| ResourceUsage || integer|| || 0|| 
|-
| PresentOnAllValidPlots || boolean|| || false|| 
|-
| Area || boolean|| || false|| 
|-
| Hills || boolean|| || false|| 
|-
| Flatlands || boolean|| || false|| 
|-
| NoRiverSide || boolean|| || false|| 
|-
| Normalize || boolean|| || false|| 
|-
| IconString || text|| || || 
|-
| PortraitIndex || integer|| || -1|| 
|-
| IconAtlas || text|| IconTextureAtlases(Atlas)|| NULL|| 
|}

==Resource_YieldChanges==
*[[CIV5Yields]] contains the definitions of the Yields referenced in this table.
{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"
|+Resource_YieldChanges Table
! scope="col" style="background: #efefef;" | Name
! scope="col" style="background: #efefef;" | Type
! scope="col" style="background: #efefef;" | Reference
! scope="col" style="background: #efefef;" | Default
|-
| ResourceType || text|| Resources(Type)|| 
|-
| YieldType || text|| Yields(Type)|| 
|-
| Yield || integer|| || 0
|}
==Resource_Flavors==
*[[CIV5Flavors]] contains the definitions of the Flavors referenced in this table.
{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"
|+Resource_Flavors Table
! scope="col" style="background: #efefef;" | Name
! scope="col" style="background: #efefef;" | Type
! scope="col" style="background: #efefef;" | Reference
! scope="col" style="background: #efefef;" | Default
|-
| ResourceType || text|| Resources(Type)|| 
|-
| FlavorType || text|| Flavors(Type)|| 
|-
| Flavor || integer|| || 0
|}
==Resource_TerrainBooleans==
*[[CIV5Terrains]] contains the definitions of the Terrains referenced in this table.
{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"
|+Resource_TerrainBooleans Table
! scope="col" style="background: #efefef;" | Name
! scope="col" style="background: #efefef;" | Type
! scope="col" style="background: #efefef;" | Reference
|-
| ResourceType || text|| Resources(Type)
|-
| TerrainType || text|| Terrains(Type)
|}
==Resource_FeatureBooleans==
*[[CIV5Features]] contains the definitions of the Features referenced in this table.
{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"
|+Resource_FeatureBooleans Table
! scope="col" style="background: #efefef;" | Name
! scope="col" style="background: #efefef;" | Type
! scope="col" style="background: #efefef;" | Reference
|-
| ResourceType || text|| Resources(Type)
|-
| FeatureType || text|| Features(Type)
|}
==Resource_FeatureTerrainBooleans==
*[[CIV5Terrains]] contains the definitions of the Terrains referenced in this table.
{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"
|+Resource_FeatureTerrainBooleans Table
! scope="col" style="background: #efefef;" | Name
! scope="col" style="background: #efefef;" | Type
! scope="col" style="background: #efefef;" | Reference
|-
| ResourceType || text|| Resources(Type)
|-
| TerrainType || text|| Terrains(Type)
|}
==Resource_QuantityTypes==
{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"
|+Resource_QuantityTypes Table
! scope="col" style="background: #efefef;" | Name
! scope="col" style="background: #efefef;" | Type
! scope="col" style="background: #efefef;" | Reference
! scope="col" style="background: #efefef;" | Notes
|-
| ResourceType || text|| Resources(Type)|| 
|-
| Quantity || integer|| || Not Null
|}
{{Civ5_XML_Files}}