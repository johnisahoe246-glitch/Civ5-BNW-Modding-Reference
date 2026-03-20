{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|ID.png|The <code>MajorCivApproachType</code> pseudo-type is actually a regular '''integer'''. Pseudo-types do not exist in Lua, they only serve a documentation purpose on the wiki!
* {{Lua}} Integers labeled as <code>MajorCivApproachType</code> corresponds to the constants defined in the '''MajorCivApproachTypes''' Lua enumeration.
}}


= Lua: the MajorCivApproachTypes enumeration =
Firaxis provides a Lua enumeration named <code>MajorCivApproachTypes</code>. This is just a regular global table. Its keys are the constants' names and the pairs the corresponding values.

<br/>Below are the values found in this enumeration.
<code>
{|
|-
!align="left" |Key
!
!align="left" |Value 
|-
|align="left" |"NO_MAJOR_CIV_APPROACH"
|
|align="right" |-1
|-
|align="left" |"MAJOR_CIV_APPROACH_WAR"
|
|align="right" |0
|-
|align="left" |"MAJOR_CIV_APPROACH_HOSTILE"
|
|align="right" |1
|-
|align="left" |"MAJOR_CIV_APPROACH_DECEPTIVE"
|
|align="right" |2
|-
|align="left" |"MAJOR_CIV_APPROACH_GUARDED"
|
|align="right" |3
|-
|align="left" |"MAJOR_CIV_APPROACH_AFRAID"
|
|align="right" |4
|-
|align="left" |"MAJOR_CIV_APPROACH_FRIENDLY"
|
|align="right" |5
|-
|align="left" |"MAJOR_CIV_APPROACH_NEUTRAL"
|
|align="right" |6
|-
|align="left" |"NUM_MAJOR_CIV_APPROACHES"
|
|align="right" |7
|}</code>


= Examples =
Here is how to use the LUA enumeration to retrieve the ''ID'' from the ''type''. Those examples will return and assign the integer value 0.
<syntaxhighlight lang="lua" class="civ5-example">
local id = MajorCivApproachTypes.MAJOR_CIV_APPROACH_WAR
local id = MajorCivApproachTypes["MAJOR_CIV_APPROACH_WAR"]
</syntaxhighlight>


=Used by=
{|cellspacing="4" cellpadding="0" width="100%" style="background-color:#F0F0F0"
<!-- 
GETAPPROACHTOWARDSUSGUESS
-->
|-
|align="right" width="200" |<code>{{Type5|MajorCivApproachType}}</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|GetApproachTowardsUsGuess}}<b>(</b>{{Type5|PlayerID}} player<b>)</b></code>
|}




{{Civ5 API Footer}}
[[Category:Civ5 Types|MajorCivApproachType]]