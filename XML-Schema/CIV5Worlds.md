=civ5worlds.xml=
*The civ5worlds.xml file contains definitions for the Worlds.
*The reference field in the tables below indicates the table and column the entry is linked to.
*This information is taken from the civ5worlds.xml file itself.
==Worlds==
*[[CIV5IconTextureAtlases]] contains the definitions of the IconTextureAtlases referenced in this table.
{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"
|+Worlds Table
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
| DefaultPlayers || integer|| || || 
|-
| DefaultMinorCivs || integer|| || || 
|-
| FogTilesPerBarbarianCamp || integer|| || || 
|-
| NumNaturalWonders || integer|| || || 
|-
| UnitNameModifier || integer|| || || 
|-
| TargetNumCities || integer|| || || 
|-
| NumFreeBuildingResources || integer|| || || 
|-
| BuildingClassPrereqModifier || integer|| || || 
|-
| MaxConscriptModifier || integer|| || || 
|-
| GridWidth || integer|| || || 
|-
| GridHeight || integer|| || || 
|-
| TerrainGrainChange || integer|| || || 
|-
| FeatureGrainChange || integer|| || || 
|-
| ResearchPercent || integer|| || || 
|-
| NumCitiesUnhappinessPercent || integer|| || || 
|-
| NumCitiesPolicyCostMod || integer|| || || 
|-
| AdvancedStartPointsMod || integer|| || || 
|-
| PortraitIndex || integer|| || -1|| 
|-
| IconAtlas || text|| IconTextureAtlases(Atlas)|| NULL|| 
|}
{{Civ5_XML_Files}}