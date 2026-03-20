=civ5votesources.xml=
*The civ5votesources.xml file contains definitions for the VoteSources.
*This information is taken from the civ5votesources.xml file itself.
==VoteSources==
{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"
|+VoteSources Table
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
| PopupText || text|| || 
|-
| SecretaryGeneralText || text|| || 
|-
| VoteInterval || integer|| || 
|-
| FreeSpecialist || text|| NULL|| 
|-
| Policy || text|| NULL|| 
|}
{{Civ5_XML_Files}}