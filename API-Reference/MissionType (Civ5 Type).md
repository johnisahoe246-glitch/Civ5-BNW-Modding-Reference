{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|ID.png|The <code>MissionType</code> pseudo-type is actually a regular '''integer'''. Pseudo-types do not exist in Lua, they only serve a documentation purpose on the wiki!
* {{DB}} Integers labeled as <code>MissionType</code> corresponds to the ''ID'' column of the {{Table5|Missions|CIV5Missions}} XML table.
* {{Lua}} The standard (unmodded) values in the ''ID'' and ''Type'' columns are also stored in the '''MissionTypes''' Lua enumeration.
}}


= Lua: the MissionTypes enumeration =
Firaxis provides a Lua enumeration named <code>MissionTypes</code>. This is just a regular global table. Its keys are the constants' names and the pairs the corresponding values.
* This specific enumeration contains data from the {{Table5|Missions|CIV5Missions}} data table.<br/>
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
|align="right" |0
|
|align="left" |"MISSION_MOVE_TO"
|-
|align="right" |1
|
|align="left" |"MISSION_ROUTE_TO"
|-
|align="right" |2
|
|align="left" |"MISSION_MOVE_TO_UNIT"
|-
|align="right" |3
|
|align="left" |"MISSION_SWAP_UNITS"
|-
|align="right" |4
|
|align="left" |"MISSION_SKIP"
|-
|align="right" |5
|
|align="left" |"MISSION_SLEEP"
|-
|align="right" |6
|
|align="left" |"MISSION_ALERT"
|-
|align="right" |7
|
|align="left" |"MISSION_FORTIFY"
|-
|align="right" |8
|
|align="left" |"MISSION_GARRISON"
|-
|align="right" |9
|
|align="left" |"MISSION_SET_UP_FOR_RANGED_ATTACK"
|-
|align="right" |10
|
|align="left" |"MISSION_EMBARK"
|-
|align="right" |11
|
|align="left" |"MISSION_DISEMBARK"
|-
|align="right" |12
|
|align="left" |"MISSION_AIRPATROL"
|-
|align="right" |13
|
|align="left" |"MISSION_HEAL"
|-
|align="right" |14
|
|align="left" |"MISSION_AIRLIFT"
|-
|align="right" |15
|
|align="left" |"MISSION_NUKE"
|-
|align="right" |16
|
|align="left" |"MISSION_PARADROP"
|-
|align="right" |17
|
|align="left" |"MISSION_AIR_SWEEP"
|-
|align="right" |18
|
|align="left" |"MISSION_REBASE"
|-
|align="right" |19
|
|align="left" |"MISSION_RANGE_ATTACK"
|-
|align="right" |20
|
|align="left" |"MISSION_PILLAGE"
|-
|align="right" |21
|
|align="left" |"MISSION_FOUND"
|-
|align="right" |22
|
|align="left" |"MISSION_JOIN"
|-
|align="right" |23
|
|align="left" |"MISSION_CONSTRUCT"
|-
|align="right" |24
|
|align="left" |"MISSION_DISCOVER"
|-
|align="right" |25
|
|align="left" |"MISSION_HURRY"
|-
|align="right" |26
|
|align="left" |"MISSION_TRADE"
|-
|align="right" |27
|
|align="left" |"MISSION_REPAIR_FLEET"
|-
|align="right" |28
|
|align="left" |"MISSION_SPACESHIP"
|-
|align="right" |29
|
|align="left" |"MISSION_CULTURE_BOMB"
|-
|align="right" |30
|
|align="left" |"MISSION_FOUND_RELIGION"
|-
|align="right" |31
|
|align="left" |"MISSION_GOLDEN_AGE"
|-
|align="right" |32
|
|align="left" |"MISSION_BUILD"
|-
|align="right" |33
|
|align="left" |"MISSION_LEAD"
|-
|align="right" |34
|
|align="left" |"MISSION_DIE_ANIMATION"
|-
|align="right" |35
|
|align="left" |"MISSION_BEGIN_COMBAT"
|-
|align="right" |36
|
|align="left" |"MISSION_END_COMBAT"
|-
|align="right" |37
|
|align="left" |"MISSION_AIRSTRIKE"
|-
|align="right" |38
|
|align="left" |"MISSION_SURRENDER"
|-
|align="right" |39
|
|align="left" |"MISSION_CAPTURED"
|-
|align="right" |40
|
|align="left" |"MISSION_IDLE"
|-
|align="right" |41
|
|align="left" |"MISSION_DIE"
|-
|align="right" |42
|
|align="left" |"MISSION_DAMAGE"
|-
|align="right" |43
|
|align="left" |"MISSION_MULTI_SELECT"
|-
|align="right" |44
|
|align="left" |"MISSION_MULTI_DESELECT"
|-
|align="right" |45
|
|align="left" |"MISSION_WAIT_FOR"
|-
|align="right" |46
|
|align="left" |"MISSION_SPREAD_RELIGION"
|-
|align="right" |47
|
|align="left" |"MISSION_ENHANCE_RELIGION"
|-
|align="right" |48
|
|align="left" |"MISSION_REMOVE_HERESY"
|-
|align="left" |"NO_MISSION"
|
|align="right" |-1
|-
|align="left" |"MISSION_MOVE_TO"
|
|align="right" |0
|-
|align="left" |"MISSION_ROUTE_TO"
|
|align="right" |1
|-
|align="left" |"MISSION_MOVE_TO_UNIT"
|
|align="right" |2
|-
|align="left" |"MISSION_SWAP_UNITS"
|
|align="right" |3
|-
|align="left" |"MISSION_SKIP"
|
|align="right" |4
|-
|align="left" |"MISSION_SLEEP"
|
|align="right" |5
|-
|align="left" |"MISSION_ALERT"
|
|align="right" |6
|-
|align="left" |"MISSION_FORTIFY"
|
|align="right" |7
|-
|align="left" |"MISSION_GARRISON"
|
|align="right" |8
|-
|align="left" |"MISSION_SET_UP_FOR_RANGED_ATTACK"
|
|align="right" |9
|-
|align="left" |"MISSION_EMBARK"
|
|align="right" |10
|-
|align="left" |"MISSION_DISEMBARK"
|
|align="right" |11
|-
|align="left" |"MISSION_AIRPATROL"
|
|align="right" |12
|-
|align="left" |"MISSION_HEAL"
|
|align="right" |13
|-
|align="left" |"MISSION_AIRLIFT"
|
|align="right" |14
|-
|align="left" |"MISSION_NUKE"
|
|align="right" |15
|-
|align="left" |"MISSION_PARADROP"
|
|align="right" |16
|-
|align="left" |"MISSION_AIR_SWEEP"
|
|align="right" |17
|-
|align="left" |"MISSION_REBASE"
|
|align="right" |18
|-
|align="left" |"MISSION_RANGE_ATTACK"
|
|align="right" |19
|-
|align="left" |"MISSION_PILLAGE"
|
|align="right" |20
|-
|align="left" |"MISSION_FOUND"
|
|align="right" |21
|-
|align="left" |"MISSION_JOIN"
|
|align="right" |22
|-
|align="left" |"MISSION_CONSTRUCT"
|
|align="right" |23
|-
|align="left" |"MISSION_DISCOVER"
|
|align="right" |24
|-
|align="left" |"MISSION_HURRY"
|
|align="right" |25
|-
|align="left" |"MISSION_TRADE"
|
|align="right" |26
|-
|align="left" |"MISSION_REPAIR_FLEET"
|
|align="right" |27
|-
|align="left" |"MISSION_SPACESHIP"
|
|align="right" |28
|-
|align="left" |"MISSION_CULTURE_BOMB"
|
|align="right" |29
|-
|align="left" |"MISSION_FOUND_RELIGION"
|
|align="right" |30
|-
|align="left" |"MISSION_GOLDEN_AGE"
|
|align="right" |31
|-
|align="left" |"MISSION_BUILD"
|
|align="right" |32
|-
|align="left" |"MISSION_LEAD"
|
|align="right" |33
|-
|align="left" |"MISSION_DIE_ANIMATION"
|
|align="right" |34
|-
|align="left" |"MISSION_BEGIN_COMBAT"
|
|align="right" |35
|-
|align="left" |"MISSION_END_COMBAT"
|
|align="right" |36
|-
|align="left" |"MISSION_AIRSTRIKE"
|
|align="right" |37
|-
|align="left" |"MISSION_SURRENDER"
|
|align="right" |38
|-
|align="left" |"MISSION_CAPTURED"
|
|align="right" |39
|-
|align="left" |"MISSION_IDLE"
|
|align="right" |40
|-
|align="left" |"MISSION_DIE"
|
|align="right" |41
|-
|align="left" |"MISSION_DAMAGE"
|
|align="right" |42
|-
|align="left" |"MISSION_MULTI_SELECT"
|
|align="right" |43
|-
|align="left" |"MISSION_MULTI_DESELECT"
|
|align="right" |44
|-
|align="left" |"MISSION_WAIT_FOR"
|
|align="right" |45
|-
|align="left" |"MISSION_SPREAD_RELIGION"
|
|align="right" |46
|-
|align="left" |"MISSION_ENHANCE_RELIGION"
|
|align="right" |47
|-
|align="left" |"MISSION_REMOVE_HERESY"
|
|align="right" |48
|-
|align="left" |"NUM_MISSION_TYPES"
|
|align="right" |49
|}</code>


