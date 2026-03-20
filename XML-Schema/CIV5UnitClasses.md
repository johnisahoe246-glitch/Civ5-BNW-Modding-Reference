==CIV5UnitClasses.xml==
*The CIV5UnitClasses.xml file contains definitions for the unit classes.
*This information is taken from the CIV5UnitClasses.xml file itself.
==UnitClasses==
{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"				
|+ UnitClasses Table					
|-	
! scope="col" style="background: #efefef;" | Name	
! scope="col" style="background: #efefef;" | Type
! scope="col" style="background: #efefef;" | Default
! scope="col" style="background: #efefef;" | Notes
|-
| ID || integer || || Primary Key, Autoincrement
|-
| Type || Text || || Not Null, Unique
|-
| Description || Text || ||
|-
| MaxGlobalInstances || Integer || -1 ||
|-
| MaxTeamInstances || Integer || -1 ||
|-
| MaxPlayerInstances || Integer || -1 ||
|-
| InstanceCostModifier || Integer || 0 ||
|-
| DefaultUnit || Text || ||
|}

{{Civ5_XML_Files}}