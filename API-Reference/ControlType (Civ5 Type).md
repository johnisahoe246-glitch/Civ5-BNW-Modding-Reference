{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|ID.png|The <code>ControlType</code> pseudo-type is actually a regular '''integer'''. Pseudo-types do not exist in Lua, they only serve a documentation purpose on the wiki!
* {{Lua}} Integers labeled as <code>ControlType</code> corresponds to the constants defined in the '''ControlTypes''' Lua enumeration.
}}


= Lua: the ControlTypes enumeration =
Firaxis provides a Lua enumeration named <code>ControlTypes</code>. This is just a regular global table. Its keys are the constants' names and the pairs the corresponding values.

<br/>Below are the values found in this enumeration.
<code>
{|
|-
!align="left" |Key
!
!align="left" |Value 
|-
|align="left" |"NO_CONTROL"
|
|align="right" |-1
|-
|align="left" |"CONTROL_CENTERONSELECTION"
|
|align="right" |0
|-
|align="left" |"CONTROL_SELECTYUNITTYPE"
|
|align="right" |1
|-
|align="left" |"CONTROL_SELECTYUNITALL"
|
|align="right" |2
|-
|align="left" |"CONTROL_SELECTCITY"
|
|align="right" |3
|-
|align="left" |"CONTROL_SELECTCAPITAL"
|
|align="right" |4
|-
|align="left" |"CONTROL_NEXTCITY"
|
|align="right" |5
|-
|align="left" |"CONTROL_PREVCITY"
|
|align="right" |6
|-
|align="left" |"CONTROL_NEXTUNIT"
|
|align="right" |7
|-
|align="left" |"CONTROL_PREVUNIT"
|
|align="right" |8
|-
|align="left" |"CONTROL_CYCLEUNIT"
|
|align="right" |9
|-
|align="left" |"CONTROL_CYCLEUNIT_ALT"
|
|align="right" |10
|-
|align="left" |"CONTROL_CYCLEWORKER"
|
|align="right" |11
|-
|align="left" |"CONTROL_LASTUNIT"
|
|align="right" |12
|-
|align="left" |"CONTROL_ENDTURN"
|
|align="right" |13
|-
|align="left" |"CONTROL_ENDTURN_ALT"
|
|align="right" |14
|-
|align="left" |"CONTROL_FORCEENDTURN"
|
|align="right" |15
|-
|align="left" |"CONTROL_AUTOMOVES"
|
|align="right" |16
|-
|align="left" |"CONTROL_PING"
|
|align="right" |17
|-
|align="left" |"CONTROL_YIELDS"
|
|align="right" |18
|-
|align="left" |"CONTROL_RESOURCE_ALL"
|
|align="right" |19
|-
|align="left" |"CONTROL_UNIT_ICONS"
|
|align="right" |20
|-
|align="left" |"CONTROL_SCORES"
|
|align="right" |21
|-
|align="left" |"CONTROL_LOAD_GAME"
|
|align="right" |22
|-
|align="left" |"CONTROL_OPTIONS_SCREEN"
|
|align="right" |23
|-
|align="left" |"CONTROL_RETIRE"
|
|align="right" |24
|-
|align="left" |"CONTROL_SAVE_GROUP"
|
|align="right" |25
|-
|align="left" |"CONTROL_SAVE_NORMAL"
|
|align="right" |26
|-
|align="left" |"CONTROL_QUICK_SAVE"
|
|align="right" |27
|-
|align="left" |"CONTROL_QUICK_LOAD"
|
|align="right" |28
|-
|align="left" |"CONTROL_CIVILOPEDIA"
|
|align="right" |29
|-
|align="left" |"CONTROL_POLICIES_SCREEN"
|
|align="right" |30
|-
|align="left" |"CONTROL_FOREIGN_SCREEN"
|
|align="right" |31
|-
|align="left" |"CONTROL_MILITARY_SCREEN"
|
|align="right" |32
|-
|align="left" |"CONTROL_TECH_CHOOSER"
|
|align="right" |33
|-
|align="left" |"CONTROL_TURN_LOG"
|
|align="right" |34
|-
|align="left" |"CONTROL_DOMESTIC_SCREEN"
|
|align="right" |35
|-
|align="left" |"CONTROL_VICTORY_SCREEN"
|
|align="right" |36
|-
|align="left" |"CONTROL_INFO"
|
|align="right" |37
|-
|align="left" |"CONTROL_SELECT_HEALTHY"
|
|align="right" |38
|-
|align="left" |"CONTROL_TOGGLE_STRATEGIC_VIEW"
|
|align="right" |39
|-
|align="left" |"CONTROL_ADVISOR_COUNSEL"
|
|align="right" |40
|-
|align="left" |"CONTROL_ESPIONAGE_OVERVIEW"
|
|align="right" |41
|-
|align="left" |"CONTROL_RELIGION_OVERVIEW"
|
|align="right" |42
|}</code>


= Examples =
Here is how to use the LUA enumeration to retrieve the ''ID'' from the ''type''. Those examples will return and assign the integer value 0.
<syntaxhighlight lang="lua" class="civ5-example">
local id = ControlTypes.CONTROL_CENTERONSELECTION
local id = ControlTypes["CONTROL_CENTERONSELECTION"]
</syntaxhighlight>


=Used by=
{|cellspacing="4" cellpadding="0" width="100%" style="background-color:#F0F0F0"
<!-- 
CANDOCONTROL
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Game}}.{{Func5|Game|CanDoControl}}<b>(</b>{{Type5|ControlType}} arg0<b>)</b></code>
<!-- 
DOCONTROL
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Game}}.{{Func5|Game|DoControl}}<b>(</b>{{Type5|ControlType}} control<b>)</b></code>
|}




{{Civ5 API Footer}}
[[Category:Civ5 Types|ControlType]]