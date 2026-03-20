{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|ID.png|The <code>FlavorType</code> pseudo-type is actually a regular '''integer'''. Pseudo-types do not exist in Lua, they only serve a documentation purpose on the wiki!
* {{DB}} Integers labeled as <code>FlavorType</code> corresponds to the ''ID'' column of the {{Table5|Flavors|CIV5Flavors}} XML table.
}}


= XML: the Flavors table =
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
|FLAVOR_OFFENSE
|-
|align="right"|1
|
|FLAVOR_DEFENSE
|-
|align="right"|2
|
|FLAVOR_CITY_DEFENSE
|-
|align="right"|3
|
|FLAVOR_MILITARY_TRAINING
|-
|align="right"|4
|
|FLAVOR_RECON
|-
|align="right"|5
|
|FLAVOR_RANGED
|-
|align="right"|6
|
|FLAVOR_MOBILE
|-
|align="right"|7
|
|FLAVOR_NAVAL
|-
|align="right"|8
|
|FLAVOR_NAVAL_RECON
|-
|align="right"|9
|
|FLAVOR_NAVAL_GROWTH
|-
|align="right"|10
|
|FLAVOR_NAVAL_TILE_IMPROVEMENT
|-
|align="right"|11
|
|FLAVOR_AIR
|-
|align="right"|12
|
|FLAVOR_EXPANSION
|-
|align="right"|13
|
|FLAVOR_GROWTH
|-
|align="right"|14
|
|FLAVOR_TILE_IMPROVEMENT
|-
|align="right"|15
|
|FLAVOR_INFRASTRUCTURE
|-
|align="right"|16
|
|FLAVOR_PRODUCTION
|-
|align="right"|17
|
|FLAVOR_GOLD
|-
|align="right"|18
|
|FLAVOR_SCIENCE
|-
|align="right"|19
|
|FLAVOR_CULTURE
|-
|align="right"|20
|
|FLAVOR_HAPPINESS
|-
|align="right"|21
|
|FLAVOR_GREAT_PEOPLE
|-
|align="right"|22
|
|FLAVOR_WONDER
|-
|align="right"|23
|
|FLAVOR_RELIGION
|-
|align="right"|24
|
|FLAVOR_DIPLOMACY
|-
|align="right"|25
|
|FLAVOR_SPACESHIP
|-
|align="right"|26
|
|FLAVOR_WATER_CONNECTION
|-
|align="right"|27
|
|FLAVOR_NUKE
|-
|align="right"|28
|
|FLAVOR_ANTIAIR
|-
|align="right"|29
|
|FLAVOR_USE_NUKE
|-
|align="right"|30
|
|FLAVOR_ESPIONAGE
|-
|align="right"|31
|
|FLAVOR_AIR_CARRIER
|}</code>


= Examples =


=Used by=
{|cellspacing="4" cellpadding="0" width="100%" style="background-color:#F0F0F0"
<!-- 
FLAVORVALUE
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Unit}}:{{Func5|Unit|FlavorValue}}<b>(</b>{{Type5|FlavorType}} flavor<b>)</b></code>
|}




{{Civ5 API Footer}}
[[Category:Civ5 Types|FlavorType]]