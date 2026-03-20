=civ5playercolors.xml=
*The civ5playercolors.xml file contains definitions for the PlayerColors.
*The reference field in the tables below indicates the table and column the entry is linked to.
*This information is taken from the civ5playercolors.xml file itself.
==PlayerColors==
*[[CIV5Colors]] contains the definitions of the Colors referenced in this table.
{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"
|+PlayerColors Table
! scope="col" style="background: #efefef;" | Name
! scope="col" style="background: #efefef;" | Type
! scope="col" style="background: #efefef;" | Reference
! scope="col" style="background: #efefef;" | Notes
|-
| ID || integer|| || Primary Key,Autoincrement
|-
| Type || text|| || Not Null,Unique
|-
| PrimaryColor || text|| Colors(type)|| Not Null
|-
| SecondaryColor || text|| Colors(Type)|| Not Null
|-
| TextColor || text|| Colors(Type)|| Not Null
|}
{{Civ5_XML_Files}}