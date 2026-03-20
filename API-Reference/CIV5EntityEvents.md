=civ5entityevents.xml=
*The civ5entityevents.xml file contains definitions for the EntityEvents.
*The reference field in the tables below indicates the table and column the entry is linked to.
*This information is taken from the civ5entityevents.xml file itself.
==EntityEvents==
{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"
|+EntityEvents Table
! scope="col" style="background: #efefef;" | Name
! scope="col" style="background: #efefef;" | Type
! scope="col" style="background: #efefef;" | Default
! scope="col" style="background: #efefef;" | Notes
|-
| ID || integer|| || Primary Key,Autoincrement
|-
| Type || text|| || 
|-
| UpdateFormation || boolean|| false|| 
|}
==EntityEvent_AnimationPaths==
*[[CIV5AnimationPaths]] contains the definitions of the AnimationPaths referenced in this table.
{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"
|+EntityEvent_AnimationPaths Table
! scope="col" style="background: #efefef;" | Name
! scope="col" style="background: #efefef;" | Type
! scope="col" style="background: #efefef;" | Reference
|-
| EntityEventType || text|| EntityEvents(Type)
|-
| AnimationPathType || text|| AnimationPaths(Type)
|}
{{Civ5_XML_Files}}