= XML: the Missions table =
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
|MISSION_MOVE_TO
|-
|align="right"|1
|
|MISSION_ROUTE_TO
|-
|align="right"|2
|
|MISSION_MOVE_TO_UNIT
|-
|align="right"|3
|
|MISSION_SWAP_UNITS
|-
|align="right"|4
|
|MISSION_SKIP
|-
|align="right"|5
|
|MISSION_SLEEP
|-
|align="right"|6
|
|MISSION_ALERT
|-
|align="right"|7
|
|MISSION_FORTIFY
|-
|align="right"|8
|
|MISSION_GARRISON
|-
|align="right"|9
|
|MISSION_SET_UP_FOR_RANGED_ATTACK
|-
|align="right"|10
|
|MISSION_EMBARK
|-
|align="right"|11
|
|MISSION_DISEMBARK
|-
|align="right"|12
|
|MISSION_AIRPATROL
|-
|align="right"|13
|
|MISSION_HEAL
|-
|align="right"|14
|
|MISSION_AIRLIFT
|-
|align="right"|15
|
|MISSION_NUKE
|-
|align="right"|16
|
|MISSION_PARADROP
|-
|align="right"|17
|
|MISSION_AIR_SWEEP
|-
|align="right"|18
|
|MISSION_REBASE
|-
|align="right"|19
|
|MISSION_RANGE_ATTACK
|-
|align="right"|20
|
|MISSION_PILLAGE
|-
|align="right"|21
|
|MISSION_FOUND
|-
|align="right"|22
|
|MISSION_JOIN
|-
|align="right"|23
|
|MISSION_CONSTRUCT
|-
|align="right"|24
|
|MISSION_DISCOVER
|-
|align="right"|25
|
|MISSION_HURRY
|-
|align="right"|26
|
|MISSION_TRADE
|-
|align="right"|27
|
|MISSION_SPACESHIP
|-
|align="right"|27
|
|MISSION_REPAIR_FLEET
|-
|align="right"|28
|
|MISSION_CULTURE_BOMB
|-
|align="right"|29
|
|MISSION_GOLDEN_AGE
|-
|align="right"|30
|
|MISSION_BUILD
|-
|align="right"|30
|
|MISSION_FOUND_RELIGION
|-
|align="right"|31
|
|MISSION_LEAD
|-
|align="right"|32
|
|MISSION_DIE_ANIMATION
|-
|align="right"|33
|
|MISSION_BEGIN_COMBAT
|-
|align="right"|34
|
|MISSION_END_COMBAT
|-
|align="right"|35
|
|MISSION_AIRSTRIKE
|-
|align="right"|36
|
|MISSION_SURRENDER
|-
|align="right"|37
|
|MISSION_CAPTURED
|-
|align="right"|38
|
|MISSION_IDLE
|-
|align="right"|39
|
|MISSION_DIE
|-
|align="right"|40
|
|MISSION_DAMAGE
|-
|align="right"|41
|
|MISSION_MULTI_SELECT
|-
|align="right"|42
|
|MISSION_MULTI_DESELECT
|-
|align="right"|43
|
|MISSION_WAIT_FOR
|-
|align="right"|46
|
|MISSION_SPREAD_RELIGION
|-
|align="right"|47
|
|MISSION_ENHANCE_RELIGION
|-
|align="right"|48
|
|MISSION_REMOVE_HERESY
|}</code>


