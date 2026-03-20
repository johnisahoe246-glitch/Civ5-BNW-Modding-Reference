=civ5specialists.xml=
*The civ5specialists.xml file contains definitions for the Specialists.
*The reference field in the tables below indicates the table and column the entry is linked to.
*This information is taken from the civ5specialists.xml file itself.
==Specialists==
*[[CIV5IconTextureAtlases]] contains the definitions of the IconTextureAtlases referenced in this table.
{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"
|+Specialists Table
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
| Civilopedia || text|| || || 
|-
| Strategy || text|| || || 
|-
| GreatPeopleTitle || text|| || || 
|-
| PortraitIndex || integer|| || -1|| 
|-
| IconAtlas || text|| IconTextureAtlases(Atlas)|| NULL|| 
|-
| Visible || boolean|| || false|| 
|-
| Cost || integer|| || 0|| 
|-
| Experience || integer|| || 0|| 
|-
| GreatPeopleRateChange || integer|| || 0|| 
|-
| CulturePerTurn || integer|| || 0|| 
|-
| GreatPeopleUnitClass || text|| || NULL|| 
|}
==SpecialistFlavors==
*[[CIV5Flavors]] contains the definitions of the Flavors referenced in this table.
{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"
|+SpecialistFlavors Table
! scope="col" style="background: #efefef;" | Name
! scope="col" style="background: #efefef;" | Type
! scope="col" style="background: #efefef;" | Reference
|-
| SpecialistType || text|| Specialists(Type)
|-
| FlavorType || text|| Flavors(Type)
|-
| Flavor || integer|| 
|}
==SpecialistYields==
*[[CIV5Yields]] contains the definitions of the Yields referenced in this table.
{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"
|+SpecialistYields Table
! scope="col" style="background: #efefef;" | Name
! scope="col" style="background: #efefef;" | Type
! scope="col" style="background: #efefef;" | Reference
|-
| SpecialistType || text|| Specialists(Type)
|-
| YieldType || text|| Yields(Type)
|-
| Yield || integer|| 
|}
{{Civ5_XML_Files}}