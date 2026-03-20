'''BeginUnit''' is the subsection that defines a unit at this plot. A unit is defined in the following way:
 BeginUnit
  UnitType=AAAA, UnitOwner=BBBB
  Level=CCCC, Experience=DDDD
  PromotionType=EEEE
  UnitAIType=FFFF
 EndUnit
Where:
* AAAA = the unit type that is at the plot. These values are defined in CIV4UnitInfos.xml.
* BBBB = the unit owner (the player number who owns this unit). The first player is player 0 with the last possible player being player 17 (equals 18 players).
* CCCC = the experience level of the unit. Each level means one more promotion is possible. EG: Level=0 means no promotions, Level=2 means 2 promotions.
* DDDD = the actual experience of the unit. This reflects how many points it has gained towards the next promotion level.
* EEEE = the promotions this unit has. You assign as many PromotionType lines as Levels given to the unit above. These values are defined in CIV4PromotionInfos.xml.
* FFFF = the usage of the unit for the AI. Assigning the correct UnitAIType for a unit is important as it tells the AI what the unit is used for. EG: Settler units should get UnitAIType=UNITAI_SETTLE

{{Civ4_World_Builder}}