==CIV5AICityStrategies.xml==
*The CIV5AICityStrategies.xml file contains definitions for the technologies.
*The reference field in the tables below indicates the table and column the entry is linked to.
*This information is taken from the CIV5AICityStrategies.xml file itself.
<blockquote>
Entries in this file define the attributes of various AI City Strategies.  Entries can be completely removed safely, but be careful when changing values, as this can result in unexpected AI behavior.  Defines which also help shape use of AI City Strategies are located in the GlobalAIDefines.xml file inside the XML\AI\ directory.  Flavors determine which Units, Buildings, Wonders, etc. a City wants to obtain.  WeightThreshold is used in the AI code to determine if this City Strategy should be adopted - note that it's used in a different way by each City Strategy.  PersonalityFlavorThresholdMods change the liklihood of a City Strategy being adopted based on the AI player's intrinsic Flavors.  As with WeightThreshold, the use of the PersonalityFlavorMod values isn't consistent across all City Strategies.  For more information on how these City Strategies work, reference CvCityStrategyAI.cpp in the GameCoreDLL project.
</blockquote>

==AICityStrategies==
*[[CIV5Technologies]] contains the definitions of the Technologies referenced in this table.
{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"
|+AICityStrategies Table
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
| CheckTriggerTurnCount || integer|| || || 
|-
| MinimumNumTurnsExecuted || integer|| || || 
|-
| WeightThreshold || integer|| || 0|| 
|-
| NoMinorCivs || boolean|| || false|| 
|-
| Permanent || boolean|| || false|| 
|-
| TechPrereq || text|| Technologies(Type)|| NULL|| 
|-
| TechObsolete || text|| Technologies(Type)|| NULL|| 
|-
| Advisor || text|| || || 
|-
| AdvisorCounsel || text|| || || 
|-
| AdvisorCounselImportance || integer|| || 1|| 
|}

==AICityStrategy_Flavors==
*[[CIV5Flavors]] contains the definitions of the Flavors referenced in this table.
{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"
|+AICityStrategy_Flavors Table
! scope="col" style="background: #efefef;" | Name
! scope="col" style="background: #efefef;" | Type
! scope="col" style="background: #efefef;" | Reference
|-
| AICityStrategyType || text|| AICityStrategies(Type)
|-
| FlavorType || text|| Flavors(Type)
|-
| Flavor || integer|| 
|}

==AICityStrategy_PersonalityFlavorThresholdMods==
*[[CIV5Flavors]] contains the definitions of the Flavors referenced in this table.
{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"
|+AICityStrategy_PersonalityFlavorThresholdMods Table
! scope="col" style="background: #efefef;" | Name
! scope="col" style="background: #efefef;" | Type
! scope="col" style="background: #efefef;" | Reference
|-
| AICityStrategyType || text|| AICityStrategies(Type)
|-
| FlavorType || text|| Flavors(Type)
|-
| Flavor || integer|| 
|}

{{Civ5_XML_Files}}