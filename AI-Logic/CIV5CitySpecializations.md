=CIV5CitySpecializations.xml=
*The CIV5CitySpecializations.xml file contains definitions for the CitySpecializations.
*The reference field in the tables below indicates the table and column the entry is linked to.
*This information is taken from the CIV5CitySpecializations.xml file itself.
==CitySpecializations==
*[[CIV5Yields]] contains the definitions of the Yields referenced in this table.
{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"
|+CitySpecializations Table
! scope="col" style="background: #efefef;" | Name
! scope="col" style="background: #efefef;" | Type
! scope="col" style="background: #efefef;" | Reference
! scope="col" style="background: #efefef;" | Notes
|-
| ID || integer|| || Primary Key,Autoincrement
|-
| Type || text|| || Not Null,Unique
|-
| YieldType || text|| Yields(Type)|| 
|-
| Subtype || integer|| || 
|-
| MustBeCoastal || boolean|| || 
|-
| IsWonder || boolean|| || 
|-
| IsDefault || boolean|| || 
|-
| IsOperationUnitProvider || boolean|| || 
|}
==CitySpecialization_Flavors==
*[[CIV5Flavors]] contains the definitions of the Flavors referenced in this table.
{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"
|+CitySpecialization_Flavors Table
! scope="col" style="background: #efefef;" | Name
! scope="col" style="background: #efefef;" | Type
! scope="col" style="background: #efefef;" | Reference
|-
| CitySpecializationType || text|| CitySpecializations(Type)
|-
| FlavorType || text|| Flavors(Type)
|-
| Flavor || integer|| 
|}
{{Civ5_XML_Files}}