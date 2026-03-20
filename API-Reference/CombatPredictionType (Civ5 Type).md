{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|ID.png|The <code>CombatPredictionType</code> pseudo-type is actually a regular '''integer'''. Pseudo-types do not exist in Lua, they only serve a documentation purpose on the wiki!
* {{Lua}} Integers labeled as <code>CombatPredictionType</code> corresponds to the constants defined in the '''CombatPredictionTypes''' Lua enumeration.
}}


= Lua: the CombatPredictionTypes enumeration =
Firaxis provides a Lua enumeration named <code>CombatPredictionTypes</code>. This is just a regular global table. Its keys are the constants' names and the pairs the corresponding values.

<br/>Below are the values found in this enumeration.
<code>
{|
|-
!align="left" |Key
!
!align="left" |Value 
|-
|align="left" |"NO_COMBAT_PREDICTION"
|
|align="right" |-1
|-
|align="left" |"COMBAT_PREDICTION_RANGED"
|
|align="right" |0
|-
|align="left" |"COMBAT_PREDICTION_STALEMATE"
|
|align="right" |1
|-
|align="left" |"COMBAT_PREDICTION_TOTAL_DEFEAT"
|
|align="right" |2
|-
|align="left" |"COMBAT_PREDICTION_TOTAL_VICTORY"
|
|align="right" |3
|-
|align="left" |"COMBAT_PREDICTION_MAJOR_VICTORY"
|
|align="right" |4
|-
|align="left" |"COMBAT_PREDICTION_SMALL_VICTORY"
|
|align="right" |5
|-
|align="left" |"COMBAT_PREDICTION_MAJOR_DEFEAT"
|
|align="right" |6
|-
|align="left" |"COMBAT_PREDICTION_SMALL_DEFEAT"
|
|align="right" |7
|-
|align="left" |"NUM_COMBAT_PREDICTIONS"
|
|align="right" |8
|}</code>


= Examples =
Here is how to use the LUA enumeration to retrieve the ''ID'' from the ''type''. Those examples will return and assign the integer value 0.
<syntaxhighlight lang="lua" class="civ5-example">
local id = CombatPredictionTypes.COMBAT_PREDICTION_RANGED
local id = CombatPredictionTypes["COMBAT_PREDICTION_RANGED"]
</syntaxhighlight>


=Used by=
{|cellspacing="4" cellpadding="0" width="100%" style="background-color:#F0F0F0"
<!-- 
GETCOMBATPREDICTION
-->
|-
|align="right" width="200" |<code>{{Type5|CombatPredictionType}}</code>
|style="padding-left:6px" |<code>{{Type5|Game}}.{{Func5|Game|GetCombatPrediction}}<b>(</b>{{Type5|Unit}} myUnit, {{Type5|Unit}} theirUnit<b>)</b></code>
|}




{{Civ5 API Footer}}
[[Category:Civ5 Types|CombatPredictionType]]