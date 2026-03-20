=CIV5HurryInfos.xml=
*The CIV5HurryInfos.xml file contains definitions for the HurryInfos.
*The reference field in the tables below indicates the table and column the entry is linked to.
*This information is taken from the CIV5HurryInfos.xml file itself.
==HurryInfos==
*[[CIV5Policies]] contains the definitions of the Policies referenced in this table.
{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"
|+HurryInfos Table
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
| PolicyPrereq || text|| Policies(Type)|| || 
|-
| GoldPerProduction || integer|| || 0|| 
|-
| ProductionPerPopulation || integer|| || 0|| 
|-
| GoldPerBeaker || integer|| || 0|| 
|-
| GoldPerCulture || integer|| || 0|| 
|}
{{Civ5_XML_Files}}