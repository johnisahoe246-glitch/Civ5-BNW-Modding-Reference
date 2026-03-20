=civ5yields.xml=
*The civ5yields.xml file contains definitions for the Yields.
*This information is taken from the civ5yields.xml file itself.
==Yields==
{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"
|+Yields Table
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
| IconString || text|| || 
|-
| HillsChange || integer|| 0|| 
|-
| MountainChange || integer|| 0|| 
|-
| LakeChange || integer|| 0|| 
|-
| CityChange || integer|| 0|| 
|-
| PopulationChangeOffset || integer|| 0|| 
|-
| PopulationChangeDivisor || integer|| 0|| 
|-
| MinCity || integer|| || 
|-
| GoldenAgeYield || integer|| 0|| 
|-
| GoldenAgeYieldThreshold || integer|| 0|| 
|-
| AIWeightPercent || integer|| || 
|}
{{Civ5_XML_Files}}