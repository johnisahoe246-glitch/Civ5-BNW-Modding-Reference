{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|ID.png|The <code>CoopWarState</code> pseudo-type is actually a regular '''integer'''. Pseudo-types do not exist in Lua, they only serve a documentation purpose on the wiki!
* {{Lua}} Integers labeled as <code>CoopWarState</code> corresponds to the constants defined in the '''CoopWarStates''' Lua enumeration.
}}


= Lua: the CoopWarStates enumeration =
Firaxis provides a Lua enumeration named <code>CoopWarStates</code>. This is just a regular global table. Its keys are the constants' names and the pairs the corresponding values.

<br/>Below are the values found in this enumeration.
<code>
{|
|-
!align="left" |Key
!
!align="left" |Value 
|-
|align="left" |"NO_COOP_WAR_STATE"
|
|align="right" |-1
|-
|align="left" |"COOP_WAR_STATE_REJECTED"
|
|align="right" |0
|-
|align="left" |"COOP_WAR_STATE_SOON"
|
|align="right" |1
|-
|align="left" |"COOP_WAR_STATE_ACCEPTED"
|
|align="right" |2
|-
|align="left" |"NUM_COOP_WAR_STATES"
|
|align="right" |3
|}</code>


= Examples =
Here is how to use the LUA enumeration to retrieve the ''ID'' from the ''type''. Those examples will return and assign the integer value 0.
<syntaxhighlight lang="lua" class="civ5-example">
local id = CoopWarStates.COOP_WAR_STATE_REJECTED
local id = CoopWarStates["COOP_WAR_STATE_REJECTED"]
</syntaxhighlight>


=Used by=
{|cellspacing="4" cellpadding="0" width="100%" style="background-color:#F0F0F0"
<!-- 
GETCOOPWARACCEPTEDSTATE
-->
|-
|align="right" width="200" |<code>{{Type5|CoopWarState}}</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|GetCoopWarAcceptedState}}<b>(</b>{{Type5|PlayerID}} withPlayer, {{Type5|PlayerID}} againstPlayer<b>)</b></code>
|}




{{Civ5 API Footer}}
[[Category:Civ5 Types|CoopWarState]]