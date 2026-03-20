=Civ5Controls.xml=
*The Civ5Controls.xml file contains definitions for the Controls.
*This information is taken from the Civ5Controls.xml file itself.
==Controls==
{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"
|+Controls Table
! scope="col" style="background: #efefef;" | Name
! scope="col" style="background: #efefef;" | Type
! scope="col" style="background: #efefef;" | Default
! scope="col" style="background: #efefef;" | Notes
|-
| ID || integer|| || Primary Key,Autoincrement
|-
| Type || text||[[ControlTypes|Controls(Types)]] || Not Null,Unique
|-
| Description || text|| || 
|-
| Help || text|| || 
|-
| DisabledHelp || text|| || 
|-
| Button || text|| || 
|-
| HotKey || text|| || 
|-
| HotKeyAlt || text|| || 
|-
| HotKeyPriority || integer|| 0|| 
|-
| HotKeyPriorityAlt || integer|| 0|| 
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
|}
{{Civ5_XML_Files}}