{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|ID.png|The <code>GenericWorldAnchorType</code> pseudo-type is actually a regular '''integer'''. Pseudo-types do not exist in Lua, they only serve a documentation purpose on the wiki!
* {{Lua}} Integers labeled as <code>GenericWorldAnchorType</code> corresponds to the constants defined in the '''GenericWorldAnchorTypes''' Lua enumeration.
}}


= Lua: the GenericWorldAnchorTypes enumeration =
Firaxis provides a Lua enumeration named <code>GenericWorldAnchorTypes</code>. This is just a regular global table. Its keys are the constants' names and the pairs the corresponding values.

<br/>Below are the values found in this enumeration.
<code>
{|
|-
!align="left" |Key
!
!align="left" |Value 
|-
|align="left" |"NO_WORLD_ANCHOR"
|
|align="right" |-1
|-
|align="left" |"WORLD_ANCHOR_NATURAL_WONDER"
|
|align="right" |0
|-
|align="left" |"WORLD_ANCHOR_SETTLER"
|
|align="right" |1
|-
|align="left" |"WORLD_ANCHOR_WORKER"
|
|align="right" |2
|-
|align="left" |"NUM_WORLD_ANCHORS"
|
|align="right" |3
|}</code>


= Examples =
Here is how to use the LUA enumeration to retrieve the ''ID'' from the ''type''. Those examples will return and assign the integer value 0.
<syntaxhighlight lang="lua" class="civ5-example">
local id = GenericWorldAnchorTypes.WORLD_ANCHOR_NATURAL_WONDER
local id = GenericWorldAnchorTypes["WORLD_ANCHOR_NATURAL_WONDER"]
</syntaxhighlight>


=Used by=
{|cellspacing="4" cellpadding="0" width="100%" style="background-color:#F0F0F0"
<!-- 
GENERICWORLDANCHOR
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Events}}.{{Func5|Events|GenericWorldAnchor}}<b>(</b>{{Type5|GenericWorldAnchorType}} type, '''bool''' show, '''int''' plotX, '''int''' plotY, {{Type5|FeatureType}} data1 = nil<b>)</b></code>
|}




{{Civ5 API Footer}}
[[Category:Civ5 Types|GenericWorldAnchorType]]