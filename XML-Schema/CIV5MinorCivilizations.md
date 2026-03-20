=CIV5MinorCivilizations.xml=
*The CIV5MinorCivilizations.xml file contains definitions for the MinorCivilizations.
*[[CIV5GameTexInfos_CityStates]] and [[CIV5GameTextInfos_Civilopedia]] contains the text strings for the minor civilizations referenced in this table.
*The reference field in the tables below indicates the table and column the entry is linked to.
*This information is taken from the CIV5MinorCivilizations.xml file itself.
==MinorCivilizations==
*[[CIV5MinorCivTraits]] contains the definitions of the MinorCivTraits referenced in this table.
{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"
|+MinorCivilizations Table
! scope="col" style="background: #efefef;" | Name
! scope="col" style="background: #efefef;" | Type
! scope="col" style="background: #efefef;" | Reference
! scope="col" style="background: #efefef;" | Default
! scope="col" style="background: #efefef;" | Notes
|-
| ID || integer|| || || Primary Key,Autoincrement
|-
| Type || text|| || || Not Null,Unique, Key used to reference this minor civilization, typically in the MINOR_CIV_<name> format
|-
| Description || text|| || || Test string description of the minor civ
|-
| Civilopedia || text|| || || 
|-
| ShortDescription || text|| || || 
|-
| Adjective || text|| || || Text string for the qualifier to things that belong to this minor civ. For Warsaw it is "Warsaw"
|-
| ArtDefineTag || text|| || || 
|-
| DefaultPlayerColor || text|| || NULL|| The default color of this minor civ for borders, unit flags, etc.
|-
| ArtStyleType || text|| || NULL|| Defines the art style used for buildings that are used in this minor civilization's city
|-
| ArtStyleSuffix || text|| || NULL|| Used to pick different flavors of improvements and wonder art
|-
| ArtStylePrefix || text|| || NULL|| Used to pick different flavors of improvements and wonder art
|-
| MinorCivTrait || text|| MinorCivTraits(Type)|| || Not Null, What kind of minor Civ the listed civ is, ie Maritime, Cultured or Militaristic
|}
==MinorCivilization_Flavors==
*[[CIV5Flavors]] contains the definitions of the Flavors referenced in this table.
{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"
|+MinorCivilization_Flavors Table
! scope="col" style="background: #efefef;" | Name
! scope="col" style="background: #efefef;" | Type
! scope="col" style="background: #efefef;" | Reference
|-
| MinorCivType || text|| MinorCivilizations(Type)
|-
| FlavorType || text|| Flavors(Type)
|-
| Flavor || integer|| 
|}
==MinorCivilization_CityNames==
*[[CIV5GameTexInfos_CityStates]] contains the text strings of the city names referenced in this table.
*Lists the city names available to minor civilizations
{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"
|+MinorCivilization_CityNames Table
! scope="col" style="background: #efefef;" | Name
! scope="col" style="background: #efefef;" | Type
! scope="col" style="background: #efefef;" | Reference
! scope="col" style="background: #efefef;" | Notes
|-
| MinorCivType || text|| MinorCivilizations(Type)|| 
|-
| CityName || text|| || Not Null
|}
{{Civ5_XML_Files}}