= Examples =
Here is how to use the LUA enumeration to retrieve the ''ID'' from the ''type''. Those examples will return and assign the integer value 0.
<syntaxhighlight lang="lua" class="civ5-example">
local id = MissionTypes.MISSION_MOVE_TO
local id = MissionTypes["MISSION_MOVE_TO"]
</syntaxhighlight>
Here is how to use the LUA enumeration to retrieve one of string values from its index. Those examples will return and assign the string value MISSION_MOVE_TO.
<syntaxhighlight lang="lua" class="civ5-example">
local str = MissionTypes[0]
</syntaxhighlight>


=Used by=
{|cellspacing="4" cellpadding="0" width="100%" style="background-color:#F0F0F0"
<!-- 
PUSHMISSION
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Unit}}:{{Func5|Unit|PushMission}}<b>(</b>{{Type5|MissionType}} mission, '''int''' data1 = -1, '''int''' data2 = -1, '''int''' flags = 0, '''bool''' append = false, '''bool''' manual = fa;se, {{Type5|MissionType}} missionAI = NO_MISSIONAI, {{Type5|Plot}} missionAIPlot = nil, {{Type5|Unit}} missionAIUnit = nil<b>)</b></code>
|}




{{Civ5 API Footer}}
[[Category:Civ5 Types|MissionType]]