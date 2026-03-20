=civ5votes.xml=
*The civ5votes.xml file contains definitions for the Votes.
*This information is taken from the civ5votes.xml file itself.
==Votes==
{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"
|+Votes Table
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
| PopulationThreshold || integer|| 0|| 
|-
| MinVoters || integer|| 0|| 
|-
| CityVoting || boolean|| false|| 
|-
| CivVoting || boolean|| false|| 
|-
| SecretaryGeneral || boolean|| false|| 
|-
| Victory || boolean|| false|| 
|-
| FreeTrade || boolean|| false|| 
|-
| NoNukes || boolean|| false|| 
|-
| DefensivePact || boolean|| false|| 
|-
| OpenBorders || boolean|| false|| 
|-
| ForcePeace || boolean|| false|| 
|-
| ForceNoTrade || boolean|| false|| 
|-
| ForceWar || boolean|| false|| 
|-
| AssignCity || boolean|| false|| 
|}
==Vote_DiploVotes==
{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"
|+Vote_DiploVotes Table
! scope="col" style="background: #efefef;" | Name
! scope="col" style="background: #efefef;" | Type
! scope="col" style="background: #efefef;" | Reference
|-
| VoteType || text|| Votes(Type)
|-
| DiploVoteType || text|| 
|}
{{Civ5_XML_Files}}