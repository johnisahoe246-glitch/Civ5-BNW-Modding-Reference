{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|ID.png|The <code>DisputeLevelType</code> pseudo-type is actually a regular '''integer'''. Pseudo-types do not exist in Lua, they only serve a documentation purpose on the wiki!
* {{Lua}} Integers labeled as <code>DisputeLevelType</code> corresponds to the constants defined in the '''DisputeLevelTypes''' Lua enumeration.
}}


= Lua: the DisputeLevelTypes enumeration =
Firaxis provides a Lua enumeration named <code>DisputeLevelTypes</code>. This is just a regular global table. Its keys are the constants' names and the pairs the corresponding values.

<br/>Below are the values found in this enumeration.
<code>
{|
|-
!align="left" |Key
!
!align="left" |Value 
|-
|align="left" |"NO_DISPUTE_LEVEL"
|
|align="right" |-1
|-
|align="left" |"DISPUTE_LEVEL_NONE"
|
|align="right" |0
|-
|align="left" |"DISPUTE_LEVEL_WEAK"
|
|align="right" |1
|-
|align="left" |"DISPUTE_LEVEL_STRONG"
|
|align="right" |2
|-
|align="left" |"DISPUTE_LEVEL_FIERCE"
|
|align="right" |3
|-
|align="left" |"NUM_DISPUTE_LEVELS"
|
|align="right" |4
|}</code>


= Examples =
Here is how to use the LUA enumeration to retrieve the ''ID'' from the ''type''. Those examples will return and assign the integer value 0.
<syntaxhighlight lang="lua" class="civ5-example">
local id = DisputeLevelTypes.DISPUTE_LEVEL_NONE
local id = DisputeLevelTypes["DISPUTE_LEVEL_NONE"]
</syntaxhighlight>


=Used by=
{|cellspacing="4" cellpadding="0" width="100%" style="background-color:#F0F0F0"
<!-- 
GETLANDDISPUTELEVEL
-->
|-
|align="right" width="200" |<code>{{Type5|DisputeLevelType}}</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|GetLandDisputeLevel}}<b>(</b>{{Type5|PlayerID}} activePlayer<b>)</b></code>
<!-- 
GETMINORCIVDISPUTELEVEL
-->
|-
|align="right" width="200" |<code>{{Type5|DisputeLevelType}}</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|GetMinorCivDisputeLevel}}<b>(</b>{{Type5|PlayerID}} activePlayer<b>)</b></code>
<!-- 
GETWONDERDISPUTELEVEL
-->
|-
|align="right" width="200" |<code>{{Type5|DisputeLevelType}}</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|GetWonderDisputeLevel}}<b>(</b>{{Type5|PlayerID}} activePlayer<b>)</b></code>
|}




{{Civ5 API Footer}}
[[Category:Civ5 Types|DisputeLevelType]]