{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|ID.png|The <code>UnitClassType</code> pseudo-type is actually a regular '''integer'''. Pseudo-types do not exist in Lua, they only serve a documentation purpose on the wiki!
* {{DB}} Integers labeled as <code>UnitClassType</code> corresponds to the ''ID'' column of the {{Table5|UnitClasses|CIV5UnitClasses}} XML table.
}}


= XML: the UnitClasses table =
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
|UNITCLASS_SETTLER
|-
|align="right"|0
|
|UNITCLASS_PROPHET
|-
|align="right"|1
|
|UNITCLASS_WORKER
|-
|align="right"|1
|
|UNITCLASS_MISSIONARY
|-
|align="right"|2
|
|UNITCLASS_WARRIOR
|-
|align="right"|2
|
|UNITCLASS_COMPOSITE_BOWMAN
|-
|align="right"|3
|
|UNITCLASS_SCOUT
|-
|align="right"|3
|
|UNITCLASS_GATLINGGUN
|-
|align="right"|4
|
|UNITCLASS_ARCHER
|-
|align="right"|4
|
|UNITCLASS_GALLEASS
|-
|align="right"|5
|
|UNITCLASS_SPEARMAN
|-
|align="right"|5
|
|UNITCLASS_GREAT_WAR_INFANTRY
|-
|align="right"|6
|
|UNITCLASS_CHARIOT_ARCHER
|-
|align="right"|6
|
|UNITCLASS_MARINE
|-
|align="right"|7
|
|UNITCLASS_SWORDSMAN
|-
|align="right"|7
|
|UNITCLASS_TRIPLANE
|-
|align="right"|8
|
|UNITCLASS_HORSEMAN
|-
|align="right"|8
|
|UNITCLASS_WWI_BOMBER
|-
|align="right"|9
|
|UNITCLASS_CATAPULT
|-
|align="right"|9
|
|UNITCLASS_WWI_TANK
|-
|align="right"|10
|
|UNITCLASS_KNIGHT
|-
|align="right"|10
|
|UNITCLASS_MACHINE_GUN
|-
|align="right"|11
|
|UNITCLASS_CROSSBOWMAN
|-
|align="right"|11
|
|UNITCLASS_PRIVATEER
|-
|align="right"|12
|
|UNITCLASS_PIKEMAN
|-
|align="right"|12
|
|UNITCLASS_INQUISITOR
|-
|align="right"|13
|
|UNITCLASS_TREBUCHET
|-
|align="right"|13
|
|UNITCLASS_GREAT_ADMIRAL
|-
|align="right"|14
|
|UNITCLASS_LONGSWORDSMAN
|-
|align="right"|15
|
|UNITCLASS_MUSKETMAN
|-
|align="right"|16
|
|UNITCLASS_CANNON
|-
|align="right"|17
|
|UNITCLASS_LANCER
|-
|align="right"|18
|
|UNITCLASS_RIFLEMAN
|-
|align="right"|19
|
|UNITCLASS_CAVALRY
|-
|align="right"|20
|
|UNITCLASS_INFANTRY
|-
|align="right"|21
|
|UNITCLASS_ARTILLERY
|-
|align="right"|22
|
|UNITCLASS_TANK
|-
|align="right"|23
|
|UNITCLASS_ANTI_TANK_GUN
|-
|align="right"|24
|
|UNITCLASS_ANTI_AIRCRAFT_GUN
|-
|align="right"|25
|
|UNITCLASS_PARATROOPER
|-
|align="right"|26
|
|UNITCLASS_FIGHTER
|-
|align="right"|27
|
|UNITCLASS_BOMBER
|-
|align="right"|28
|
|UNITCLASS_ATOMIC_BOMB
|-
|align="right"|29
|
|UNITCLASS_ROCKET_ARTILLERY
|-
|align="right"|30
|
|UNITCLASS_MECHANIZED_INFANTRY
|-
|align="right"|31
|
|UNITCLASS_MODERN_ARMOR
|-
|align="right"|32
|
|UNITCLASS_HELICOPTER_GUNSHIP
|-
|align="right"|33
|
|UNITCLASS_MOBILE_SAM
|-
|align="right"|34
|
|UNITCLASS_GUIDED_MISSILE
|-
|align="right"|35
|
|UNITCLASS_JET_FIGHTER
|-
|align="right"|36
|
|UNITCLASS_STEALTH_BOMBER
|-
|align="right"|37
|
|UNITCLASS_NUCLEAR_MISSILE
|-
|align="right"|38
|
|UNITCLASS_MECH
|-
|align="right"|39
|
|UNITCLASS_WORKBOAT
|-
|align="right"|40
|
|UNITCLASS_GALLEY
|-
|align="right"|41
|
|UNITCLASS_TRIREME
|-
|align="right"|42
|
|UNITCLASS_CARAVEL
|-
|align="right"|43
|
|UNITCLASS_FRIGATE
|-
|align="right"|44
|
|UNITCLASS_IRONCLAD
|-
|align="right"|45
|
|UNITCLASS_DESTROYER
|-
|align="right"|46
|
|UNITCLASS_BATTLESHIP
|-
|align="right"|47
|
|UNITCLASS_SUBMARINE
|-
|align="right"|48
|
|UNITCLASS_CARRIER
|-
|align="right"|49
|
|UNITCLASS_NUCLEAR_SUBMARINE
|-
|align="right"|50
|
|UNITCLASS_MISSILE_CRUISER
|-
|align="right"|51
|
|UNITCLASS_ARTIST
|-
|align="right"|52
|
|UNITCLASS_SCIENTIST
|-
|align="right"|53
|
|UNITCLASS_MERCHANT
|-
|align="right"|54
|
|UNITCLASS_ENGINEER
|-
|align="right"|55
|
|UNITCLASS_GREAT_GENERAL
|-
|align="right"|56
|
|UNITCLASS_SS_COCKPIT
|-
|align="right"|57
|
|UNITCLASS_SS_STASIS_CHAMBER
|-
|align="right"|58
|
|UNITCLASS_SS_ENGINE
|-
|align="right"|59
|
|UNITCLASS_SS_BOOSTER
|}</code>


