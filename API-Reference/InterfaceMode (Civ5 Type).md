{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|ID.png|The <code>InterfaceMode</code> pseudo-type is actually a regular '''integer'''. Pseudo-types do not exist in Lua, they only serve a documentation purpose on the wiki!
* {{DB}} Integers labeled as <code>InterfaceMode</code> corresponds to the ''ID'' column of the {{Table5|InterfaceModes|CIV5InterfaceModes}} XML table.
* {{Lua}} The standard (unmodded) values in the ''ID'' and ''Type'' columns are also stored in the '''InterfaceModeTypes''' Lua enumeration.
}}


= Lua: the InterfaceModeTypes enumeration =
Firaxis provides a Lua enumeration named <code>InterfaceModeTypes</code>. This is just a regular global table. Its keys are the constants' names and the pairs the corresponding values.
* This specific enumeration contains data from the {{Table5|InterfaceModes|CIV5InterfaceModes}} data table.<br/>
* They are stored as key/value pairs: the keys are the strings from the ''Type'' column and the values are the integers from the ''ID'' column.<br/>
{{Warning}} Be careful: this enumeration do '''not''' reflect the changes, additions and deletions made by mods. As a result it is advised to rely on {{Type5|GameInfo}} instead.<br/>

<br/>Below are the values found in this enumeration.
<code>
{|
|-
!align="left" |Key
!
!align="left" |Value 
|-
|align="left" |"NO_INTERFACEMODE"
|
|align="right" |-1
|-
|align="left" |"INTERFACEMODE_DEBUG"
|
|align="right" |0
|-
|align="left" |"INTERFACEMODE_SELECTION"
|
|align="right" |1
|-
|align="left" |"INTERFACEMODE_PING"
|
|align="right" |2
|-
|align="left" |"INTERFACEMODE_MOVE_TO"
|
|align="right" |3
|-
|align="left" |"INTERFACEMODE_MOVE_TO_TYPE"
|
|align="right" |4
|-
|align="left" |"INTERFACEMODE_MOVE_TO_ALL"
|
|align="right" |5
|-
|align="left" |"INTERFACEMODE_ROUTE_TO"
|
|align="right" |6
|-
|align="left" |"INTERFACEMODE_AIRLIFT"
|
|align="right" |7
|-
|align="left" |"INTERFACEMODE_NUKE"
|
|align="right" |8
|-
|align="left" |"INTERFACEMODE_PARADROP"
|
|align="right" |9
|-
|align="left" |"INTERFACEMODE_ATTACK"
|
|align="right" |10
|-
|align="left" |"INTERFACEMODE_RANGE_ATTACK"
|
|align="right" |11
|-
|align="left" |"INTERFACEMODE_AIRSTRIKE"
|
|align="right" |12
|-
|align="left" |"INTERFACEMODE_AIR_SWEEP"
|
|align="right" |13
|-
|align="left" |"INTERFACEMODE_REBASE"
|
|align="right" |14
|-
|align="left" |"INTERFACEMODE_PLACE_UNIT"
|
|align="right" |15
|-
|align="left" |"INTERFACEMODE_EMBARK"
|
|align="right" |16
|-
|align="left" |"INTERFACEMODE_DISEMBARK"
|
|align="right" |17
|-
|align="left" |"INTERFACEMODE_GIFT_UNIT"
|
|align="right" |18
|-
|align="left" |"INTERFACEMODE_CITY_PLOT_SELECTION"
|
|align="right" |19
|-
|align="left" |"INTERFACEMODE_PURCHASE_PLOT"
|
|align="right" |20
|-
|align="left" |"INTERFACEMODE_CITY_RANGE_ATTACK"
|
|align="right" |21
|-
|align="left" |"INTERFACEMODE_GIFT_TILE_IMPROVEMENT"
|
|align="right" |22
|-
|align="left" |"NUM_INTERFACEMODE_TYPES"
|
|align="right" |23
|}</code>


