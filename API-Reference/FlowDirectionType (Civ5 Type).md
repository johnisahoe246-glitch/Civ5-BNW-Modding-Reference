{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|ID.png|The <code>FlowDirectionType</code> pseudo-type is actually a regular '''integer'''. Pseudo-types do not exist in Lua, they only serve a documentation purpose on the wiki!
* {{Lua}} Integers labeled as <code>FlowDirectionType</code> corresponds to the constants defined in the '''FlowDirectionTypes''' Lua enumeration.
}}


= Lua: the FlowDirectionTypes enumeration =
Firaxis provides a Lua enumeration named <code>FlowDirectionTypes</code>. This is just a regular global table. Its keys are the constants' names and the pairs the corresponding values.

<br/>Below are the values found in this enumeration.
<code>
{|
|-
!align="left" |Key
!
!align="left" |Value 
|-
|align="left" |"NO_FLOWDIRECTION"
|
|align="right" |-1
|-
|align="left" |"FLOWDIRECTION_NORTH"
|
|align="right" |0
|-
|align="left" |"FLOWDIRECTION_NORTH_MASK"
|
|align="right" |1
|-
|align="left" |"FLOWDIRECTION_NORTHEAST"
|
|align="right" |1
|-
|align="left" |"FLOWDIRECTION_SOUTH_MASK"
|
|align="right" |2
|-
|align="left" |"FLOWDIRECTION_SOUTHEAST"
|
|align="right" |2
|-
|align="left" |"FLOWDIRECTION_SOUTH"
|
|align="right" |3
|-
|align="left" |"FLOWDIRECTION_SOUTHEAST_MASK"
|
|align="right" |4
|-
|align="left" |"FLOWDIRECTION_SOUTHWEST"
|
|align="right" |4
|-
|align="left" |"FLOWDIRECTION_NORTHWEST"
|
|align="right" |5
|-
|align="left" |"NUM_FLOWDIRECTION_TYPES"
|
|align="right" |6
|-
|align="left" |"FLOWDIRECTION_NORTHWEST_MASK"
|
|align="right" |8
|-
|align="left" |"FLOWDIRECTION_SOUTHWEST_MASK"
|
|align="right" |16
|-
|align="left" |"FLOWDIRECTION_NORTHEAST_MASK"
|
|align="right" |32
|}</code>


= Examples =
Here is how to use the LUA enumeration to retrieve the ''ID'' from the ''type''. Those examples will return and assign the integer value 0.
<syntaxhighlight lang="lua" class="civ5-example">
local id = FlowDirectionTypes.FLOWDIRECTION_NORTH
local id = FlowDirectionTypes["FLOWDIRECTION_NORTH"]
</syntaxhighlight>


=Used by=
{|cellspacing="4" cellpadding="0" width="100%" style="background-color:#F0F0F0"
<!-- 
DORIVER
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Func5|DoRiver}}<b>(</b>{{Type5|Plot}} startPlot, {{Type5|FlowDirectionType}} thisFlowDirection = nil, {{Type5|FlowDirectionType}} originalFlowDirection = nil, '''int''' riverID = nil<b>)</b></code>
<!-- 
GETOPPOSITEFLOWDIRECTION
-->
|-
|align="right" width="200" |<code>{{Type5|FlowDirectionType}}</code>
|style="padding-left:6px" |<code>{{Func5|GetOppositeFlowDirection}}<b>(</b>{{Type5|FlowDirectionType}} dir<b>)</b></code>
<!-- 
GETRIVEREFLOWDIRECTION
-->
|-
|align="right" width="200" |<code>{{Type5|FlowDirectionType}}</code>
|style="padding-left:6px" |<code>{{Type5|Plot}}:{{Func5|Plot|GetRiverEFlowDirection}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETRIVERSEFLOWDIRECTION
-->
|-
|align="right" width="200" |<code>{{Type5|FlowDirectionType}}</code>
|style="padding-left:6px" |<code>{{Type5|Plot}}:{{Func5|Plot|GetRiverSEFlowDirection}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETRIVERSWFLOWDIRECTION
-->
|-
|align="right" width="200" |<code>{{Type5|FlowDirectionType}}</code>
|style="padding-left:6px" |<code>{{Type5|Plot}}:{{Func5|Plot|GetRiverSWFlowDirection}}<b>(</b><!-- No arguments --><b>)</b></code>
|}




{{Civ5 API Footer}}
[[Category:Civ5 Types|FlowDirectionType]]