==CIV5AIEconomicStrategies.xml==
*The CIV5AIEconomicStrategies.xml file contains definitions for the economic strategies used by the AI.
*The reference field in the tables below indicates the table and column the entry is linked to.
*This information is taken from the CIV5AIEconomicStrategies.xml file itself.

==AIEconomicStrategies==
*[[CIV5Technologies]] contains the definitions of the Technologies used in this table.
{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"				
|+ AIEconomicStrategies Table					
|-	
! scope="col" style="background: #efefef;" | Name	
! scope="col" style="background: #efefef;" | Type	
! scope="col" style="background: #efefef;" | Reference
! scope="col" style="background: #efefef;" | Notes
|-
| ID || Integer || || Primary Key, Autoincrement
|-
| Type || Text || || Not Null, Unique
|-
| DontUpdateCityFlavors || Boolean || False ||
|-
| NoMinorCivs|| Boolean || False ||
|-
| CheckTriggerTurnCount || Integer || 0 ||
|-
| MinimumNumTurnsExecuted || Integer || 0 ||
|-
| WeightThreshold || Integer || 0 ||
|-
| FirstTurnExecuted || Integer || 0 ||
|-
| TechPrereq || Text || NULL || Technologies(Type)
|-
| TechObsolete || Text || NULL || Technologies(Type)
|-
| Advisor || Text || || 
|-
| AdvisorCounsel || Text || || 
|-
| AdvisorCounselImportance || Integer || 1 ||
|}

==AIEconomicStrategy_Flavors==
*[[CIV5Flavors]] contains the definitions of the Flavors used in this table.
{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"				
|+ AIEconomicStrategy_Flavors Table					
|-	
! scope="col" style="background: #efefef;" | Name	
! scope="col" style="background: #efefef;" | Type	
! scope="col" style="background: #efefef;" | Reference
|-
| AIEconomicStrategyType || Text || AIEconomicStrategies(Type)
|-
| FlavorType || Text || Flavors(Type)
|-
| Flavor || Integer ||
|}

==AIEconomicStrategy_PersonalityFlavorThresholdMods==
*[[CIV5Flavors]] contains the definitions of the Flavors used in this table.
{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"				
|+ AIEconomicStrategy_PersonalityFlavorThresholdMods Table
|-	
! scope="col" style="background: #efefef;" | Name	
! scope="col" style="background: #efefef;" | Type	
! scope="col" style="background: #efefef;" | Reference
|-
| AIEconomicStrategyType || Text || AIEconomicStrategies(Type)
|-
| FlavorType || Text || Flavors(Type)
|-
| Flavor || Integer ||
|}

{{Civ5_XML_Files}}