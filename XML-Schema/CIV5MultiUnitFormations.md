=Civ5MultiUnitFormations.xml=
*The Civ5MultiUnitFormations.xml file contains definitions for the MultiUnitPositions.
*The reference field in the tables below indicates the table and column the entry is linked to.
*This information is taken from the Civ5MultiUnitFormations.xml file itself.
==MultiUnitPositions==
{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"
|+MultiUnitPositions Table
! scope="col" style="background: #efefef;" | Name
! scope="col" style="background: #efefef;" | Type
! scope="col" style="background: #efefef;" | Notes
|-
| ID || integer|| Primary Key,Autoincrement
|-
| Type || text|| Not Null,Unique
|-
| Description || text|| 
|-
| Name || text|| 
|}
==MultiUnitFormations==
{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"
|+MultiUnitFormations Table
! scope="col" style="background: #efefef;" | Name
! scope="col" style="background: #efefef;" | Type
! scope="col" style="background: #efefef;" | Notes
|-
| ID || integer|| Primary Key,Autoincrement
|-
| Type || text|| Not Null,Unique
|-
| Description || text|| 
|-
| Name || text|| 
|}
==MultiUnitFormation_SlotEntries==
*[[CIV5UnitAIInfos]] contains the definitions of the UnitAIInfos referenced in this table.
{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"
|+MultiUnitFormation_SlotEntries Table
! scope="col" style="background: #efefef;" | Name
! scope="col" style="background: #efefef;" | Type
! scope="col" style="background: #efefef;" | Reference
|-
| MultiUnitFormationType || text|| MultiUnitFormations(Type)
|-
| PrimaryUnitType || text|| UnitAIInfos(Type)
|-
| SecondaryUnitType || text|| UnitAIInfos(Type)
|-
| MultiUnitPositionType || text|| MultiUnitPositions(Type)
|-
| RequiredSlot || boolean|| 
|}
{{Civ5_XML_Files}}