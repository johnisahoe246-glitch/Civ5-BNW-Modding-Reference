=CIV5MinorCivTraits.xml=
*The CIV5MinorCivTraits.xml file contains definitions for the MinorCivTraits.
*This information is taken from the CIV5MinorCivTraits.xml file itself.
==MinorCivTraits==
{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"
|+MinorCivTraits Table
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
| TraitIcon || text|| NULL|| 
|-
| TraitTitleIcon || text|| NULL|| 
|-
| BackgroundImage || text|| || 
|}
==MinorCivTraits_Status==
{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"
|+MinorCivTraits_Status Table
! scope="col" style="background: #efefef;" | Name
! scope="col" style="background: #efefef;" | Type
|-
| Type || text
|-
| StatusIcon || text
|-
| StatusMeter || text
|}
{{Civ5_XML_Files}}