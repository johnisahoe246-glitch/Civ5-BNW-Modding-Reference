{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|ID.png|The <code>EndGameType</code> pseudo-type is actually a regular '''integer'''. Pseudo-types do not exist in Lua, they only serve a documentation purpose on the wiki!
* {{Lua}} Integers labeled as <code>EndGameType</code> corresponds to the constants defined in the '''EndGameTypes''' Lua enumeration.
}}


= Lua: the EndGameTypes enumeration =
Firaxis provides a Lua enumeration named <code>EndGameTypes</code>. This is just a regular global table. Its keys are the constants' names and the pairs the corresponding values.

<br/>Below are the values found in this enumeration.
<code>
{|
|-
!align="left" |Key
!
!align="left" |Value 
|-
|align="left" |"Technology"
|
|align="right" |0
|-
|align="left" |"Culture"
|
|align="right" |1
|-
|align="left" |"Domination"
|
|align="right" |2
|-
|align="left" |"Diplomatic"
|
|align="right" |3
|-
|align="left" |"Time"
|
|align="right" |4
|-
|align="left" |"Tutorial1"
|
|align="right" |5
|-
|align="left" |"Tutorial2"
|
|align="right" |6
|-
|align="left" |"Tutorial3"
|
|align="right" |7
|-
|align="left" |"Tutorial4"
|
|align="right" |8
|-
|align="left" |"Tutorial5"
|
|align="right" |9
|-
|align="left" |"Loss"
|
|align="right" |10
|}</code>


= Examples =
Here is how to use the LUA enumeration to retrieve the ''ID'' from the ''type''. Those examples will return and assign the integer value 0.
<syntaxhighlight lang="lua" class="civ5-example">
local id = EndGameTypes.Technology
local id = EndGameTypes["Technology"]
</syntaxhighlight>


=Used by=
{|cellspacing="4" cellpadding="0" width="100%" style="background-color:#F0F0F0"
<!-- 
ENDGAMESHOW
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Events}}.{{Func5|Events|EndGameShow}}<b>(</b>{{Type5|EndGameType}} type, {{Type5|TeamID}} team<b>)</b></code>
|}




{{Civ5 API Footer}}
[[Category:Civ5 Types|EndGameType]]