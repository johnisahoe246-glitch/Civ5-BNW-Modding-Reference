=Civ5Commands.xml=
*The Civ5Commands.xml file contains definitions for the Commands.
*This information is taken from the Civ5Commands.xml file itself.
==Commands==
{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"
|+Commands Table
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
| All || boolean|| false|| 
|-
| ConfirmCommand || boolean|| false|| 
|-
| Automate || text|| || 
|}
{{Civ5_XML_Files}}