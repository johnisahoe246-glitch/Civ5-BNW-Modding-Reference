=CIV5AIMilitaryStrategies.xml=
*The CIV5AIMilitaryStrategies.xml file contains definitions for the AIMilitaryStrategies.
*The reference field in the tables below indicates the table and column the entry is linked to.
*This information is taken from the CIV5AIMilitaryStrategies.xml file itself.
==AIMilitaryStrategies==
*[[CIV5Technologies]] contains the definitions of the Technologies referenced in this table.
{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"
|+AIMilitaryStrategies Table
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
| DontUpdateCityFlavors || boolean|| || false|| 
|-
| NoMinorCivs || boolean|| || false|| 
|-
| OnlyMinorCivs || boolean|| || false|| 
|-
| UpdateCitySpecializations || boolean|| || false|| 
|-
| CheckTriggerTurnCount || integer|| || 0|| 
|-
| FirstTurnExecuted || integer|| || 0|| 
|-
| MinimumNumTurnsExecuted || integer|| || 0|| 
|-
| WeightThreshold || integer|| || 0|| 
|-
| TechObsolete || text|| Technologies(Type)|| NULL|| 
|-
| TechPrereq || text|| Technologies(Type)|| NULL|| 
|-
| Advisor || text|| || || 
|-
| AdvisorCounsel || text|| || || 
|-
| AdvisorCounselImportance || integer|| || 1|| 
|}
==AIMilitaryStrategy_Flavors==
*[[CIV5Flavors]] contains the definitions of the Flavors referenced in this table.
{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"
|+AIMilitaryStrategy_Flavors Table
! scope="col" style="background: #efefef;" | Name
! scope="col" style="background: #efefef;" | Type
! scope="col" style="background: #efefef;" | Reference
|-
| AIMilitaryStrategyType || text|| AIMilitaryStrategies(Type)
|-
| FlavorType || text|| Flavors(Type)
|-
| Flavor || integer|| 
|}
==AIMilitaryStrategy_PersonalityFlavorThresholdMods==
*[[CIV5Flavors]] contains the definitions of the Flavors referenced in this table.
{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"
|+AIMilitaryStrategy_PersonalityFlavorThresholdMods Table
! scope="col" style="background: #efefef;" | Name
! scope="col" style="background: #efefef;" | Type
! scope="col" style="background: #efefef;" | Reference
|-
| AIMilitaryStrategyType || text|| AIMilitaryStrategies(Type)
|-
| FlavorType || text|| Flavors(Type)
|-
| Flavor || integer|| 
|}
{{Civ5_XML_Files}}