=civ5gamespeeds.xml=
*The civ5gamespeeds.xml file contains definitions for the GameSpeeds.
*The reference field in the tables below indicates the table and column the entry is linked to.
*This information is taken from the civ5gamespeeds.xml file itself.
==GameSpeeds==
*[[CIV5IconTextureAtlases]] contains the definitions of the IconTextureAtlases referenced in this table.
{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"
|+GameSpeeds Table
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
| Help || text|| || || 
|-
| DealDuration || integer|| || 0|| 
|-
| GrowthPercent || integer|| || 0|| 
|-
| TrainPercent || integer|| || 0|| Percent of production cost for units
|-
| ConstructPercent || integer|| || 0|| Percent of production cost for buildings
|-
| CreatePercent || integer|| || 0|| 
|-
| ResearchPercent || integer|| || 0|| Multiplier percent applied to base research costs
|-
| GoldPercent || integer|| || 0|| 
|-
| GoldGiftMod || integer|| || 0|| 
|-
| BuildPercent || integer|| || 0|| Multiplier for time it takes workers to build things(routes/improvements)
|-
| ImprovementPercent || integer|| || 0|| 
|-
| GreatPeoplePercent || integer|| || 0|| 
|-
| CulturePercent || integer|| || 0|| 
|-
| BarbPercent || integer|| || 0|| 
|-
| FeatureProductionPercent || integer|| || 0|| 
|-
| UnitDiscoverPercent || integer|| || 0|| 
|-
| UnitHurryPercent || integer|| || 0|| 
|-
| UnitTradePercent || integer|| || 0|| 
|-
| GoldenAgePercent || integer|| || 0|| 
|-
| HurryPercent || integer|| || 0|| 
|-
| InflationPercent || integer|| || 0|| 
|-
| InflationOffset || integer|| || 0|| 
|-
| VictoryDelayPercent || integer|| || 0|| 
|-
| PortraitIndex || integer|| || -1|| 
|-
| IconAtlas || text|| IconTextureAtlases(Atlas)|| NULL|| 
|}

==GameSpeed_Turns==
{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"
|+GameSpeed_Turns Table
! scope="col" style="background: #efefef;" | Name
! scope="col" style="background: #efefef;" | Type
! scope="col" style="background: #efefef;" | Reference
|-
| GameSpeedType || text|| GameSpeeds(Type)
|-
| MonthIncrement || integer|| 
|-
| TurnsPerIncrement || integer|| 
|}
{{Civ5_XML_Files}}