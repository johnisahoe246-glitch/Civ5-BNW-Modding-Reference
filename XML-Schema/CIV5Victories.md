=Civ5Victories.xml=
*The Civ5Victories.xml file contains definitions for the victories.
*The reference field in the tables below indicates the table and column the entry is linked to.
*This information is taken from the Civ5Victories.xml file itself.
==Victories==
{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"
|+Victories Table
! scope="col" style="background: #efefef;" | Name
! scope="col" style="background: #efefef;" | Type
! scope="col" style="background: #efefef;" | Default
! scope="col" style="background: #efefef;" | Notes
|-
| ID || integer|| || Primary Key,Autoincrement
|-
| Type || text|| || Unique, Not Null
|-
| Description || text|| || 
|-
| VictoryStatement || text|| || 
|-
| VictoryBackground || text|| || 
|-
| Civilopedia || text|| || 
|-
| WinsGame || boolean|| false|| 
|-
| TargetScore || boolean|| false|| 
|-
| EndScore || boolean|| false|| 
|-
| Conquest || boolean|| false|| 
|-
| DiploVote || boolean|| false|| 
|-
| Permanent || boolean|| false|| 
|-
| ReligionInAllCities || boolean|| false|| 
|-
| FindAllNaturalWonders || boolean|| false||
|-
| PopulationPercentLead || integer|| 0|| 
|-
| LandPercent || integer|| 0|| 
|-
| MinLandPercent || integer|| 0|| 
|-
| NumCultureCities || integer|| 0|| 
|-
| TotalCultureRation || integer|| 0|| 
|-
| VictoryDelayTurns || integer|| 0|| 
|-
| VictoryMovie || text|| || 
|-
|CityCulture || text|| NULL|| 
|-
| Audio || text|| NULL|| 
|}
==VictoryPointAwards==
{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"
|+VictoryPointAwards Table
! scope="col" style="background: #efefef;" | Name
! scope="col" style="background: #efefef;" | Type
! scope="col" style="background: #efefef;" | Reference
! scope="col" style="background: #efefef;" | Notes
|-
| VictoryType || text|| Victories(Type)|| Primary Key, Autoincrement
|-
| VictoryPoints || integer|| || Not Null
|}
==HistoricRankings==
{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"
|+HistoricRankings Table
! scope="col" style="background: #efefef;" | Name
! scope="col" style="background: #efefef;" | Type
! scope="col" style="background: #efefef;" | Reference
! scope="col" style="background: #efefef;" | Notes/Default
|-
| ID || integer|| || Primary Key, Autoincrement
|-
| HistoricLeader || text|| || 
|-
| LeaderQuote || text|| || 
|-
| LeaderScore || integer|| || 0
|}
{{Civ5_XML_Files}}