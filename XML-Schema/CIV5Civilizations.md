=civ5civilizations.xml=
*The civ5civilizations.xml file contains definitions for the Civilizations.
*The reference field in the tables below indicates the table and column the entry is linked to.
*This information is taken from the Kael's Modder's Guide to Civilization 5.
==Civilizations==
*[[CIV5IconTextureAtlases]] contains the definitions of the IconTextureAtlases referenced in this table.
{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"
|+Civilizations Table
! scope="col" style="background: #efefef;" | Name
! scope="col" style="background: #efefef;" | Type
! scope="col" style="background: #efefef;" | Reference
! scope="col" style="background: #efefef;" | Default
! scope="col" style="background: #efefef;" | Notes
|-
| ID || integer|| || || Primary Key,Autoincrement
|-
| Type || text|| || || Not Null,Unique, key used to reference this civilization typically in the CIVILIZATION_<name> format
|-
| Description || text|| || || Text string description of the civ, for America it is "American Empire" located in the TXT_KEY_CIV_AMERICA_DESC
|-
| Civilopedia || text|| || NULL|| NOT USED
|-
| CivilopediaTag || text|| || || starting text string for the pedia entry
|-
| Strategy || text|| || Ask Paul|| NOT USED
|-
| Playable || boolean|| || true|| If true, human player can select this civ.
|-
| AIPlayable || boolean|| || true|| If true, the AI can select this civ. Setting both Playable and AIPlayable to false is a good way to remove a civ from a game, without actually deleting the assets (and makes other mods compatible)
|-
| ShortDescription || text|| || NULL|| The short text string for this civ.  For america its "America"
|-
| Adjective || text|| || NULL|| The text string for the qualifier to things that belong to this civ. For American, its "American"
|-
| DefaultPlayerColor || text|| || NULL|| The default color of this civ for borders, unit flags, etc.  The color has to be specified in the [[CIV5PlayerColors]]
|-
| ArtDefineTag || text|| || NULL|| NOT USED
|-
| ArtStyleType || text|| || NULL|| Defines the art style used for buildings that are used in this civilization's cities
|-
| ArtStyleSuffix || text|| || NULL|| Used to pick different flavors of improvements and wonder art
|-
| ArtStylePrefix || text|| || NULL|| Used to pick different flavors of improvements and wonder art
|-
| DerivativeCiv || text|| || NULL|| NOT USED
|-
| PortraitIndex || integer|| || -1|| The number of the icon in the icon atlas used for this civ
|-
| IconAtlas || text|| IconTextureAtlases(Atlas)|| NULL|| The Icon Atlas that holds the icons for this civ
|-
| AlphaIconAtlas || text|| IconTextureAtlases(Atlas)|| NULL|| The Icon Atlas that has the alpha layer for this icon
|-
| MapImage || text|| || NULL|| The picture (as a .dds file) that is displayed when the civ is selected from the civilization selection menu.  Typically this is a map of the civilization
|-
| DawnOfManQuote || text|| || NULL|| The text string that is displayed on the loading (Dawn of Man) screen
|-
| DawnOfManImage || text|| || NULL|| The picture (as a .dds file) that is shown on the loading (Dawn of Man) screen
|-
| DawnOfManAudio || text|| || NULL|| The audio file that is played the loading (Dawn of Man) screen. Typically this is the reading of the Quote
|}

==Civilization_BuildingClassOverrides==
*[[CIV5BuildingClasses]] contains the definitions of the BuildingClasses referenced in this table.
*[[CIV5Buildings]] contains the definitions of the Buildings referenced in this table.
{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"
|+Civilization_BuildingClassOverrides Table
! scope="col" style="background: #efefef;" | Name
! scope="col" style="background: #efefef;" | Type
! scope="col" style="background: #efefef;" | Reference
! scope="col" style="background: #efefef;" | Notes
|-
| CivilizationType || text|| Civilizations(Type)|| Name (Type) of civilization to have building defined
|-
| BuildingClassType || text|| BuildingClasses(Type)|| Not Null
|-
| BuildingType || text|| Buildings(Type)|| This defines a civ's Unique Buildings and can be used to block civs from building a specific building, for example a minor civ from building the Sydney Opera House, when tag is left empty: <BuildingType/>
|}

