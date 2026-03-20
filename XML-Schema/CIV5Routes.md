=CIV5Routes.xml=
*The CIV5Routes.xml file contains definitions for the Routes.
*The reference field in the tables below indicates the table and column the entry is linked to.
*This information is taken from the CIV5Routes.xml file itself.
==Routes==
*[[CIV5IconTextureAtlases]] contains the definitions of the IconTextureAtlases referenced in this table.
{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"
|+Routes Table
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
| AdvancedStartCost || integer|| || 0|| 
|-
| Value || integer|| || 0|| 
|-
| Movement || integer|| || 0|| 
|-
| FlatMovement || integer|| || 0|| 
|-
| GoldMaintenance || integer|| || 0|| 
|-
| Industrial || boolean|| || false|| 
|-
| PortraitIndex || integer|| || -1|| 
|-
| IconAtlas || text|| IconTextureAtlases(Atlas)|| NULL|| 
|-
| Civilopedia || text|| || || 
|}
==Route_Yields==
*[[CIV5Yields]] contains the definitions of the Yields referenced in this table.
{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"
|+Route_Yields Table
! scope="col" style="background: #efefef;" | Name
! scope="col" style="background: #efefef;" | Type
! scope="col" style="background: #efefef;" | Reference
! scope="col" style="background: #efefef;" | Notes
|-
| RouteType || text|| Routes(Type)|| 
|-
| YieldType || text|| Yields(Type)|| 
|-
| Yield || integer|| || Not Null
|}
==Route_TechMovementChanges==
*[[CIV5Technologies]] contains the definitions of the Technologies referenced in this table.
{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"
|+Route_TechMovementChanges Table
! scope="col" style="background: #efefef;" | Name
! scope="col" style="background: #efefef;" | Type
! scope="col" style="background: #efefef;" | Reference
! scope="col" style="background: #efefef;" | Notes
|-
| RouteType || text|| Routes(Type)|| 
|-
| TechType || text|| Technologies(Type)|| 
|-
| MovementChange || integer|| || Not Null
|}
==Route_ResourceQuantityRequirements==
*[[CIV5Resources]] contains the definitions of the Resources referenced in this table.
{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"
|+Route_ResourceQuantityRequirements Table
! scope="col" style="background: #efefef;" | Name
! scope="col" style="background: #efefef;" | Type
! scope="col" style="background: #efefef;" | Reference
! scope="col" style="background: #efefef;" | Notes
|-
| RouteType || text|| Routes(Type)|| 
|-
| ResourceType || text|| Resources(Type)|| 
|-
| Cost || integer|| || Not Null
|}
{{Civ5_XML_Files}}