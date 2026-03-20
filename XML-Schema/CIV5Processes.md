=CIV5Processes.xml=
*The CIV5Processes.xml file contains definitions for the Processes.
*The reference field in the tables below indicates the table and column the entry is linked to.
*This information is taken from the CIV5Processes.xml file itself.
==Processes==
*[[CIV5Technologies]] contains the definitions of the Technologies referenced in this table.
*[[CIV5IconTextureAtlases]] contains the definitions of the IconTextureAtlases referenced in this table.
{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"
|+Processes Table
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
| Strategy || text|| || || 
|-
| TechPrereq || text|| Technologies(Type)|| || 
|-
| PortraitIndex || integer|| || -1|| 
|-
| IconAtlas || text|| IconTextureAtlases(Atlas)|| NULL|| 
|}
==Process_ProductionYields==
*[[CIV5Yields]] contains the definitions of the Yields referenced in this table.
{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"
|+Process_ProductionYields Table
! scope="col" style="background: #efefef;" | Name
! scope="col" style="background: #efefef;" | Type
! scope="col" style="background: #efefef;" | Reference
! scope="col" style="background: #efefef;" | Notes
|-
| ProcessType || text|| Processes(Type)|| 
|-
| YieldType || text|| Yields(Type)|| 
|-
| Yield || integer|| || Not Null
|}
{{Civ5_XML_Files}}