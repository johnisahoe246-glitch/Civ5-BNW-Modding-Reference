{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|ID.png|The <code>DirectionType</code> pseudo-type is actually a regular '''integer'''. Pseudo-types do not exist in Lua, they only serve a documentation purpose on the wiki!
* {{Lua}} Integers labeled as <code>DirectionType</code> corresponds to the constants defined in the '''DirectionTypes''' Lua enumeration.
}}


= Lua: the DirectionTypes enumeration =
Firaxis provides a Lua enumeration named <code>DirectionTypes</code>. This is just a regular global table. Its keys are the constants' names and the pairs the corresponding values.

<br/>Below are the values found in this enumeration.
<code>
{|
|-
!align="left" |Key
!
!align="left" |Value 
|-
|align="left" |"NO_DIRECTION"
|
|align="right" |-1
|-
|align="left" |"DIRECTION_NORTHEAST"
|
|align="right" |0
|-
|align="left" |"DIRECTION_EAST"
|
|align="right" |1
|-
|align="left" |"DIRECTION_SOUTHEAST"
|
|align="right" |2
|-
|align="left" |"DIRECTION_SOUTHWEST"
|
|align="right" |3
|-
|align="left" |"DIRECTION_WEST"
|
|align="right" |4
|-
|align="left" |"DIRECTION_NORTHWEST"
|
|align="right" |5
|-
|align="left" |"NUM_DIRECTION_TYPES"
|
|align="right" |6
|}</code>


= Examples =
Here is how to use the LUA enumeration to retrieve the ''ID'' from the ''type''. Those examples will return and assign the integer value 0.
<syntaxhighlight lang="lua" class="civ5-example">
local id = DirectionTypes.DIRECTION_NORTHEAST
local id = DirectionTypes["DIRECTION_NORTHEAST"]
</syntaxhighlight>


=Used by=
{|cellspacing="4" cellpadding="0" width="100%" style="background-color:#F0F0F0"
<!-- 
INITUNIT
-->
|-
|align="right" width="200" |<code>{{Type5|Unit}}</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|InitUnit}}<b>(</b>{{Type5|UnitType}} unit, {{Type5|ResourceType}} x, {{Type5|ResourceType}} y, {{Type5|UnitAIType}} unitAI = NO_UNITAI, {{Type5|DirectionType}} facingDirection = NO_DIRECTION<b>)</b></code>
<!-- 
ISRIVERCONNECTION
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|Plot}}:{{Func5|Plot|IsRiverConnection}}<b>(</b>{{Type5|DirectionType}} direction<b>)</b></code>
<!-- 
ISRIVERCROSSING
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|Plot}}:{{Func5|Plot|IsRiverCrossing}}<b>(</b>{{Type5|DirectionType}} index<b>)</b></code>
<!-- 
ISRIVERCROSSINGTOPLOT
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|Plot}}:{{Func5|Plot|IsRiverCrossingToPlot}}<b>(</b>{{Type5|DirectionType}} index<b>)</b></code>
|}




{{Civ5 API Footer}}
[[Category:Civ5 Types|DirectionType]]