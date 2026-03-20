=Civ5Automates.xml=
*The Civ5Automates.xml file contains definitions for the Automates.
*The reference field in the tables below indicates the table and column the entry is linked to.
*This information is taken from the Civ5Automates.xml file itself.
==Automates==
{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"
|+AnimationPaths Table
! scope="col" style="background: #efefef;" | Name
! scope="col" style="background: #efefef;" | Type
! scope="col" style="background: #efefef;" | Default
! scope="col" style="background: #efefef;" | Notes/Reference
|-
| ID || integer|| || Primary Key,Autoincrement
|-
| Type || text|| || 
|-
| Description || text|| || 
|-
| Help || text|| || 
|-
| DisabledHelp || text|| || 
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
| Visible || boolean|| false|| 
|-
| ConfirmCommand || boolean|| false|| 
|-
| Automate || text|| || 
|-
| Command || text|| || 
|-
| IconIndex || integer|| -1|| 
|-
| IconAtlas || text|| NULL|| IconTextureAtlases(Atlas)
|}
{{Civ5_XML_Files}}