=CIV5EmphasizeInfos.xml=
*The CIV5EmphasizeInfos.xml file contains definitions for the EmphasizeInfos.
*The reference field in the tables below indicates the table and column the entry is linked to.
*This information is taken from the CIV5EmphasizeInfos.xml file itself.
==EmphasizeInfos==
{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"
|+EmphasizeInfos Table
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
| Strategy || text|| 
|-
| AvoidGrowth || boolean|| 
|-
| GreatPeople || boolean|| 
|}
==EmphasizeInfo_Yields==
*[[CIV5Yields]] contains the definitions of the Yields referenced in this table.
{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"
|+EmphasizeInfo_Yields Table
! scope="col" style="background: #efefef;" | Name
! scope="col" style="background: #efefef;" | Type
! scope="col" style="background: #efefef;" | Reference
! scope="col" style="background: #efefef;" | Notes
|-
| EmphasizeType || text|| EmphasizeInfos(Type)|| 
|-
| YieldType || text|| Yields(Type)|| 
|-
| Yield || integer|| || Not Null
|}
{{Civ5_XML_Files}}