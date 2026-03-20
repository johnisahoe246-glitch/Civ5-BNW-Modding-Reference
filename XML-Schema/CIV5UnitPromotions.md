==CIV5UnitPromotions.xml==
*The CIV5UnitPromotions.xml file contains definitions for the units. The tables below indicate the structure of the entries in the CIV5UnitPromotions file.
*The reference field in the tables below indicates the table and column the entry is linked to.
*This information is taken from the CIV5UnitPromotions.xml file.
==UnitPromotions==
*[[CIV5IconTextureAtlases]] contains the definitions of the IconTextureAtlases used in this table
*[[CIV5Technologies]] contains the definitions of the Technologies used in this table
*[[CIV5InvisibleInfos]] contains the definitions of the InvisibleInfos used in this table
{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"				
|+ UnitPromotions Table					
|-	
! scope="col" style="background: #efefef;" | Name	
! scope="col" style="background: #efefef;" | Type	
! scope="col" style="background: #efefef;" | Default	
! scope="col" style="background: #efefef;" | Reference
! scope="col" style="background: #efefef;" | Notes
|-
| ID || integer || || || Primary Key, Autoincrement
|-
| Type || text || || || Not Null, Unique
|-
| Description || Text || || Language_en_US(Tag) ||
|-
| Help || Text || || Language_en_US(Tag) ||
|-
| DisabledHelp || Text || || ||
|-
| Button || Text || || ||
|-
| PortraitIndex || Integer || 9 || ||
|-
| IconAtlas || Text || ABILITY_ATLAS  || IconTextureAtlases(Atlas) ||
|-
| HotKey || Text || || ||
|-
| HotKeyAlt || Text || || ||
|-
| HotKeyPriority || Integer || 0 || ||
|-
| HotKeyPriorityAlt || Integer || 0 || ||
|-
| OrderPriority || Integer || 0 || ||
|-
| AltDown || Boolean || False || ||
|-
| AltDownAlt || Boolean || False || ||
|-
| ShiftDown || Boolean || False || ||
|-
| ShiftDownAlt || Boolean || False || ||
|-
| CtrlDown || Boolean || False || ||
|-
| CtrlDownAlt || Boolean || False || ||
|-
| Sound || Text || || ||
|-
| CannotBeChosen || Boolean || False || ||
|-
| LostWithUpgrade || Boolean || False || ||
|-
| InstaHeal || Boolean || False || ||
|-
| Leader || Boolean || False || ||
|-
| Blitz || Boolean || False || ||
|-
| Amphib || Boolean || False || ||
|-
| River || Boolean || False || ||
|-
| EnemyRoute || Boolean || False || ||
|-
| RivalTerritory || Boolean || False || ||
|-
| MustSetupToRangedAttack || Boolean || False || ||
|-
| RangedSupportFire || Boolean || False || ||
|-
| CanMoveAfterAttack || Boolean || False || ||
|-
| AlwaysHeal || Boolean || False || ||
|-
| HealsOutsideFriendly || Boolean || False || ||
|-
| HillsDoubleMove || Boolean || False || ||
|-
| RoughTerrainEndsTurn || Boolean || False || ||
|-
| IgnoreTerrainCost || Boolean || False || ||
|-
| HoveringUnit || Boolean || False || ||
|-
| FlatMovementCost || Boolean || False || ||
|-
| CanMoveImpassable || Boolean || False || ||
|-
| NoCapture || Boolean || False || ||
|-
| OnlyDefensive || Boolean || False || ||
|-
| NoDefensiveBonus || Boolean || False || ||
|-
| NukeImmune || Boolean || False || ||
|-
| HiddenNationality || Boolean || False || || |Attention: Seems to be broken in 1.0.1.141, see [http://forums.civfanatics.com/showthread.php?t=404816| here]
|-
| AlwaysHostile || Boolean || False || ||
|-
| NoRevealMap || Boolean || False || ||
|-
| Recon || Boolean || False || ||
|-
| CanMoveAllTerrain || Boolean || False || ||
|-
| FreePillageMoves || Boolean || False || ||
|-
| AirSweepCapable || Boolean || False || ||
|-
| AllowsEmbarkation || Boolean || False || ||
|-
| HealIfDestroyExcludesBarbarians || Boolean || False || ||
|-
| RangeAttackIgnoreLOS || Boolean || False || ||
|-
| RangedAttackModifier || Integer || 0 || ||
|-
| InterceptionCombatModifier || Integer|| 0 || ||
|-
| InterceptionDefenseDamageModifier || Integer || 0 || ||
|-
| AirSweepCombatModifier || Integer || 0 || ||
|-
| ExtraAttacks || Integer || 0 || ||
|-
| ExtraNavalMovement || Integer || 0 || ||
|-
| VisibilityChange || Integer || 0 || ||
|-
| MovesChange || Integer || 0 || ||
|-
| MovesDiscountChange || Integer || 0 || ||
|-
| RangeChange || Integer || 0 || ||
|-
| InterceptChanceChange || Integer || 0 || ||
|-
| NumInterceptionChange || Integer || 0 || ||
|-
| EvasionChange || Integer || 0 || ||
|-
| CargoChange || Integer || 0 || ||
|-
| EnemyHealChange || Integer || 0 || ||
|-
| NeutralHealChange || Integer || 0 || ||
|-
| FriendlyHealChange || Integer || 0 || ||
|-
| SameTileHealChange || Integer || 0 || ||
|-
| AdjacentTileHealChange || Integer || 0 || ||
|-
| CombatPercent || Integer || 0 || ||
|-
| CityAttack || Integer || 0 || ||
|-
| CityDefense || Integer || 0 || ||
|-
| RangedDefenseMod || Integer || 0 || ||
|-
| HillsAttack || Integer || 0 || ||
|-
| HillsDefense || Integer || 0 || ||
|-
| OpenAttack || Integer || 0 || ||
|-
| OpenRangedAttackMod || Integer || 0 || ||
|-
| OpenDefense || Integer || 0 || ||
|-
| RoughAttack || Integer || 0 || ||
|-
| RoughRangedAttackMod || Integer || 0 || ||
|-
| RoughDefense || Integer || 0 || ||
|-
| AttackFortifiedMod || Integer || 0 || ||
|-
| AttackWoundedMod || Integer || 0 || ||
|-
| UpgradeDiscount || Integer || 0 || ||
|-
| ExperiencePercent || Integer || 0 || ||
|-
| AdjacentMod || Integer || 0 || ||
|-
| AttackMod || Integer || 0 || ||
|-
| DefenseMod || Integer || 0 || ||
|-
| DropRange || Integer || 0 || ||
|-
| GreatGeneral || Integer || 0 || ||
|-
| GreatGeneralModifier || Integer || 0 || ||
|-
| FriendlyLandsModifier || Integer || 0 || ||
|-
| FriendlyLandsAttackModifier || Integer || 0 || ||
|-
| OutsideFriendlyLandsModifier || Integer || 0 || ||
|-
| HPHealedIfDestroyEnemy || Integer || 0 || ||
|-
| LayerAnimationPath || Text || "NULL" || ||
|-
| TechPrereq || Text || NULL || Technologies(Type) ||
|-
| Invisible || Text || NULL || InvisibleInfos(Type) ||
|-
| SeeInvisible || Text || NULL || InvisibleInfos(Type) ||
|-
| PromotionPrereq || Text || NULL || UnitPromotions(Type) ||
|-
| PromotionPrereqOr1 || Text || NULL || UnitPromotions(Type) ||
|-
| PromotionPrereqOr2 || Text || NULL || UnitPromotions(Type) ||
|-
| PromotionPrereqOr3 || Text || NULL || UnitPromotions(Type) ||
|-
| PromotionPrereqOr4 || Text || NULL || UnitPromotions(Type) ||
|-
| PediaType || Text || || ||
|-
| PediaEntry || Text || || Language_en_US(Tag) ||
|}

==UnitPromotions_Terrain==
*[[CIV5Terrains]] contains the definitions of the Terrains used in this table
*[[CIV5Technologies]] contains the definitions of the Technologies used in this table
{| border="1" style="text-align:left" cellpadding="3" cellspacing="0" 
|+ UnitPromotions_Terrain Table 
|- 
! scope="col" style="background: #efefef;" | Name 
! scope="col" style="background: #efefef;" | Type 
! scope="col" style="background: #efefef;" | Default
! scope="col" style="background: #efefef;" | Reference
|-
| PromotionType|| Text || || UnitPromotions(Type)
|-
| TerrainType || Text || || Terrains(Type)
|-
| Attack || Integer || 0 ||
|-
| Defense || Integer || 0 ||
|-
| DoubleMove || Boolean || False ||
|-
| Impassable || Boolean || False ||
|-
| PassableTech || Text|| || Technologies(Type)
|}

==UnitPromotions_UnitClasses==
*[[CIV5UnitClasses]] contains the definitions of the UnitClasses used in this table
{| border="1" style="text-align:left" cellpadding="3" cellspacing="0" 
|+ UnitPromotions_UnitClasses Table 
|- 
! scope="col" style="background: #efefef;" | Name 
! scope="col" style="background: #efefef;" | Type 
! scope="col" style="background: #efefef;" | Reference
|-
| PromotionType|| Text || UnitPromotions(Type)
|-
| UnitClassType || Text || UnitClasses(Type)
|-
| Modifier || Integer ||
|-
| Attack || Integer ||
|-
| Defense || Integer ||
|-
| PediaType || Text ||
|}

==UnitPromotions_Domains==
*[[CIV5Domains]] contains the definitions of the Domains used in this table
{| border="1" style="text-align:left" cellpadding="3" cellspacing="0" 
|+ UnitPromotions_Domains Table 
|- 
! scope="col" style="background: #efefef;" | Name 
! scope="col" style="background: #efefef;" | Type 
! scope="col" style="background: #efefef;" | Reference
|-
| PromotionType || Text || UnitPromotions(Type)
|-
| DomainType || Text || Domains(Type)
|-
| Modifier || Integer ||
|-
| PediaType || Text ||
|}


==UnitPromotions_UnitCombatMods==
*[[CIV5UnitCombatInfos]] contains the definitions of the UnitCombatInfos used in this table
{| border="1" style="text-align:left" cellpadding="3" cellspacing="0" 
|+ UnitPromotions_UnitCombatMods Table 
|- 
! scope="col" style="background: #efefef;" | Name 
! scope="col" style="background: #efefef;" | Type 
! scope="col" style="background: #efefef;" | Reference
|-
| PromotionType || Text || UnitPromotions(Type)
|-
| UnitCombtType || Text || UnitCombatInfos(Type)
|-
| Modifier || Integer ||
|-
| PediaType || Text ||
|}

==UnitPromotions_UnitCombats==
*[[CIV5UnitCombatInfos]] contains the definitions of the UnitCombatInfos used in this table
{| border="1" style="text-align:left" cellpadding="3" cellspacing="0" 
|+ UnitPromotions_UnitCombats Table 
|- 
! scope="col" style="background: #efefef;" | Name 
! scope="col" style="background: #efefef;" | Type 
! scope="col" style="background: #efefef;" | Reference
|-
| PromotionType || Text || UnitPromotions(Type)
|-
| UnitCombtType || Text || UnitCombatInfos(Type)
|-
| PediaType || Text ||
|}

{{Civ5_XML_Files}}