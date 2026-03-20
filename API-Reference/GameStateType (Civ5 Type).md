{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|ID.png|The <code>GameStateType</code> pseudo-type is actually a regular '''integer'''. Pseudo-types do not exist in Lua, they only serve a documentation purpose on the wiki!
* {{Lua}} Integers labeled as <code>GameStateType</code> corresponds to the constants defined in the '''GameStateTypes''' Lua enumeration.
}}


= Lua: the GameStateTypes enumeration =
Firaxis provides a Lua enumeration named <code>GameStateTypes</code>. This is just a regular global table. Its keys are the constants' names and the pairs the corresponding values.

<br/>Below are the values found in this enumeration.
<code>
{|
|-
!align="left" |Key
!
!align="left" |Value 
|-
|align="left" |"CIV5_GS_UNKNOWN"
|
|align="right" |-1
|-
|align="left" |"CIV5_GS_EXIT"
|
|align="right" |0
|-
|align="left" |"CIV5_GS_OPENING_MOVIE"
|
|align="right" |1
|-
|align="left" |"CIV5_GS_LOAD_GAME"
|
|align="right" |2
|-
|align="left" |"CIV5_GS_MAIN_MENU"
|
|align="right" |3
|-
|align="left" |"CIV5_GS_MULTIPLAYER_MENU"
|
|align="right" |4
|-
|align="left" |"CIV5_GS_LANLOBBY"
|
|align="right" |5
|-
|align="left" |"CIV5_GS_INETLOBBY"
|
|align="right" |6
|-
|align="left" |"CIV5_GS_STAGING"
|
|align="right" |7
|-
|align="left" |"CIV5_GS_SCENARIOSETUP"
|
|align="right" |8
|-
|align="left" |"CIV5_GS_MAINGAMEVIEW"
|
|align="right" |9
|-
|align="left" |"CIV5_GS_UI_VIEWER"
|
|align="right" |10
|-
|align="left" |"CIV5_GS_LEADER_HEAD_BENCHMARK"
|
|align="right" |11
|-
|align="left" |"CIV5_GS_LEADER_HEAD_VIEW"
|
|align="right" |12
|-
|align="left" |"CIV5_GS_NEXUS"
|
|align="right" |13
|-
|align="left" |"CIV5_GS_WORLD_BUILDER_LOAD"
|
|align="right" |14
|-
|align="left" |"CIV5_GS_CREDITS"
|
|align="right" |15
|}</code>


= Examples =
Here is how to use the LUA enumeration to retrieve the ''ID'' from the ''type''. Those examples will return and assign the integer value 0.
<syntaxhighlight lang="lua" class="civ5-example">
local id = GameStateTypes.CIV5_GS_EXIT
local id = GameStateTypes["CIV5_GS_EXIT"]
</syntaxhighlight>


=Used by=
{|cellspacing="4" cellpadding="0" width="100%" style="background-color:#F0F0F0"
<!-- 
GETCURRENTGAMESTATE
-->
|-
|align="right" width="200" |<code>{{Type5|GameStateType}}</code>
|style="padding-left:6px" |<code>{{Type5|UI}}.{{Func5|UI|GetCurrentGameState}}<b>(</b><!-- No arguments --><b>)</b></code>
|}




{{Civ5 API Footer}}
[[Category:Civ5 Types|GameStateType]]