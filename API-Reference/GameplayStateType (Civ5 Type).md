{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|ID.png|The <code>GameplayStateType</code> pseudo-type is actually a regular '''integer'''. Pseudo-types do not exist in Lua, they only serve a documentation purpose on the wiki!
* {{Lua}} Integers labeled as <code>GameplayStateType</code> corresponds to the constants defined in the '''GameplayGameStateTypes''' Lua enumeration.
}}


= Lua: the GameplayGameStateTypes enumeration =
Firaxis provides a Lua enumeration named <code>GameplayGameStateTypes</code>. This is just a regular global table. Its keys are the constants' names and the pairs the corresponding values.

<br/>Below are the values found in this enumeration.
<code>
{|
|-
!align="left" |Key
!
!align="left" |Value 
|-
|align="left" |"GAMESTATE_ON"
|
|align="right" |0
|-
|align="left" |"GAMESTATE_OVER"
|
|align="right" |1
|-
|align="left" |"GAMESTATE_EXTENDED"
|
|align="right" |2
|}</code>


= Examples =
Here is how to use the LUA enumeration to retrieve the ''ID'' from the ''type''. Those examples will return and assign the integer value 0.
<syntaxhighlight lang="lua" class="civ5-example">
local id = GameplayGameStateTypes.GAMESTATE_ON
local id = GameplayGameStateTypes["GAMESTATE_ON"]
</syntaxhighlight>


=Used by=
{|cellspacing="4" cellpadding="0" width="100%" style="background-color:#F0F0F0"
<!-- 
GETGAMESTATE
-->
|-
|align="right" width="200" |<code>{{Type5|GameplayStateType}}</code>
|style="padding-left:6px" |<code>{{Type5|Game}}.{{Func5|Game|GetGameState}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
SETGAMESTATE
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Game}}.{{Func5|Game|SetGameState}}<b>(</b>{{Type5|GameplayStateType}} arg0<b>)</b></code>
|}




{{Civ5 API Footer}}
[[Category:Civ5 Types|GameplayStateType]]