==Civilization_CityNames==
*This is a list of the available city names for a civilization.
{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"
|+Civilization_CityNames Table
! scope="col" style="background: #efefef;" | Name
! scope="col" style="background: #efefef;" | Type
! scope="col" style="background: #efefef;" | Reference
! scope="col" style="background: #efefef;" | Notes
|-
| CivilizationType || text|| Civilizations(Type)||  Name (Type) of civilization to have city name defined
|-
| CityName || text|| || Not Null, text string for available city name for a city
|}
==Civilization_DisableTechs==
*[[CIV5Technologies]] contains the definitions of the Technologies referenced in this table.
*Any techs set here for a specific civilization won't be available for that civilization to research
{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"
|+Civilization_DisableTechs Table
! scope="col" style="background: #efefef;" | Name
! scope="col" style="background: #efefef;" | Type
! scope="col" style="background: #efefef;" | Reference
|-
| CivilizationType || text|| Civilizations(Type)
|-
| TechType || text|| Technologies(Type)
|}
==Civilization_FreeBuildingClasses==
*[[CIV5BuildingClasses]] contains the definitions of the BuildingClasses referenced in this table.
*This is the free buildings available to a civilization when they found their first city. By default all civilizations get a free palace.
{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"
|+Civilization_FreeBuildingClasses Table
! scope="col" style="background: #efefef;" | Name
! scope="col" style="background: #efefef;" | Type
! scope="col" style="background: #efefef;" | Reference
|-
| CivilizationType || text|| Civilizations(Type)
|-
| BuildingClassType || text|| BuildingClasses(Type)
|}
==Civilization_FreeTechs==
*[[CIV5Technologies]] contains the definitions of the Technologies referenced in this table.
*These are the free techs a civilization starts with. By default all civilizations get agriculture.
{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"
|+Civilization_FreeTechs Table
! scope="col" style="background: #efefef;" | Name
! scope="col" style="background: #efefef;" | Type
! scope="col" style="background: #efefef;" | Reference
|-
| CivilizationType || text|| Civilizations(Type)
|-
| TechType || text|| Technologies(Type)
|}
==Civilization_FreeUnits==
*[[CIV5UnitClasses]] contains the definitions of the UnitClasses referenced in this table.
*[[CIV5UnitAIInfos]] contains the definitions of the UnitAIInfos referenced in this table.
*These are the units the civilization starts with. By default all civilizations are set to start with 1 free settler (Count=1).
{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"
|+Civilization_FreeUnits Table
! scope="col" style="background: #efefef;" | Name
! scope="col" style="background: #efefef;" | Type
! scope="col" style="background: #efefef;" | Reference
|-
| CivilizationType || text|| Civilizations(Type)
|-
| UnitClassType || text|| UnitClasses(Type)
|-
| UnitAIType || text|| UnitAIInfos(Type)
|-
| Count || integer|| 
|}
==Civilization_Leaders==
*This is where leaders are associated to their civilizations. In Civ5 each civilization can only have 1 leader.
{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"
|+Civilization_Leaders Table
! scope="col" style="background: #efefef;" | Name
! scope="col" style="background: #efefef;" | Type
! scope="col" style="background: #efefef;" | Reference
|-
| CivilizationType || text|| Civilizations(Type)
|-
| LeaderheadType || text|| Leaders(Type)
|}
==Civilization_UnitClassOverrides==
*[[CIV5UnitClasses]] contains the definitions of the UnitClasses referenced in this table.
*[[CIV5Units]] contains the definitions of the Units referenced in this table.
Much like the building class overrides this is where unique units are set with the unit they replace for this civilization and civilizations are blocked from building units.
{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"
|+Civilization_UnitClassOverrides Table
! scope="col" style="background: #efefef;" | Name
! scope="col" style="background: #efefef;" | Type
! scope="col" style="background: #efefef;" | Reference
! scope="col" style="background: #efefef;" | Notes
|-
| CivilizationType || text|| Civilizations(Type)|| 
|-
| UnitClassType || text|| UnitClasses(Type)|| Not Null
|-
| UnitType || text|| Units(Type)|| 
|}
==Civilization_Start_Along_Ocean==
*If a civilization has this set the game will attempt to start them along a coastal tile. 
*Each civ can have ONLY one of the 4 start bias, if a civilization has more than one, the 1st one will be used, and others will be ignored 
{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"
|+Civilization_Start_Along_Ocean Table
! scope="col" style="background: #efefef;" | Name
! scope="col" style="background: #efefef;" | Type
! scope="col" style="background: #efefef;" | Reference
! scope="col" style="background: #efefef;" | Default
|-
| CivilizationType || text|| Civilizations(Type)|| 
|-
| StartAlongOcean || boolean|| || false
|}
==Civilization_Start_Along_River==
*If a civilization has this set the game will attempt to start them along a river tile.
*Each civ can have ONLY one of the 4 start bias, if a civilization has more than one, the 1st one will be used, and others will be ignored 
{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"
|+Civilization_Start_Along_River Table
! scope="col" style="background: #efefef;" | Name
! scope="col" style="background: #efefef;" | Type
! scope="col" style="background: #efefef;" | Reference
! scope="col" style="background: #efefef;" | Default
|-
| CivilizationType || text|| Civilizations(Type)|| 
|-
| StartAlongRiver || boolean|| || false
|}
==Civilization_Start_Region_Priority==
*[[CIV5Regions]] contains the definitions of the Regions referenced in this table.
*If a civilization has this set the game will attempt to start them in the specified region. For example Arabia has Desert set for this.
*Each civ can have ONLY one of the 4 start bias, if a civilization has more than one, the 1st one will be used, and others will be ignored
*Multiple entries per civ for each start priority/avoid are supported
{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"
|+Civilization_Start_Region_Priority Table
! scope="col" style="background: #efefef;" | Name
! scope="col" style="background: #efefef;" | Type
! scope="col" style="background: #efefef;" | Reference
|-
| CivilizationType || text|| Civilizations(Type)
|-
| RegionType || text|| Regions(Type)
|}
==Civilization_Start_Region_Avoid==
*[[CIV5Regions]] contains the definitions of the Regions referenced in this table.
*If a civilization has this set the game will attempt to avoid these regions when deciding the civilizations starting location. For example Egypt is set to avoid starts in Jungles.
*Each civ can have ONLY one of the 4 start bias, if a civilization has more than one, the 1st one will be used, and others will be ignored.  Will only be used if the first 3 bias are empty for a given civilization. 
*Multiple entries per civ for each start priority/avoid are supported
{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"
|+Civilization_Start_Region_Avoid Table
! scope="col" style="background: #efefef;" | Name
! scope="col" style="background: #efefef;" | Type
! scope="col" style="background: #efefef;" | Reference
|-
| CivilizationType || text|| Civilizations(Type)
|-
| RegionType || text|| Regions(Type)
|}
{{Civ5_XML_Files}}