{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|ID.png|The <code>GameOptionType</code> pseudo-type is actually a regular '''integer'''. Pseudo-types do not exist in Lua, they only serve a documentation purpose on the wiki!
* {{Lua}} Integers labeled as <code>GameOptionType</code> corresponds to the constants defined in the '''GameOptionTypes''' Lua enumeration.
}}


= Lua: the GameOptionTypes enumeration =
Firaxis provides a Lua enumeration named <code>GameOptionTypes</code>. This is just a regular global table. Its keys are the constants' names and the pairs the corresponding values.

<br/>Below are the values found in this enumeration.
<code>
{|
|-
!align="left" |Key
!
!align="left" |Value 
|-
|align="left" |"NO_GAMEOPTION"
|
|align="right" |-1
|-
|align="left" |"GAMEOPTION_NO_CITY_RAZING"
|
|align="right" |0
|-
|align="left" |"GAMEOPTION_NO_BARBARIANS"
|
|align="right" |1
|-
|align="left" |"GAMEOPTION_RAGING_BARBARIANS"
|
|align="right" |2
|-
|align="left" |"GAMEOPTION_ALWAYS_WAR"
|
|align="right" |3
|-
|align="left" |"GAMEOPTION_ALWAYS_PEACE"
|
|align="right" |4
|-
|align="left" |"GAMEOPTION_ONE_CITY_CHALLENGE"
|
|align="right" |5
|-
|align="left" |"GAMEOPTION_NO_CHANGING_WAR_PEACE"
|
|align="right" |6
|-
|align="left" |"GAMEOPTION_NEW_RANDOM_SEED"
|
|align="right" |7
|-
|align="left" |"GAMEOPTION_LOCK_MODS"
|
|align="right" |8
|-
|align="left" |"GAMEOPTION_COMPLETE_KILLS"
|
|align="right" |9
|-
|align="left" |"GAMEOPTION_NO_GOODY_HUTS"
|
|align="right" |10
|-
|align="left" |"GAMEOPTION_RANDOM_PERSONALITIES"
|
|align="right" |11
|-
|align="left" |"GAMEOPTION_POLICY_SAVING"
|
|align="right" |12
|-
|align="left" |"GAMEOPTION_PROMOTION_SAVING"
|
|align="right" |13
|-
|align="left" |"GAMEOPTION_END_TURN_TIMER_ENABLED"
|
|align="right" |14
|-
|align="left" |"GAMEOPTION_QUICK_COMBAT"
|
|align="right" |15
|-
|align="left" |"GAMEOPTION_DISABLE_START_BIAS"
|
|align="right" |16
|-
|align="left" |"GAMEOPTION_NO_SCIENCE"
|
|align="right" |17
|-
|align="left" |"GAMEOPTION_NO_POLICIES"
|
|align="right" |18
|-
|align="left" |"GAMEOPTION_NO_HAPPINESS"
|
|align="right" |19
|-
|align="left" |"GAMEOPTION_NO_TUTORIAL"
|
|align="right" |20
|-
|align="left" |"GAMEOPTION_NO_RELIGION"
|
|align="right" |21
|-
|align="left" |"NUM_GAMEOPTION_TYPES"
|
|align="right" |22
|}</code>


= Examples =
Here is how to use the LUA enumeration to retrieve the ''ID'' from the ''type''. Those examples will return and assign the integer value 0.
<syntaxhighlight lang="lua" class="civ5-example">
local id = GameOptionTypes.GAMEOPTION_NO_CITY_RAZING
local id = GameOptionTypes["GAMEOPTION_NO_CITY_RAZING"]
</syntaxhighlight>


=Used by=
{|cellspacing="4" cellpadding="0" width="100%" style="background-color:#F0F0F0"
<!-- 
SETOPTION
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Game}}.{{Func5|Game|SetOption}}<b>(</b>{{Type5|GameOptionType}} index, '''bool''' enabled<b>)</b></code>
|}




{{Civ5 API Footer}}
[[Category:Civ5 Types|GameOptionType]]