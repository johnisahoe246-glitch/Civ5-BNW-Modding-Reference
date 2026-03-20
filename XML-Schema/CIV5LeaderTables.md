=civ5leadertables.xml=
*The civ5leadertables.xml file contains definitions for the Leaders.
*The reference field in the tables below indicates the table and column the entry is linked to.
*This information is taken from the civ5leadertables.xml file itself.
*The values for each leader can be found [http://forums.civfanatics.com/showthread.php?t=386066 here].
==Leaders==
*[[CIV5IconTextureAtlases]] contains the definitions of the IconTextureAtlases referenced in this table.
{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"
|+Leaders Table
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
| Description || text|| || || 
|-
| Civilopedia || text|| || || 
|-
| CivilopediaTag || text|| || || 
|-
| ArtDefineTag || text|| || || 
|-
| VictoryCompetitiveness || integer|| || 0|| 
|-
| WonderCompetitiveness || integer|| || 0|| 
|-
| MinorCivCompetitiveness || integer|| || 0|| 
|-
| Boldness || integer|| || 0|| 
|-
| DiploBalance || integer|| || 0|| 
|-
| WarmongerHate || integer|| || 0|| 
|-
| WorkAgainstWillingness || integer|| || 0|| 
|-
| WorkWithWillingness || integer|| || 0|| 
|-
| PortraitIndex || integer|| || -1|| 
|-
| IconAtlas || text|| IconTextureAtlases(Atlas)|| NULL|| 
|}
==Leader_MajorCivApproachBiases==
*[[CIV5MajorCivApproachTypes]] contains the definitions of the MajorCivApproachTypes referenced in this table.
{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"
|+Leader_MajorCivApproachBiases Table
! scope="col" style="background: #efefef;" | Name
! scope="col" style="background: #efefef;" | Type
! scope="col" style="background: #efefef;" | Reference
|-
| LeaderType || text|| Leaders(Type)
|-
| MajorCivApproachType || text|| MajorCivApproachTypes(Type)
|-
| Bias || integer|| 
|}
==Leader_MinorCivApproachBiases==
*[[CIV5MinorCivApproachTypes]] contains the definitions of the MinorCivApproachTypes referenced in this table.
{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"
|+Leader_MinorCivApproachBiases Table
! scope="col" style="background: #efefef;" | Name
! scope="col" style="background: #efefef;" | Type
! scope="col" style="background: #efefef;" | Reference
|-
| LeaderType || text|| Leaders(Type)
|-
| MinorCivApproachType || text|| MinorCivApproachTypes(Type)
|-
| Bias || integer|| 
|}
==Leader_Flavors==
*[[CIV5Flavors]] contains the definitions of the Flavors referenced in this table.
{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"
|+Leader_Flavors Table
! scope="col" style="background: #efefef;" | Name
! scope="col" style="background: #efefef;" | Type
! scope="col" style="background: #efefef;" | Reference
|-
| LeaderType || text|| Leaders(Type)
|-
| FlavorType || text|| Flavors(Type)
|-
| Flavor || integer|| 
|}
==Leader_Traits==
*[[CIV5Traits]] contains the definitions of the Traits referenced in this table.
{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"
|+Leader_Traits Table
! scope="col" style="background: #efefef;" | Name
! scope="col" style="background: #efefef;" | Type
! scope="col" style="background: #efefef;" | Reference
|-
| LeaderType || text|| Leaders(Type)
|-
| TraitType || text|| Traits(Type)
|}
{{Civ5_XML_Files}}