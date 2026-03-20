=Civ5AnimationPaths.xml=
*The Civ5AnimationPaths.xml file contains definitions for the AnimationPaths.
*The reference field in the tables below indicates the table and column the entry is linked to.
*This information is taken from the Civ5AnimationPaths.xml file itself.
==AnimationPaths==
{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"
|+AnimationPaths Table
! scope="col" style="background: #efefef;" | Name
! scope="col" style="background: #efefef;" | Type
! scope="col" style="background: #efefef;" | Default
! scope="col" style="background: #efefef;" | Notes
|-
| ID || integer|| || Primary Key,Autoincrement
|-
| Type || text|| || 
|-
| MissionPath || boolean|| false|| 
|}
==AnimationPath_Entries==
{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"
|+AnimationPath_Entries Table
! scope="col" style="background: #efefef;" | Name
! scope="col" style="background: #efefef;" | Type
! scope="col" style="background: #efefef;" | Reference
! scope="col" style="background: #efefef;" | Default
|-
| AnimationPathType || text|| AnimationPaths(Type)|| 
|-
| Category || text|| || 
|-
| Operator || text|| || 
|-
| Parameter || float|| || 0
|}
{{Civ5_XML_Files}}