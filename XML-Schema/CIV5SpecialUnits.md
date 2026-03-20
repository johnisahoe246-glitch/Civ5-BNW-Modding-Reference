=civ5specialunits.xml=
*The civ5specialunits.xml file contains definitions for the SpecialUnits.
*The reference field in the tables below indicates the table and column the entry is linked to.
*This information is taken from the civ5specialunits.xml file itself.
==SpecialUnits==
{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"
|+SpecialUnits Table
! scope="col" style="background: #efefef;" | Name
! scope="col" style="background: #efefef;" | Type
! scope="col" style="background: #efefef;" | Notes
|-
| ID || integer|| Primary Key,Autoincrement
|-
| Type || text|| 
|-
| Description || text|| 
|-
| Valid || boolean|| 
|-
| CityLoad || boolean|| 
|}
==SpecialUnit_CarrierUnitAI==
{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"
|+SpecialUnit_CarrierUnitAI Table
! scope="col" style="background: #efefef;" | Name
! scope="col" style="background: #efefef;" | Type
! scope="col" style="background: #efefef;" | Reference
|-
| SpecialUnitType || text|| SpecialUnits(Type)
|-
| UnitAIType || text|| 
|}
==SpecialUnit_ProductionTraits==
*[[CIV5Traits]] contains the definitions of the Traits referenced in this table.
{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"
|+SpecialUnit_ProductionTraits Table
! scope="col" style="background: #efefef;" | Name
! scope="col" style="background: #efefef;" | Type
! scope="col" style="background: #efefef;" | Reference
|-
| SpecialUnitType || text|| SpecialUnits(Type)
|-
| TraitType || text|| Traits(Type)
|-
| Trait || integer|| 
|}
{{Civ5_XML_Files}}