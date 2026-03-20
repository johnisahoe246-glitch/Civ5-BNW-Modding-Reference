=CIV5InterfaceModes.xml=
*The CIV5InterfaceModes.xml file contains definitions for the InterfaceModes.
*This information is taken from the CIV5InterfaceModes.xml file itself.
==InterfaceModes==
{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"
|+InterfaceModes Table
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
| CursorType || text|| || 
|-
| Mission || text|| || 
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
| GotoPlot || boolean|| false|| 
|-
| HighlightPlot || boolean|| false|| 
|-
| SelectType || boolean|| false|| 
|-
| SelectAll || boolean|| false|| 
|}
{{Civ5_XML_Files}}