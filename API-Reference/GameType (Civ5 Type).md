{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|ID.png|The <code>GameType</code> pseudo-type is actually a regular '''integer'''. Pseudo-types do not exist in Lua, they only serve a documentation purpose on the wiki!
* {{Lua}} Integers labeled as <code>GameType</code> corresponds to the constants defined in the '''GameTypes''' Lua enumeration.
}}


= Lua: the GameTypes enumeration =
Firaxis provides a Lua enumeration named <code>GameTypes</code>. This is just a regular global table. Its keys are the constants' names and the pairs the corresponding values.

<br/>Below are the values found in this enumeration.
<code>
{|
|-
!align="left" |Key
!
!align="left" |Value 
|-
|align="left" |"GAME_TYPE_NONE"
|
|align="right" |-1
|-
|align="left" |"GAME_SINGLE_PLAYER"
|
|align="right" |0
|-
|align="left" |"GAME_NETWORK_MULTIPLAYER"
|
|align="right" |1
|-
|align="left" |"GAME_HOTSEAT_MULTIPLAYER"
|
|align="right" |2
|-
|align="left" |"GAME_EMAIL_MULTIPLAYER"
|
|align="right" |3
|}</code>


= Examples =
Here is how to use the LUA enumeration to retrieve the ''ID'' from the ''type''. Those examples will return and assign the integer value 0.
<syntaxhighlight lang="lua" class="civ5-example">
local id = GameTypes.GAME_SINGLE_PLAYER
local id = GameTypes["GAME_SINGLE_PLAYER"]
</syntaxhighlight>


=Used by=
{|cellspacing="4" cellpadding="0" width="100%" style="background-color:#F0F0F0"
<!-- 
GETGAMETYPE
-->
|-
|align="right" width="200" |<code>{{Type5|GameType}}</code>
|style="padding-left:6px" |<code>{{Type5|PreGame}}.{{Func5|PreGame|GetGameType}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
SETGAMETYPE
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|PreGame}}.{{Func5|PreGame|SetGameType}}<b>(</b>{{Type5|GameType}} gameType<b>)</b></code>
<!-- 
SAVEFILELIST
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|UI}}.{{Func5|UI|SaveFileList}}<b>(</b>table({{Type5|SpecialistType}} => '''bool''') FileList, {{Type5|GameType}} GameType, '''bool''' ShowAutoSaves, '''bool''' arg3<b>)</b></code>
|}




{{Civ5 API Footer}}
[[Category:Civ5 Types|GameType]]