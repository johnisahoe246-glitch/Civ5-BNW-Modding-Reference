==CIV5Units.xml==
*The CIV5Units.xml file contains definitions for the units. The tables below indicate the structure of the entries in the CIV5Units file.
*The reference field in the tables below indicates the table and column the entry is linked to.
*This information is taken from the CIV5Units.xml file.
==Units==
*[[CIV5IconTextureAtlases]] contains the definitions of the IconTextureAtlases used in this table
*[[CIV5UnitMovementRates]] contains the definitions of the MovementRates used in this table
*[[CIV5UnitAIInfos]] contains the definitions of the UnitAIInfos used in this table
*[[CIV5UnitClasses]] contains the definitions of the UnitClasses used in this table
*[[CIV5UnitPromotions]] contains the definitions of the UnitPromotions used in this table
*[[CIV5Technologies]] contains the definitions of the Technologies used in this table
*[[CIV5SpecialUnits]] contains the definitions of the SpecialUnits used in this table
*[[CIV5Domains]] contains the definitions of the Domains used in this table
*[[CIV5CombatInfos]] contains the definitions of the CombatInfos used in this table

{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"					
|+ Units Table					
|-	
! Name	
! Type	
! Default	
! Reference	
! Notes
|-	
| ID	|| integer	|| 	|| 	|| Primary Key, Auto-Incremented
|-	
| Type	|| Text	|| 	||[[UnitTypes|Unit(Types)]] || 
|-	
| Description	|| Text	|| NULL	|| 	|| 
|-	
| Civilopedia	|| Text	|| NULL	|| 	|| 
|-	
| Help	|| Text	|| NULL	|| 	|| 
|-	
| Requirements	|| integer	|| 	|| 	|| 
|-	
| Combat	|| integer	|| 0	|| 	|| 
|-	
| RangedCombat	|| integer	|| 0	|| 	|| 
|-	
| Cost	|| integer	|| 0	|| 	|| 
|-	
| Moves	|| integer	|| 0	|| 	|| 
|-	
| Immobile	|| boolean	|| FALSE	|| 	|| 
|-	
| Range	|| integer	|| 0	|| 	|| 
|-	
| BaseSightRange	|| integer	|| 2	|| 	|| 
|-	
| Class	|| Text	|| NULL	|| UnitClasses(Type)	|| 
|-	
| Special	|| Text	|| NULL	|| SpecialUnits(Type)	|| 
|-	
| Capture	|| Text	|| NULL	|| UnitClasses(Type)	|| 
|-	
| CombatClasss	|| Text	|| NULL	|| [[UnitCombatInfos(Type)]]	|| 
|-	
| Domain	|| Text	|| NULL	|| Domains(Type)	|| 
|-	
| DefaultUnitAI	|| Text	|| NULL	|| [[UnitAIInfos(Type)]]	|| 
|-	
| Food	|| boolean	|| FALSE	|| 	|| 
|-	
| NoBadGoodies	|| boolean	|| FALSE	|| 	|| 
|-	
| RivalTerritory	|| boolean	|| FALSE	|| 	|| 
|-	
| MilitarySupport	|| boolean	|| FALSE	|| 	|| 
|-	
| MilitaryProduction	|| boolean	|| FALSE	|| 	|| 
|-	
| Pillage	|| boolean	|| FALSE	|| 	|| 
|-	
| Found	|| boolean	|| FALSE	|| 	|| 
|-	
| CultureBombRadius	|| integer	|| 0	|| 	|| 
|-	
| GoldenAgeTurns	|| integer	|| 0	|| 	|| 
|-	
| IgnoreBuildingDefense	|| boolean	|| FALSE	|| 	|| 
|-	
| PrereqResources	|| boolean	|| FALSE	|| 	|| 
|-	
| Mechanized	|| boolean	|| FALSE	|| 	|| 
|-	
| Suicide	|| boolean	|| FALSE	|| 	|| 
|-	
| PrereqTech	|| Text	|| NULL	|| Technologies(Type)	|| 
|-	
| ObsoleteTech	|| Text	|| NULL	|| Technologies(Type)	|| 
|-	
| GoodyHutUpgradeUnitClass	|| Text	|| NuLL	|| UnitClasses(Type)	|| 
|-	
| HurryCostModifier	|| integer	|| 0	|| 	|| 
|-	
| AdvancedStartCost	|| integer	|| 0	|| 	|| 
|-	
| MinAreaSize	|| integer	|| -1	|| 	|| 
|-	
| AirUnitCap	|| integer	|| 0	|| 	|| 
|-	
| NukeDamageLevel	|| integer	|| -1	|| 	|| 
|-	
| WorkRate	|| integer	|| 0	|| 	|| 
|-	
| NumFreeTechs	|| integer	|| 0	|| 	|| 
|-	
| RushBuilding	|| boolean	|| FALSE	|| 	|| 
|-	
| BaseHurry	|| integer	|| 0	|| 	|| 
|-	
| HurryMultiplier	|| integer	|| 0	|| 	|| 
|-	
| BaseGold	|| integer	|| 0	|| 	|| 
|-	
| NumGoldPerEra	|| integer	|| 0	|| 	|| 
|-	
| SpreadReligion	|| boolean	|| FALSE	|| 	|| 
|-	
| IsReligious	|| boolean	|| FALSE	|| 	|| 
|-	
| CombatLimit	|| integer	|| 100	|| 	|| 
|-	
| RangeAttackOnlyInDomain	|| boolean	|| FALSE	|| 	|| 
|-	
| RangeAttackIgnoreLOS	|| boolean	|| FALSE	|| 	|| 
|-	
| RangedCombatLimit	|| integer	|| 0	|| 	|| 
|-	
| XPValueAttack	|| integer	|| 0	|| 	|| 
|-	
| XPValueDefense	|| integer	|| 0	|| 	|| 
|-	
| SpecialCargo	|| Text	|| NULL	|| SpecialUnits(Type)	|| 
|-	
| DomainCargo	|| Text	|| NULL	|| Domains(Type)	|| 
|-	
| Conscription	|| integer	|| 0	|| 	|| 
|-	
| ExtraMaintenanceCost	|| integer	|| 0	|| 	|| 
|-	
| NoMaintenance	|| boolean	|| 0	|| 	|| 
|-	
| Unhappiness	|| integer	|| 0	|| 	|| 
|-	
| UnitArtInfo	|| Text	|| NULL	|| 	|| 
|-	
| UnitArtInfoCulturalVariation	|| boolean	|| FALSE	|| 	|| 
|-	
| UnitArtInfoEraVariation	|| boolean	|| FALSE	|| 	|| 
|-	
| ProjectPrereq	|| Text	|| NULL	|| Projects(Type)	|| 
|-	
| SpaceshipProject	|| Text	|| NULL	|| Projects(Type)	|| 
|-	
| LeaderPromotion	|| Text	|| NULL	|| UnitPromotions(Type)	|| 
|-	
| LeaderExperience	|| integer	|| 0	|| 	|| 
|-	
| ShowInPedia	|| boolean	|| TRUE	|| 	|| 
|-	
| MoveRate	|| Text	|| BIPED	|| MovementRates(Type)	|| 
|-	
| UnitFlagIconOffset	|| integer	|| 0	|| 	|| 
|-	
| PortraitIndex	|| integer	|| -1	|| 	|| 
|-	
| IconAtlas	|| Text	|| NULL	|| IconTextureAtlases(Atlas)	|| 
|-	
| UnitFlagAtlas	|| Text	|| UNIT_FLAG_ATLAS	|| IconTextureAtlases(Atlas)	|| 
|}

