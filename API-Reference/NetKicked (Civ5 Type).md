{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|ID.png|The <code>NetKicked</code> pseudo-type is actually a regular '''integer'''. Pseudo-types do not exist in Lua, they only serve a documentation purpose on the wiki!
* {{Lua}} Integers labeled as <code>NetKicked</code> corresponds to the constants defined in the '''NetKicked''' Lua enumeration.
}}


= Lua: the NetKicked enumeration =
Firaxis provides a Lua enumeration named <code>NetKicked</code>. This is just a regular global table. Its keys are the constants' names and the pairs the corresponding values.

<br/>Below are the values found in this enumeration.
<code>
{|
|-
!align="left" |Key
!
!align="left" |Value 
|-
|align="left" |"NONE"
|
|align="right" |0
|-
|align="left" |"NO_HOST"
|
|align="right" |1
|-
|align="left" |"BY_HOST"
|
|align="right" |2
|-
|align="left" |"TIMEOUT"
|
|align="right" |3
|-
|align="left" |"UNRECOGNIZED"
|
|align="right" |4
|-
|align="left" |"UNAUTHORIZED"
|
|align="right" |5
|-
|align="left" |"NO_ROOM"
|
|align="right" |6
|}</code>


= Examples =
Here is how to use the LUA enumeration to retrieve the ''ID'' from the ''type''. Those examples will return and assign the integer value 0.
<syntaxhighlight lang="lua" class="civ5-example">
local id = NetKicked.NONE
local id = NetKicked["NONE"]
</syntaxhighlight>


=Used by=
{|cellspacing="4" cellpadding="0" width="100%" style="background-color:#F0F0F0"
<!-- 
MULTIPLAYERGAMEABANDONED
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Events}}.{{Func5|Events|MultiplayerGameAbandoned}}<b>(</b>{{Type5|NetKicked}} reason<b>)</b></code>
|}




{{Civ5 API Footer}}
[[Category:Civ5 Types|NetKicked]]