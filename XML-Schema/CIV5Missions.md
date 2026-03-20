=Civ5Missions.xml=
*The Civ5Missions.xml file contains definitions for the Missions.
*The reference field in the tables below indicates the table and column the entry is linked to.
*This information is taken from the Civ5Missions.xml file itself.
==Missions==
{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"
|+Missions Table
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
| Help || text|| Language_en_US(Tag)|| || 
|-
| DisabledHelp || text|| Language_en_US(Tag)|| || 
|-
| HotKey || text|| || || 
|-
| HotKeyAlt || text|| || || 
|-
| HotKeyPriority || integer|| || 0|| 
|-
| HotKeyPriorityAlt || integer|| || 0|| 
|-
| OrderPriority || integer|| || 0|| 
|-
| AltDown || boolean|| || false|| 
|-
| AltDownAlt || boolean|| || false|| 
|-
| ShiftDown || boolean|| || false|| 
|-
| ShiftDownAlt || boolean|| || false|| 
|-
| CtrlDown || boolean|| || false|| 
|-
| CtrlDownAlt || boolean|| || false|| 
|-
| Visible || boolean|| || false|| 
|-
| Waypoint || text|| || NULL|| 
|-
| Time || integer|| || || 
|-
| Target || boolean|| || || 
|-
| Build || boolean|| || || 
|-
| Sound || boolean|| || || 
|-
| EntityEventType || text|| || || 
|}
{{Civ5_XML_Files}}