=civ5projects.xml=
*The civ5projects.xml file contains definitions for the Projects.
*The reference field in the tables below indicates the table and column the entry is linked to.
*This information is taken from the civ5projects.xml file itself.
==Projects==
*[[CIV5IconTextureAtlases]] contains the definitions of the IconTextureAtlases referenced in this table.
{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"
|+Projects Table
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
| Strategy || text|| || || 
|-
| Help || text|| || || 
|-
| Requirements || text|| || || 
|-
| MaxGlobalInstances || integer|| || 0|| 
|-
| MaxTeamInstances || integer|| || 0|| 
|-
| Cost || integer|| || 0|| 
|-
| NukeInterception || integer|| || 0|| 
|-
| CultureBranchesRequired || integer|| || 0|| 
|-
| TechShare || integer|| || 0|| 
|-
| VictoryDelayPercent || integer|| || 0|| 
|-
| Spaceship || boolean|| || false|| 
|-
| Religious || boolean|| || false|| 
|-
| AllowsNukes || boolean|| || false|| 
|-
| MovieDefineTag || text|| || NULL|| 
|-
| VictoryPrereq || text|| || NULL|| 
|-
| TechPrereq || text|| || NULL|| 
|-
| EveryoneSpecialUnit || text|| || NULL|| 
|-
| CreateSound || text|| || NULL|| 
|-
| AnyonePrereqProject || text|| || NULL|| 
|-
| PortraitIndex || integer|| || -1|| 
|-
| IconAtlas || text|| IconTextureAtlases(Atlas)|| NULL|| 
|}
==Project_Flavors==
*[[CIV5Flavors]] contains the definitions of the Flavors referenced in this table.
{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"
|+Project_Flavors Table
! scope="col" style="background: #efefef;" | Name
! scope="col" style="background: #efefef;" | Type
! scope="col" style="background: #efefef;" | Reference
! scope="col" style="background: #efefef;" | Notes
|-
| ProjectType || text|| Projects(Type)|| 
|-
| FlavorType || text|| Flavors(Type)|| 
|-
| Flavor || integer|| || Not Null
|}
==Project_Prereqs==
{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"
|+Project_Prereqs Table
! scope="col" style="background: #efefef;" | Name
! scope="col" style="background: #efefef;" | Type
! scope="col" style="background: #efefef;" | Reference
! scope="col" style="background: #efefef;" | Default
|-
| ProjectType || text|| Projects(Type)|| 
|-
| PrereqProjectType || text|| Projects(Type)|| 
|-
| AmountNeeded || integer|| || 1
|}
==Project_VictoryThresholds==
*[[CIV5Victories]] contains the definitions of the Victories referenced in this table.
{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"
|+Project_VictoryThresholds Table
! scope="col" style="background: #efefef;" | Name
! scope="col" style="background: #efefef;" | Type
! scope="col" style="background: #efefef;" | Reference
! scope="col" style="background: #efefef;" | Default
! scope="col" style="background: #efefef;" | Notes
|-
| ProjectType || text|| Projects(Type)|| || 
|-
| VictoryType || text|| Victories(Type)|| || 
|-
| Threshold || integer|| || || Not Null
|-
| MinThreshold || integer|| || 0|| 
|}
==Project_ResourceQuantityRequirements==
*[[CIV5Resources]] contains the definitions of the Resources referenced in this table.
{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"
|+Project_ResourceQuantityRequirements Table
! scope="col" style="background: #efefef;" | Name
! scope="col" style="background: #efefef;" | Type
! scope="col" style="background: #efefef;" | Reference
! scope="col" style="background: #efefef;" | Notes
|-
| ProjectType || text|| Projects(Type)|| 
|-
| ResourceType || text|| Resources(Type)|| 
|-
| Quantity || integer|| || Not Null
|}
{{Civ5_XML_Files}}