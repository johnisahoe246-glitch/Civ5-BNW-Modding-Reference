{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|ID.png|The <code>MinorCivPersonalityType</code> pseudo-type is actually a regular '''integer'''. Pseudo-types do not exist in Lua, they only serve a documentation purpose on the wiki!
* {{Lua}} Integers labeled as <code>MinorCivPersonalityType</code> corresponds to the constants defined in the '''MinorCivPersonalityTypes''' Lua enumeration.
}}


= Lua: the MinorCivPersonalityTypes enumeration =
Firaxis provides a Lua enumeration named <code>MinorCivPersonalityTypes</code>. This is just a regular global table. Its keys are the constants' names and the pairs the corresponding values.

<br/>Below are the values found in this enumeration.
<code>
{|
|-
!align="left" |Key
!
!align="left" |Value 
|-
|align="left" |"NO_MINOR_CIV_PERSONALITY_TYPE"
|
|align="right" |-1
|-
|align="left" |"MINOR_CIV_PERSONALITY_FRIENDLY"
|
|align="right" |0
|-
|align="left" |"MINOR_CIV_PERSONALITY_NEUTRAL"
|
|align="right" |1
|-
|align="left" |"MINOR_CIV_PERSONALITY_HOSTILE"
|
|align="right" |2
|-
|align="left" |"MINOR_CIV_PERSONALITY_IRRATIONAL"
|
|align="right" |3
|-
|align="left" |"NUM_MINOR_CIV_PERSONALITY_TYPES"
|
|align="right" |4
|}</code>


= Examples =
Here is how to use the LUA enumeration to retrieve the ''ID'' from the ''type''. Those examples will return and assign the integer value 0.
<syntaxhighlight lang="lua" class="civ5-example">
local id = MinorCivPersonalityTypes.MINOR_CIV_PERSONALITY_FRIENDLY
local id = MinorCivPersonalityTypes["MINOR_CIV_PERSONALITY_FRIENDLY"]
</syntaxhighlight>


=Used by=
{|cellspacing="4" cellpadding="0" width="100%" style="background-color:#F0F0F0"
<!-- 
GETPERSONALITY
-->
|-
|align="right" width="200" |<code>{{Type5|MinorCivPersonalityType}}</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|GetPersonality}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
SETPERSONALITYTYPE
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|SetPersonalityType}}<b>(</b>{{Type5|MinorCivPersonalityType}} newValue<b>)</b></code>
|}




{{Civ5 API Footer}}
[[Category:Civ5 Types|MinorCivPersonalityType]]