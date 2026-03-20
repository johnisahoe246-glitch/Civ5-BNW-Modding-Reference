{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|ID.png|The <code>UnitAIType</code> pseudo-type is actually a regular '''integer'''. Pseudo-types do not exist in Lua, they only serve a documentation purpose on the wiki!
* {{DB}} Integers labeled as <code>UnitAIType</code> corresponds to the ''ID'' column of the {{Table5|UnitAIInfos|CIV5UnitAIInfos}} XML table.
}}


= XML: the UnitAIInfos table =
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
|UNITAI_UNKNOWN
|-
|align="right"|1
|
|UNITAI_SETTLE
|-
|align="right"|2
|
|UNITAI_WORKER
|-
|align="right"|3
|
|UNITAI_ATTACK
|-
|align="right"|4
|
|UNITAI_CITY_BOMBARD
|-
|align="right"|5
|
|UNITAI_FAST_ATTACK
|-
|align="right"|6
|
|UNITAI_DEFENSE
|-
|align="right"|7
|
|UNITAI_COUNTER
|-
|align="right"|8
|
|UNITAI_RANGED
|-
|align="right"|9
|
|UNITAI_CITY_SPECIAL
|-
|align="right"|10
|
|UNITAI_EXPLORE
|-
|align="right"|11
|
|UNITAI_ARTIST
|-
|align="right"|12
|
|UNITAI_SCIENTIST
|-
|align="right"|13
|
|UNITAI_GENERAL
|-
|align="right"|14
|
|UNITAI_MERCHANT
|-
|align="right"|15
|
|UNITAI_ENGINEER
|-
|align="right"|16
|
|UNITAI_ICBM
|-
|align="right"|17
|
|UNITAI_WORKER_SEA
|-
|align="right"|18
|
|UNITAI_ATTACK_SEA
|-
|align="right"|19
|
|UNITAI_RESERVE_SEA
|-
|align="right"|20
|
|UNITAI_ESCORT_SEA
|-
|align="right"|21
|
|UNITAI_EXPLORE_SEA
|-
|align="right"|22
|
|UNITAI_ASSAULT_SEA
|-
|align="right"|23
|
|UNITAI_SETTLER_SEA
|-
|align="right"|24
|
|UNITAI_CARRIER_SEA
|-
|align="right"|25
|
|UNITAI_MISSILE_CARRIER_SEA
|-
|align="right"|26
|
|UNITAI_PIRATE_SEA
|-
|align="right"|27
|
|UNITAI_ATTACK_AIR
|-
|align="right"|28
|
|UNITAI_DEFENSE_AIR
|-
|align="right"|29
|
|UNITAI_CARRIER_AIR
|-
|align="right"|30
|
|UNITAI_MISSILE_AIR
|-
|align="right"|31
|
|UNITAI_PARADROP
|-
|align="right"|32
|
|UNITAI_SPACESHIP_PART
|-
|align="right"|33
|
|UNITAI_TREASURE
|-
|align="right"|34
|
|UNITAI_PROPHET
|-
|align="right"|35
|
|UNITAI_MISSIONARY
|-
|align="right"|36
|
|UNITAI_INQUISITOR
|-
|align="right"|37
|
|UNITAI_ADMIRAL
|}</code>


= Examples =


=Used by=
{|cellspacing="4" cellpadding="0" width="100%" style="background-color:#F0F0F0"
<!-- 
GETNUMTRAINUNITAI
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|City}}:{{Func5|City|GetNumTrainUnitAI}}<b>(</b>{{Type5|UnitAIType}} unitAI<b>)</b></code>
<!-- 
GETPRODUCTIONUNITAI
-->
|-
|align="right" width="200" |<code>{{Type5|UnitAIType}}</code>
|style="padding-left:6px" |<code>{{Type5|City}}:{{Func5|City|GetProductionUnitAI}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ADDFREEUNIT
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|AddFreeUnit}}<b>(</b>{{Type5|UnitType}} arg0, {{Type5|UnitAIType}} UNITAI_DEFENSE<b>)</b></code>
<!-- 
INITUNIT
-->
|-
|align="right" width="200" |<code>{{Type5|Unit}}</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|InitUnit}}<b>(</b>{{Type5|UnitType}} unit, {{Type5|ResourceType}} x, {{Type5|ResourceType}} y, {{Type5|UnitAIType}} unitAI = NO_UNITAI, {{Type5|DirectionType}} facingDirection = NO_DIRECTION<b>)</b></code>
<!-- 
GETUNITAICARGO
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Unit}}:{{Func5|Unit|GetUnitAICargo}}<b>(</b>{{Type5|UnitAIType}} unitAI<b>)</b></code>
<!-- 
GETUNITAITYPE
-->
|-
|align="right" width="200" |<code>{{Type5|UnitAIType}}</code>
|style="padding-left:6px" |<code>{{Type5|Unit}}:{{Func5|Unit|GetUnitAIType}}<b>(</b><!-- No arguments --><b>)</b></code>
|}




{{Civ5 API Footer}}
[[Category:Civ5 Types|UnitAIType]]