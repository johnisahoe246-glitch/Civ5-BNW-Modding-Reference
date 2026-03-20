{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|ID.png|The <code>SlotClaim</code> pseudo-type is actually a regular '''integer'''. Pseudo-types do not exist in Lua, they only serve a documentation purpose on the wiki!
* {{Lua}} Integers labeled as <code>SlotClaim</code> corresponds to the constants defined in the '''SlotClaim''' Lua enumeration.
}}


= Lua: the SlotClaim enumeration =
Firaxis provides a Lua enumeration named <code>SlotClaim</code>. This is just a regular global table. Its keys are the constants' names and the pairs the corresponding values.

<br/>Below are the values found in this enumeration.
<code>
{|
|-
!align="left" |Key
!
!align="left" |Value 
|-
|align="left" |"SLOTCLAIM_UNASSIGNED"
|
|align="right" |0
|-
|align="left" |"SLOTCLAIM_RESERVED"
|
|align="right" |1
|-
|align="left" |"SLOTCLAIM_ASSIGNED"
|
|align="right" |2
|-
|align="left" |"NUM_SLOTCLAIMS"
|
|align="right" |3
|}</code>


= Examples =
Here is how to use the LUA enumeration to retrieve the ''ID'' from the ''type''. Those examples will return and assign the integer value 0.
<syntaxhighlight lang="lua" class="civ5-example">
local id = SlotClaim.SLOTCLAIM_UNASSIGNED
local id = SlotClaim["SLOTCLAIM_UNASSIGNED"]
</syntaxhighlight>


=Used by=
{|cellspacing="4" cellpadding="0" width="100%" style="background-color:#F0F0F0"
<!-- 
GETSLOTCLAIM
-->
|-
|align="right" width="200" |<code>{{Type5|SlotClaim}}</code>
|style="padding-left:6px" |<code>{{Type5|PreGame}}.{{Func5|PreGame|GetSlotClaim}}<b>(</b>{{Type5|PlayerID}} player<b>)</b></code>
<!-- 
SETSLOTCLAIM
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|PreGame}}.{{Func5|PreGame|SetSlotClaim}}<b>(</b>{{Type5|PlayerID}} player, {{Type5|SlotClaim}} arg1<b>)</b></code>
|}




{{Civ5 API Footer}}
[[Category:Civ5 Types|SlotClaim]]