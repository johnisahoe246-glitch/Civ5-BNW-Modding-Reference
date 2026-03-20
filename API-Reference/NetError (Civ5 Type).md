{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|ID.png|The <code>NetError</code> pseudo-type is actually a regular '''integer'''. Pseudo-types do not exist in Lua, they only serve a documentation purpose on the wiki!
* {{Lua}} Integers labeled as <code>NetError</code> corresponds to the constants defined in the '''NetErrors''' Lua enumeration.
}}


= Lua: the NetErrors enumeration =
Firaxis provides a Lua enumeration named <code>NetErrors</code>. This is just a regular global table. Its keys are the constants' names and the pairs the corresponding values.

<br/>Below are the values found in this enumeration.
<code>
{|
|-
!align="left" |Key
!
!align="left" |Value 
|-
|align="left" |"NO_ERROR"
|
|align="right" |0
|-
|align="left" |"MISSING_REQUIRED_DATA"
|
|align="right" |1
|-
|align="left" |"ROOM_FULL"
|
|align="right" |2
|}</code>


= Examples =
Here is how to use the LUA enumeration to retrieve the ''ID'' from the ''type''. Those examples will return and assign the integer value 0.
<syntaxhighlight lang="lua" class="civ5-example">
local id = NetErrors.NO_ERROR
local id = NetErrors["NO_ERROR"]
</syntaxhighlight>


=Used by=
{|cellspacing="4" cellpadding="0" width="100%" style="background-color:#F0F0F0"
<!-- 
MULTIPLAYERJOINROOMFAILED
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Events}}.{{Func5|Events|MultiplayerJoinRoomFailed}}<b>(</b>{{Type5|NetError}} extendedError, '''unknown''' aExtendedErrorText<b>)</b></code>
|}




{{Civ5 API Footer}}
[[Category:Civ5 Types|NetError]]