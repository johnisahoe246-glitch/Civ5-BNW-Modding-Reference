=CIV5BuildingClasses.xml=
*The CIV5BuildingClasses.xml file contains definitions for the BuildingClasses.
*The reference field in the tables below indicates the table and column the entry is linked to.
*This information is taken from the CIV5BuildingClasses.xml file itself.
==BuildingClasses==
{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"
|+BuildingClasses Table
! scope="col" style="background: #efefef;" | Name
! scope="col" style="background: #efefef;" | Type
! scope="col" style="background: #efefef;" | Default
! scope="col" style="background: #efefef;" | Notes
|-
| ID || integer|| || Primary Key,Autoincrement
|-
| Type || text|| || Not Null,Unique
|-
| Description || text|| || 
|-
| DefaultBuilding || text|| || 
|-
| MaxGlobalInstances || integer|| -1|| 
|-
| MaxTeamInstances || integer|| -1|| 
|-
| MaxPlayerInstances || integer|| -1|| 
|-
| ExtraPlayerInstances || integer|| 0|| 
|-
| NoLimit || boolean|| false|| 
|-
| Monument || boolean|| false|| 
|}
==BuildingClass_VictoryThresholds==
*[[CIV5Victories]] contains the definitions of the Victories referenced in this table.
{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"
|+BuildingClass_VictoryThresholds Table
! scope="col" style="background: #efefef;" | Name
! scope="col" style="background: #efefef;" | Type
! scope="col" style="background: #efefef;" | Reference
|-
| BuildingClassType || text|| BuildingClasses(Type)
|-
| VictoryType || text|| Victories(Type)
|-
| Threshold || integer|| 
|}
{{Civ5_XML_Files}}