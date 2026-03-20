=civ5policybranchtypes.xml=
*The civ5policybranchtypes.xml file contains definitions for the PolicyBranchTypes.
*The reference field in the tables below indicates the table and column the entry is linked to.
*This information is taken from the civ5policybranchtypes.xml file itself.
==PolicyBranchTypes==
*[[CIV5Eras]] contains the definitions of the Eras referenced in this table.
*[[CIV5Policies]] contains the definitions of the Policies referenced in this table.
{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"
|+PolicyBranchTypes Table
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
| Description || text|| Language_en_US(Tag)|| || 
|-
| Civilopedia || text|| Language_en_US(Tag)|| || 
|-
| Strategy || text|| Language_en_US(Tag)|| || 
|-
| Help || text|| Language_en_US(Tag)|| || 
|-
| Title || text|| Language_en_US(Tag)|| || 
|-
| EraPrereq || text|| Eras(Type)|| NULL|| 
|-
| FreePolicy || text|| Policies(Type)|| NULL|| 
|-
| AIMutuallyExclusive || boolean|| || false|| 
|}
==PolicyBranch_Disables==
{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"
|+PolicyBranch_Disables Table
! scope="col" style="background: #efefef;" | Name
! scope="col" style="background: #efefef;" | Type
! scope="col" style="background: #efefef;" | Reference
|-
| PolicyBranchType || text|| PolicyBranchTypes(Type)
|-
| PolicyBranchDisable || text|| PolicyBranchTypes(Type)
|}
{{Civ5_XML_Files}}