= Examples =
Here are different ways to query the database to retrieve the ''ID'' from the ''type''. Those examples will return and assign the integer value 0. See also {{Type5|GameInfo}}.
<syntaxhighlight lang="lua" class="civ5-example">
local id = GameInfo.UnitClasses.UNITCLASS_PROPHET.ID
local id = GameInfo["UnitClasses"].["UNITCLASS_PROPHET"].ID
local id = GameInfo.UnitClasses{Type="UNITCLASS_PROPHET"}().ID
</syntaxhighlight>
Alternatively you could use the ''ID'' or the ''type'' to retrieve the value of the ''Description'' column. Those examples will return and assign the value TXT_KEY_UNIT_PROPHET.
<syntaxhighlight lang="lua" class="civ5-example">
local description = GameInfo.UnitClasses[0].Description
local description = GameInfo["UnitClasses"][0]["Description"]
local description = GameInfo.UnitClasses{ID=0}().Description
</syntaxhighlight>


=Used by=
{|cellspacing="4" cellpadding="0" width="100%" style="background-color:#F0F0F0"
<!-- 
GETUNITCLASSCREATEDCOUNT
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Game}}.{{Func5|Game|GetUnitClassCreatedCount}}<b>(</b>{{Type5|UnitClassType}} index<b>)</b></code>
<!-- 
ISUNITCLASSMAXEDOUT
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|Game}}.{{Func5|Game|IsUnitClassMaxedOut}}<b>(</b>{{Type5|UnitClassType}} index, '''int''' extra<b>)</b></code>
<!-- 
GETUNITCLASSCOUNT
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|GetUnitClassCount}}<b>(</b>{{Type5|UnitClassType}} index<b>)</b></code>
<!-- 
GETUNITCLASSCOUNTPLUSMAKING
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|GetUnitClassCountPlusMaking}}<b>(</b>{{Type5|UnitClassType}} index<b>)</b></code>
<!-- 
GETUNITCLASSMAKING
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|GetUnitClassMaking}}<b>(</b>{{Type5|UnitClassType}} index<b>)</b></code>
<!-- 
ISPRODUCTIONMAXEDUNITCLASS
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|IsProductionMaxedUnitClass}}<b>(</b>{{Type5|UnitClassType}} unitClass<b>)</b></code>
<!-- 
ISUNITCLASSMAXEDOUT
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|IsUnitClassMaxedOut}}<b>(</b>{{Type5|UnitClassType}} index, '''int''' extra<b>)</b></code>
<!-- 
GETUNITCLASSCOUNT
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Team}}:{{Func5|Team|GetUnitClassCount}}<b>(</b>{{Type5|UnitClassType}} index<b>)</b></code>
<!-- 
GETUNITCLASSCOUNTPLUSMAKING
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Team}}:{{Func5|Team|GetUnitClassCountPlusMaking}}<b>(</b>{{Type5|UnitClassType}} unitClass<b>)</b></code>
<!-- 
GETUNITCLASSMAKING
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Team}}:{{Func5|Team|GetUnitClassMaking}}<b>(</b>{{Type5|UnitClassType}} unitClass<b>)</b></code>
<!-- 
ISUNITCLASSMAXEDOUT
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|Team}}:{{Func5|Team|IsUnitClassMaxedOut}}<b>(</b>{{Type5|UnitClassType}} index, '''int''' extra<b>)</b></code>
<!-- 
GETUNITCLASSMODIFIER
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Unit}}:{{Func5|Unit|GetUnitClassModifier}}<b>(</b>{{Type5|UnitClassType}} index<b>)</b></code>
<!-- 
GETUNITCLASSTYPE
-->
|-
|align="right" width="200" |<code>{{Type5|UnitClassType}}</code>
|style="padding-left:6px" |<code>{{Type5|Unit}}:{{Func5|Unit|GetUnitClassType}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
UNITCLASSATTACKMODIFIER
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Unit}}:{{Func5|Unit|UnitClassAttackModifier}}<b>(</b>{{Type5|UnitClassType}} unitClass<b>)</b></code>
<!-- 
UNITCLASSDEFENSEMODIFIER
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Unit}}:{{Func5|Unit|UnitClassDefenseModifier}}<b>(</b>{{Type5|UnitClassType}} unitClass<b>)</b></code>
|}




{{Civ5 API Footer}}
[[Category:Civ5 Types|UnitClassType]]