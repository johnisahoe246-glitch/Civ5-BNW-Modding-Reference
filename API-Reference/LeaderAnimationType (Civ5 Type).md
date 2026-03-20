{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|ID.png|The <code>LeaderAnimationType</code> pseudo-type is actually a regular '''integer'''. Pseudo-types do not exist in Lua, they only serve a documentation purpose on the wiki!
* {{Lua}} Integers labeled as <code>LeaderAnimationType</code> corresponds to the constants defined in the '''LeaderheadAnimationTypes''' Lua enumeration.
}}


= Lua: the LeaderheadAnimationTypes enumeration =
Firaxis provides a Lua enumeration named <code>LeaderheadAnimationTypes</code>. This is just a regular global table. Its keys are the constants' names and the pairs the corresponding values.

<br/>Below are the values found in this enumeration.
<code>
{|
|-
!align="left" |Key
!
!align="left" |Value 
|-
|align="left" |"NO_LEADERHEAD_ANIM"
|
|align="right" |-1
|-
|align="left" |"LEADERHEAD_ANIM_INTRO"
|
|align="right" |1
|-
|align="left" |"LEADERHEAD_ANIM_NEUTRAL_HELLO"
|
|align="right" |2
|-
|align="left" |"LEADERHEAD_ANIM_PEACEFUL"
|
|align="right" |3
|-
|align="left" |"LEADERHEAD_ANIM_OPENING_GLOAT"
|
|align="right" |4
|-
|align="left" |"LEADERHEAD_ANIM_DECLARE_WAR"
|
|align="right" |5
|-
|align="left" |"LEADERHEAD_ANIM_ATTACKED"
|
|align="right" |6
|-
|align="left" |"LEADERHEAD_ANIM_HATE_HELLO"
|
|align="right" |7
|-
|align="left" |"LEADERHEAD_ANIM_DEFEATED"
|
|align="right" |8
|-
|align="left" |"LEADERHEAD_ANIM_REQUEST"
|
|align="right" |9
|-
|align="left" |"LEADERHEAD_ANIM_DEMAND"
|
|align="right" |10
|-
|align="left" |"LEADERHEAD_ANIM_NEUTRAL_IDLE"
|
|align="right" |11
|-
|align="left" |"LEADERHEAD_ANIM_HATE_IDLE"
|
|align="right" |12
|-
|align="left" |"LEADERHEAD_ANIM_LETS_HEAR_IT"
|
|align="right" |15
|-
|align="left" |"LEADERHEAD_ANIM_YES"
|
|align="right" |16
|-
|align="left" |"LEADERHEAD_ANIM_NO"
|
|align="right" |17
|}</code>


= Examples =
Here is how to use the LUA enumeration to retrieve the ''ID'' from the ''type''. Those examples will return and assign the integer value 1.
<syntaxhighlight lang="lua" class="civ5-example">
local id = LeaderheadAnimationTypes.LEADERHEAD_ANIM_INTRO
local id = LeaderheadAnimationTypes["LEADERHEAD_ANIM_INTRO"]
</syntaxhighlight>




{{Civ5 API Footer}}
[[Category:Civ5 Types|LeaderAnimationType]]