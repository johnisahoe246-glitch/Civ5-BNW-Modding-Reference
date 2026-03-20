{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|ID.png|The <code>SlotStatus</code> pseudo-type is actually a regular '''integer'''. Pseudo-types do not exist in Lua, they only serve a documentation purpose on the wiki!
* {{Lua}} Integers labeled as <code>SlotStatus</code> corresponds to the constants defined in the '''SlotStatus''' Lua enumeration.
}}


= Lua: the SlotStatus enumeration =
Firaxis provides a Lua enumeration named <code>SlotStatus</code>. This is just a regular global table. Its keys are the constants' names and the pairs the corresponding values.

<br/>Below are the values found in this enumeration.
<code>
{|
|-
!align="left" |Key
!
!align="left" |Value 
|-
|align="left" |"SS_OPEN"
|
|align="right" |0
|-
|align="left" |"SS_COMPUTER"
|
|align="right" |1
|-
|align="left" |"SS_CLOSED"
|
|align="right" |2
|-
|align="left" |"SS_TAKEN"
|
|align="right" |3
|-
|align="left" |"SS_OBSERVER"
|
|align="right" |4
|-
|align="left" |"SS_MAX_SLOT_STATUS"
|
|align="right" |5
|}</code>


= Examples =
Here is how to use the LUA enumeration to retrieve the ''ID'' from the ''type''. Those examples will return and assign the integer value 0.
<syntaxhighlight lang="lua" class="civ5-example">
local id = SlotStatus.SS_OPEN
local id = SlotStatus["SS_OPEN"]
</syntaxhighlight>


=Used by=
{|cellspacing="4" cellpadding="0" width="100%" style="background-color:#F0F0F0"
<!-- 
GETSLOTSTATUS
-->
|-
|align="right" width="200" |<code>{{Type5|SlotStatus}}</code>
|style="padding-left:6px" |<code>{{Type5|PreGame}}.{{Func5|PreGame|GetSlotStatus}}<b>(</b>{{Type5|PlayerID}} player<b>)</b></code>
<!-- 
SETSLOTSTATUS
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|PreGame}}.{{Func5|PreGame|SetSlotStatus}}<b>(</b>{{Type5|PlayerID}} i, {{Type5|SlotStatus}} arg1<b>)</b></code>
|}




{{Civ5 API Footer}}
[[Category:Civ5 Types|SlotStatus]]