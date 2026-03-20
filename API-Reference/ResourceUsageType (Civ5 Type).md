{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|ID.png|The <code>ResourceUsageType</code> pseudo-type is actually a regular '''integer'''. Pseudo-types do not exist in Lua, they only serve a documentation purpose on the wiki!
* {{Lua}} Integers labeled as <code>ResourceUsageType</code> corresponds to the constants defined in the '''ResourceUsageTypes''' Lua enumeration.
}}


= Lua: the ResourceUsageTypes enumeration =
Firaxis provides a Lua enumeration named <code>ResourceUsageTypes</code>. This is just a regular global table. Its keys are the constants' names and the pairs the corresponding values.

<br/>Below are the values found in this enumeration.
<code>
{|
|-
!align="left" |Key
!
!align="left" |Value 
|-
|align="left" |"RESOURCEUSAGE_BONUS"
|
|align="right" |0
|-
|align="left" |"RESOURCEUSAGE_STRATEGIC"
|
|align="right" |1
|-
|align="left" |"RESOURCEUSAGE_LUXURY"
|
|align="right" |2
|-
|align="left" |"NUM_RESOURCEUSAGE_TYPES"
|
|align="right" |3
|}</code>


= Examples =
Here is how to use the LUA enumeration to retrieve the ''ID'' from the ''type''. Those examples will return and assign the integer value 0.
<syntaxhighlight lang="lua" class="civ5-example">
local id = ResourceUsageTypes.RESOURCEUSAGE_BONUS
local id = ResourceUsageTypes["RESOURCEUSAGE_BONUS"]
</syntaxhighlight>


=Used by=
{|cellspacing="4" cellpadding="0" width="100%" style="background-color:#F0F0F0"
<!-- 
GETRESOURCEUSAGETYPE
-->
|-
|align="right" width="200" |<code>{{Type5|ResourceUsageType}}</code>
|style="padding-left:6px" |<code>{{Type5|Game}}.{{Func5|Game|GetResourceUsageType}}<b>(</b>{{Type5|ResourceType}} resourceLoop<b>)</b></code>
|}




{{Civ5 API Footer}}
[[Category:Civ5 Types|ResourceUsageType]]