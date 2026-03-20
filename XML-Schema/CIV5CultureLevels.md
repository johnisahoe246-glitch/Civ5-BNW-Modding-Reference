=CIV5CultureLevels.xml=
*The CIV5CultureLevels.xml file contains definitions for the CultureLevels.
*The reference field in the tables below indicates the table and column the entry is linked to.
*This information is taken from the CIV5CultureLevels.xml file itself.
==CultureLevels==
{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"
|+CultureLevels Table
! scope="col" style="background: #efefef;" | Name
! scope="col" style="background: #efefef;" | Type
! scope="col" style="background: #efefef;" | Default
! scope="col" style="background: #efefef;" | Notes
|-
| ID || integer|| || Primary Key,Autoincrement
|-
| Type || text|| || Not Null,Unique
|-
| Description || text|| || 
|-
| CityDefenseModifier || integer|| 0|| 
|}
==CultureLevel_SpeedThresholds==
*[[CIV5GameSpeeds]] contains the definitions of the GameSpeeds referenced in this table.
{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"
|+CultureLevel_SpeedThresholds Table
! scope="col" style="background: #efefef;" | Name
! scope="col" style="background: #efefef;" | Type
! scope="col" style="background: #efefef;" | Reference
! scope="col" style="background: #efefef;" | Default
|-
| CultureLevelType || text|| CultureLevels(Type)|| 
|-
| GameSpeedType || text|| GameSpeeds(Type)|| 
|-
| Threshold || integer|| || 0
|}
{{Civ5_XML_Files}}