=civ5gameoptions.xml=
*The civ5gameoptions.xml file contains definitions for the GameOptions.
*This information is taken from the civ5gameoptions.xml file itself.
==GameOptions==
{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"
|+GameOptions Table
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
| Help || text|| || 
|-
| Default || boolean|| false|| 
|-
| Visible || boolean|| true|| 
|-
| SupportsSinglePlayer || boolean|| true|| 
|-
| SupportsMultiplayer || boolean|| true|| 
|}
{{Civ5_XML_Files}}