==CIV5Technologies.xml==
*The CIV5Technologies.xml file contains definitions for the technologies.  The tables below indicate the structure of the entries in the Civ5Technologies file.
*This file defines data for the Technology, Technology_PrereqTechs, and Technology_Flavors tables.
*The reference field in the tables below indicates the table and column the entry is linked to.
*This information is taken from the CIV5Technologies.xml file itself.

==Technology==
{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"				
|+ Technology Table					
|-	
! scope="col" style="background: #efefef;" | Name	
! scope="col" style="background: #efefef;" | Type	
! scope="col" style="background: #efefef;" | Default	
! scope="col" style="background: #efefef;" | Reference	
! scope="col" style="background: #efefef;" | Notes
|-	
| ID	|| integer	|| 	|| 	|| Primary Key, Auto-Incremented
|-	
| Type	|| Text	|| 	|| 	|| 
|-	
| Description	|| Text	|| NULL	|| 	|| 
|-	
| Civilopedia	|| Text	|| NULL	|| 	|| 
|-	
| Help	|| Text	|| NULL	|| 	|| 
|-	
| AIWeight	|| integer	|| 0	|| 	|| 
|-	
| AITradeModifier	|| integer	|| 0	|| 	|| 
|-	
| Cost	|| integer	|| 0	|| 	|| 
|-	
| AdvancedStartCost	|| integer	|| -1	|| 	|| 
|-	
| Era	|| Text	|| NULL	|| 	|| 
|-	
| FirstFreeUnitClass	|| Text	|| NULL	|| 	|| 
|-	
| FeatureProductionModifier	|| integer	|| 0	|| 	|| 
|-	
| WorkerSpeedModifier	|| integer	|| 0	|| 	|| 
|-	
| FirstFreeTechs	|| integer	|| 0	|| 	|| 
|-	
| EmbarkedMoveChange	|| integer	|| 0	|| 	|| 
|-	
| EndsGame	|| boolean	|| FALSE	|| 	|| 
|-	
| AllowsEmbarking	|| boolean	|| FALSE	|| 	|| 
|-	
| EmbarkedAllWaterPassage	|| boolean	|| FALSE	|| 	|| 
|-	
| AllowsBarbarianBoats	|| boolean	|| FALSE	|| 	|| 
|-	
| Repeat	|| boolean	|| FALSE	|| 	|| 
|-	
| Trade	|| boolean	|| FALSE	|| 	|| 
|-	
| Disable	|| boolean	|| FALSE	|| 	|| 
|-	
| GoodyTech	|| boolean	|| FALSE	|| 	|| 
|-	
| ExtraWaterSeeFrom	|| boolean	|| FALSE	|| 	|| 
|-	
| MapCentering	|| boolean	|| FALSE	|| 	|| 
|-	
| MapVisible	|| boolean	|| FALSE	|| 	|| 
|-	
| MapTrading	|| boolean	|| FALSE	|| 	|| 
|-	
| TechTrading	|| boolean	|| FALSE	|| 	|| 
|-	
| GoldTrading	|| boolean	|| FALSE	|| 	|| 
|-	
| OpenBordersTradingAllowed	|| boolean	|| FALSE	|| 	|| 
|-	
| DefensivePactTradingAllowed	|| boolean	|| FALSE	|| 	|| 
|-	
| ResearchAgreementTradingAllowed	|| boolean	|| FALSE	|| 	|| 
|-	
| TradeAgreementTradingAllowed	|| boolean	|| FALSE	|| 	|| 
|-	
| PermanentAllianceTradingAllowed	|| boolean	|| FALSE	|| 	|| 
|-	
| BridgeBuilding	|| boolean	|| FALSE	|| 	|| 
|-	
| WaterWork	|| boolean	|| FALSE	|| 	|| 
|-	
| GridX	|| integer	|| 0	|| 	|| 
|-	
| GridY	|| integer	|| 0	|| 	|| 
|-	
| Quote	|| Text	|| NULL	|| 	|| 
|-	
| PortraitIndex	|| integer	|| -1	|| 	|| 
|-	
| IconAtlas	|| Text	|| NULL	|| IconTextureAtlases(Atlas)	|| 
|-	
| AudioIntro	|| Text	|| NULL	|| 	|| 
|-	
| AudioIntroHeader	|| Text	|| NULL	|| 	|| 
|}

==Technology_DomainExtraMoves==
*[[CIV5Domains]] contains the definitions of the DomainType used in this table.
{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"
|+ Technology_DomainExtraMoves Table					
|-	
! scope="col" style="background: #efefef;" | Name	
! scope="col" style="background: #efefef;" | Type	
! scope="col" style="background: #efefef;" | Reference
|-
| TechType || Text || Technologies(Type)
|-
| DomainType || Text || Domains(Type)
|-
| Moves || Integer ||
|}

==Technology_Flavors==
{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"
|+ Technology_Flavors Table					
|-	
! scope="col" style="background: #efefef;" | Name	
! scope="col" style="background: #efefef;" | Type	
! scope="col" style="background: #efefef;" | Reference
|-
| TechType || Text || Technologies(Type)
|-
| FlavorType || Text || [[Flavors(Type)]]
|-
| Flavor|| Integer ||
|}

==Technology_ORPrereqTechs==
{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"
|+ Technology_ORPrereqTechs Table					
|-	
! scope="col" style="background: #efefef;" | Name	
! scope="col" style="background: #efefef;" | Type	
! scope="col" style="background: #efefef;" | Reference
|-
| TechType || Text || Technologies(Type)
|-
| PrereqTech || Text || Technologies(Type)
|}

==Technology_PrereqTechs==
{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"
|+ Technology_PrereqTechs Table					
|-	
! scope="col" style="background: #efefef;" | Name	
! scope="col" style="background: #efefef;" | Type	
! scope="col" style="background: #efefef;" | Reference
|-
| TechType || Text || Technologies(Type)
|-
| PrereqTech || Text || Technologies(Type)
|}

{{Civ5_XML_Files}}