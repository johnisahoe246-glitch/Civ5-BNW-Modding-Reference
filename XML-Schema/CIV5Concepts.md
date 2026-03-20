==CIV5Concepts.xml==
*The CIV5Concepts.xml file contains definitions for the technologies.
*The reference field in the tables below indicates the table and column the entry is linked to.
*This information is taken from the CIV5Concepts.xml file itself.

==Concepts==
{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"
|+Concepts Table
! scope="col" style="background: #efefef;" | Name
! scope="col" style="background: #efefef;" | Type
! scope="col" style="background: #efefef;" | Notes
|-
| ID || integer|| Primary Key,Autoincrement
|-
| Type || text|| Not Null,Unique
|-
| Topic || text|| Not Null
|-
| Description || text|| Not Null
|-
| Summary || text|| Not Null
|-
| AdvisorQuestion || text|| 
|-
| Advisor || text|| Not Null
|-
| CivilopediaPage || integer|| 
|-
| CivilopediaPageText || text|| 
|-
| CivilopediaHeaderType || text|| 
|}

==Concepts_RelatedConcept==
{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"
|+Concepts_RelatedConcept Table
! scope="col" style="background: #efefef;" | Name
! scope="col" style="background: #efefef;" | Type
! scope="col" style="background: #efefef;" | Reference
|-
| ConceptType || text|| Concepts(Type)
|-
| RelatedConcept || text|| Concepts(Type)
|}

{{Civ5_XML_Files}}