==Unit_AITypes==
*[[CIV5UnitAIInfos]] contains the definitions of the UnitAIInfos used in this table
{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"				
|+ Unit_AITypes Table					
|-	
! scope="col" style="background: #efefef;" | Name	
! scope="col" style="background: #efefef;" | Type	
! scope="col" style="background: #efefef;" | Reference
|-
| UnitType || Text || [[UnitTypes|Unit(Types)]]
|-
| UnitAIType || Text || [[UnitAIInfos(Type)]]
|}

==Unit_Buildings==
*[[CIV5Buildings]] contains the definitions of the Buildings used in this table
{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"				
|+ Unit_Buildings Table					
|-	
! scope="col" style="background: #efefef;" | Name	
! scope="col" style="background: #efefef;" | Type	
! scope="col" style="background: #efefef;" | Reference
|-
| UnitType || Text || [[UnitTypes|Unit(Types)]]
|-
| BuildingType || Text || Buildings(Type)
|}
==Unit_BuildingClassRequireds==
*[[CIV5BuildingClasses]] contains the definitions of the BuildingClasses used in this table
{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"				
|+ Unit_BuildingClassRequireds Table					
|-	
! scope="col" style="background: #efefef;" | Name	
! scope="col" style="background: #efefef;" | Type	
! scope="col" style="background: #efefef;" | Reference
|-
| UnitType || Text || [[UnitTypes|Unit(Types)]]
|-
| BuildingClassType || Text || BuildingClasses(Type)
|}
==Unit_ProductionModifierBuildings==
*[[CIV5Buildings]] contains the definitions of the Buildings used in this table
{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"				
|+ Unit_ProductionModifierBuildings Table					
|-	
! scope="col" style="background: #efefef;" | Name	
! scope="col" style="background: #efefef;" | Type	
! scope="col" style="background: #efefef;" | Reference
|-
| UnitType || Text || [[UnitTypes|Unit(Types)]]
|-
| BuildingType || Text || Buildings(Type)
|-
| ProductionModifier || Integer || 
|}
==Unit_Builds==
*[[CIV5Builds]] contains the definitions of the Builds used in this table
{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"				
|+ Unit_Builds Table					
|-	
! scope="col" style="background: #efefef;" | Name	
! scope="col" style="background: #efefef;" | Type	
! scope="col" style="background: #efefef;" | Reference
|-
| UnitType || Text || [[UnitTypes|Unit(Types)]]
|-
| BuildType || Text || Builds(Type)
|}
==Unit_ClassUpgrades==
*[[CIV5UnitClasses]] contains the definitions of the UnitClasses used in this table
{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"				
|+ Unit_ClassUpgrades Table					
|-	
! scope="col" style="background: #efefef;" | Name	
! scope="col" style="background: #efefef;" | Type	
! scope="col" style="background: #efefef;" | Reference
|-
| UnitType || Text || [[UnitTypes|Unit(Types)]]
|-
| UnitClassType|| Text || UnitClasses(Type)
|}
==Unit_FreePromotions==
*[[CIV5UnitPromotions]] contains the definitions of the UnitPromotions used in this table
{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"				
|+ Unit_FreePromotions Table					
|-	
! scope="col" style="background: #efefef;" | Name	
! scope="col" style="background: #efefef;" | Type	
! scope="col" style="background: #efefef;" | Reference
|-
| UnitType || Text || [[UnitTypes|Unit(Types)]]
|-
| PromotionType|| Text || UnitPromotions(Type)
|}
==Unit_Flavors==
*[[CIV5Flavors]] contains the definitions of the Flavors used in this table
{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"				
|+ Unit_Flavors Table					
|-	
! scope="col" style="background: #efefef;" | Name	
! scope="col" style="background: #efefef;" | Type	
! scope="col" style="background: #efefef;" | Reference
! scope="col" style="background: #efefef;" | Notes
|-
| UnitType || Text || [[UnitTypes|Unit(Types)]] || 
|-
| FlavorType || Text || Flavors(Type) || 
|-
| Flavor || Integer || || Not Null
|}
==Unit_GreatPersons==
*[[CIV5Specialists]] contains the definitions of the Specialists used in this table
{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"				
|+ Unit_GreatPersons Table					
|-	
! scope="col" style="background: #efefef;" | Name	
! scope="col" style="background: #efefef;" | Type	
! scope="col" style="background: #efefef;" | Reference
|-
| UnitType || Text || [[UnitTypes|Unit(Types)]]
|-
| GreatPersonType || Text || Specialists(Type)
|}
==Unit_ResourceQuantityRequirements==
*[[CIV5Resources]] contains the definitions of the Resources used in this table
{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"				
|+ Unit_ResourceQuantityRequirements Table					
|-	
! scope="col" style="background: #efefef;" | Name	
! scope="col" style="background: #efefef;" | Type	
! scope="col" style="background: #efefef;" | Reference
! scope="col" sytle="background: #efefef;" | Default
|-
| UnitType || Text || [[UnitTypes|Unit(Types)]] || 
|-
| ResourceType || Text || Resources(Type) || 
|-
| Cost || Integer || || 1
|}
==Unit_UniqueNames==
{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"				
|+ Unit_UniqueNames Table					
|-	
! scope="col" style="background: #efefef;" | Name	
! scope="col" style="background: #efefef;" | Type	
! scope="col" style="background: #efefef;" | Reference
! scope="col" sytle="background: #efefef;" | Notes
|-
| UnitType || Text || [[UnitTypes|Unit(Types)]] || 
|-
| UniqueName || Text || Language_en_US(Tag) || Not Null
|}
==Unit_NotAITypes==
*This table might not be used according to the xml file.
*[[CIV5UnitAIInfos]] contains the definitions of the UnitAIInfos used in this table
{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"				
|+ Unit_NotAITypes Table					
|-	
! scope="col" style="background: #efefef;" | Name	
! scope="col" style="background: #efefef;" | Type	
! scope="col" style="background: #efefef;" | Reference
|-
| UnitType || Text || [[UnitTypes|Unit(Types)]]
|-
| UnitAIType || Text || UnitAIInfos(Type)
|}
==Unit_ProductionTraits==
*This table might not be used according to the xml file.
*[[CIV5Traits]] contains the definitions of the Traits used in this table
{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"				
|+ Unit_ProductionTraits Table					
|-	
! scope="col" style="background: #efefef;" | Name	
! scope="col" style="background: #efefef;" | Type	
! scope="col" style="background: #efefef;" | Reference
|-
| UnitType || Text || [[UnitTypes|Unit(Types)]]
|-
| TraitType || Text || Traits(Type)
|-
| Trait || Integer || 
|}
==Unit_TechTypes==
*This table might not be used according to the xml file.
*[[CIV5Technologies]] contains the definitions of the Technologies used in this table
{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"				
|+ Unit_TechTypes Table					
|-	
! scope="col" style="background: #efefef;" | Name	
! scope="col" style="background: #efefef;" | Type	
! scope="col" style="background: #efefef;" | Reference
|-
| UnitType || Text || [[UnitTypes|Unit(Types)]]
|-
| TechType || Text || Technologies(Type)
|}

{{Civ5_XML_Files}}