= XML: the InterfaceModes table =
Here are the ''ID'' and ''Type'' columns found in this table.
<code>
{|
|-
!align="left" |ID
!
!align="left" |Type
|-
|align="right"|0
|
|INTERFACEMODE_DEBUG
|-
|align="right"|0
|
|INTERFACEMODE_GIFT_TILE_IMPROVEMENT
|-
|align="right"|1
|
|INTERFACEMODE_SELECTION
|-
|align="right"|2
|
|INTERFACEMODE_PING
|-
|align="right"|3
|
|INTERFACEMODE_MOVE_TO
|-
|align="right"|4
|
|INTERFACEMODE_MOVE_TO_TYPE
|-
|align="right"|5
|
|INTERFACEMODE_MOVE_TO_ALL
|-
|align="right"|6
|
|INTERFACEMODE_ROUTE_TO
|-
|align="right"|7
|
|INTERFACEMODE_AIRLIFT
|-
|align="right"|8
|
|INTERFACEMODE_NUKE
|-
|align="right"|9
|
|INTERFACEMODE_PARADROP
|-
|align="right"|10
|
|INTERFACEMODE_ATTACK
|-
|align="right"|11
|
|INTERFACEMODE_RANGE_ATTACK
|-
|align="right"|12
|
|INTERFACEMODE_AIRSTRIKE
|-
|align="right"|13
|
|INTERFACEMODE_AIR_SWEEP
|-
|align="right"|14
|
|INTERFACEMODE_REBASE
|-
|align="right"|15
|
|INTERFACEMODE_PLACE_UNIT
|-
|align="right"|16
|
|INTERFACEMODE_EMBARK
|-
|align="right"|17
|
|INTERFACEMODE_DISEMBARK
|-
|align="right"|18
|
|INTERFACEMODE_GIFT_UNIT
|-
|align="right"|19
|
|INTERFACEMODE_CITY_PLOT_SELECTION
|-
|align="right"|20
|
|INTERFACEMODE_PURCHASE_PLOT
|-
|align="right"|21
|
|INTERFACEMODE_CITY_RANGE_ATTACK
|}</code>


= Examples =
Here is how to use the LUA enumeration to retrieve the ''ID'' from the ''type''. Those examples will return and assign the integer value 0.
<syntaxhighlight lang="lua" class="civ5-example">
local id = InterfaceModeTypes.INTERFACEMODE_DEBUG
local id = InterfaceModeTypes["INTERFACEMODE_DEBUG"]
</syntaxhighlight>
Here are different ways to query the database to retrieve the ''ID'' from the ''type''. Those examples will return and assign the integer value 0. See also {{Type5|GameInfo}}.
<syntaxhighlight lang="lua" class="civ5-example">
local id = GameInfo.InterfaceModes.INTERFACEMODE_GIFT_TILE_IMPROVEMENT.ID
local id = GameInfo["InterfaceModes"].["INTERFACEMODE_GIFT_TILE_IMPROVEMENT"].ID
local id = GameInfo.InterfaceModes{Type="INTERFACEMODE_GIFT_TILE_IMPROVEMENT"}().ID
</syntaxhighlight>
Alternatively you could use the ''ID'' or the ''type'' to retrieve the value of the ''Description'' column. Those examples will return and assign the value TXT_KEY_INTERFACEMODE_GIFT_TILE_IMPROVEMENT.
<syntaxhighlight lang="lua" class="civ5-example">
local description = GameInfo.InterfaceModes[0].Description
local description = GameInfo["InterfaceModes"][0]["Description"]
local description = GameInfo.InterfaceModes{ID=0}().Description
</syntaxhighlight>


=Used by=
{|cellspacing="4" cellpadding="0" width="100%" style="background-color:#F0F0F0"
<!-- 
INTERFACEMODECHANGED
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Events}}.{{Func5|Events|InterfaceModeChanged}}<b>(</b>{{Type5|InterfaceMode}} oldInterfaceMode, {{Type5|InterfaceMode}} newInterfaceMode<b>)</b></code>
<!-- 
CANDOINTERFACEMODE
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|UI}}.{{Func5|UI|CanDoInterfaceMode}}<b>(</b>{{Type5|InterfaceMode}} interfaceMode<b>)</b></code>
<!-- 
GETINTERFACEMODE
-->
|-
|align="right" width="200" |<code>{{Type5|InterfaceMode}}</code>
|style="padding-left:6px" |<code>{{Type5|UI}}.{{Func5|UI|GetInterfaceMode}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
SETINTERFACEMODE
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|UI}}.{{Func5|UI|SetInterfaceMode}}<b>(</b>{{Type5|InterfaceMode}} interfaceModeSelection<b>)</b></code>
|}




{{Civ5 API Footer}}
[[Category:Civ5 Types|InterfaceMode]]