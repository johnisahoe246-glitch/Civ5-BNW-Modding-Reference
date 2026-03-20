=civ5eras.xml=
*The civ5eras.xml file contains definitions for the Eras.
*The reference field in the tables below indicates the table and column the entry is linked to.
*This information is taken from the civ5eras.xml file itself.
==Eras==
{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"
|+Eras Table
! scope="col" style="background: #efefef;" | Name
! scope="col" style="background: #efefef;" | Type
! scope="col" style="background: #efefef;" | Default
! scope="col" style="background: #efefef;" | Notes
|-
| ID || integer|| || Primary Key,Autoincrement
|-
| Type || text|| || Not Null,Unique
|-
| Description || text|| || 
|-
| ArtPrefix || text|| || 
|-
| Strategy || text|| || 
|-
| NoGoodies || boolean|| false|| 
|-
| NoBarbUnits || boolean|| false|| 
|-
| NoBarbCities || boolean|| false|| 
|-
| FirstSoundtrackFirst || boolean|| false|| 
|-
| ResearchAgreementCost || integer|| 0|| 
|-
| StartingUnitMultiplier || integer|| 0|| 
|-
| StartingDefenseUnits || integer|| 0|| 
|-
| StartingWorkerUnits || integer|| 0|| 
|-
| StartingExploreUnits || integer|| 0|| 
|-
| StartingGold || integer|| 0|| 
|-
| StartingCulture || integer|| 0|| 
|-
| FreePopulation || integer|| 0|| 
|-
| LaterEraBuildingConstructMod || integer|| 0|| 
|-
| StartPercent || integer|| 0|| 
|-
| BuildingMaintenancePercent || integer|| 0|| 
|-
| GrowthPercent || integer|| 0|| 
|-
| TrainPercent || integer|| 0|| 
|-
| ConstructPercent || integer|| 0|| 
|-
| CreatePercent || integer|| 0|| 
|-
| ResearchPercent || integer|| 0|| 
|-
| BuildPercent || integer|| 0|| 
|-
| ImprovementPercent || integer|| 0|| 
|-
| GreatPeoplePercent || integer|| 0|| 
|-
| CulturePercent || integer|| 0|| 
|-
| EventChancePerTurn || integer|| 0|| 
|-
| SoundtrackSpace || integer|| 0|| 
|-
| CityBombardEffectTag || text|| || 
|-
| AudioUnitVictoryScript || text|| || 
|-
| AudioUnitDefeatScript || text|| || 
|}
==Era_Soundtracks==
{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"
|+Era_Soundtracks Table
! scope="col" style="background: #efefef;" | Name
! scope="col" style="background: #efefef;" | Type
! scope="col" style="background: #efefef;" | Reference
|-
| EraType || text|| Eras(Type)
|-
| SoundTrack || text|| 
|}
==Era_CitySoundscapes==
*[[CIV5CitySizes]] contains the definitions of the CitySizes referenced in this table.
{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"
|+Era_CitySoundscapes Table
! scope="col" style="background: #efefef;" | Name
! scope="col" style="background: #efefef;" | Type
! scope="col" style="background: #efefef;" | Reference
|-
| EraType || text|| Eras(Type)
|-
| CitySizeType || text|| CitySizes(Type)
|-
| SoundscapeScript || text|| 
|}
==Era_NewEraVOs==
{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"
|+Era_NewEraVOs Table
! scope="col" style="background: #efefef;" | Name
! scope="col" style="background: #efefef;" | Type
! scope="col" style="background: #efefef;" | Reference
|-
| EraType || text|| Eras(Type)
|-
| VOScript || text|| 
|}
{{Civ5_XML_Files}}