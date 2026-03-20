=CIV5TacticalMoves.xml=
*The CIV5TacticalMoves.xml file contains definitions for the TacticalMoves.
*This information is taken from the CIV5TacticalMoves.xml file itself.
==TacticalMoves==
{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"
|+TacticalMoves Table
! scope="col" style="background: #efefef;" | Name
! scope="col" style="background: #efefef;" | Type
! scope="col" style="background: #efefef;" | Default
! scope="col" style="background: #efefef;" | Notes
|-
| ID || integer|| || Primary Key,Autoincrement
|-
| Type || text|| || Not Null,Unique
|-
| OperationsCanRecruit || boolean|| true|| 
|-
| DominanceZoneMove || boolean|| false|| 
|-
| OffenseFlavorWeight || integer|| || 
|-
| DefenseFlavorWeight || integer|| || 
|-
| Priority || integer|| || 
|}
{{Civ5_XML_Files}}