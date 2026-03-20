=Civ5Builds.xml=
*The Civ5Builds.xml file contains definitions for the Builds.
*The reference field in the tables below indicates the table and column the entry is linked to.
*This information is taken from the Civ5Builds.xml file itself.
==Builds==
{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"
|+Builds Table
! scope="col" style="background: #efefef;" | Name
! scope="col" style="background: #efefef;" | Type
! scope="col" style="background: #efefef;" | Default
! scope="col" style="background: #efefef;" | Notes
|-
| ID || integer|| || Primary Key,Autoincrement
|-
| Type || text|| || Not Null,Unique, [[BuildTypes]]
|-
| Description || text|| || 
|-
| Help || text|| || 
|-
| DisabledHelp || text|| || 
|-
| Recommendation || text|| || 
|-
| HotKey || text|| || 
|-
| HotKeyAlt || text|| || 
|-
| HotKeyPriority || integer|| 0|| 
|-
| HotKeyPriorityAlt || integer|| 0|| 
|-
| OrderPriority || integer|| 0|| 
|-
| AltDown || boolean|| false|| 
|-
| AltDownAlt || boolean|| false|| 
|-
| ShiftDown || boolean|| false|| 
|-
| ShiftDownAlt || boolean|| false|| 
|-
| CtrlDown || boolean|| false|| 
|-
| CtrlDownAlt || boolean|| false|| 
|-
| Time || integer|| || 
|-
| Cost || integer|| 0|| 
|-
| CostIncreasePerImprovement || integer|| 0|| 
|-
| Kill || boolean|| false|| 
|-
| Repair || boolean|| false|| 
|-
| RemoveRoute || boolean|| false|| 
|-
| PrereqTech || text|| NULL|| 
|-
| ImprovementType || text|| NULL||  [[ImprovementTypes]]
|-
| RouteType || text|| NULL|| 
|-
| EntityEvent || text|| NULL|| 
|}

==BuildFeatures==
{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"
|+BuildFeatures Table
! scope="col" style="background: #efefef;" | Name
! scope="col" style="background: #efefef;" | Type
! scope="col" style="background: #efefef;" | Reference
! scope="col" style="background: #efefef;" | Default
|-
| BuildType || text|| Builds(Type)|| 
|-
| FeatureType || text|| || 
|-
| PrereqTech || text|| || 
|-
| Time || integer|| || 
|-
| Production || integer|| || 0
|-
| Cost || integer|| || 0
|-
| Remove || boolean|| || false
|}
{{Civ5_XML_Files}}