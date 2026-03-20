{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|ID.png|The <code>ThreatType</code> pseudo-type is actually a regular '''integer'''. Pseudo-types do not exist in Lua, they only serve a documentation purpose on the wiki!
* {{Lua}} Integers labeled as <code>ThreatType</code> corresponds to the constants defined in the '''ThreatTypes''' Lua enumeration.
}}


= Lua: the ThreatTypes enumeration =
Firaxis provides a Lua enumeration named <code>ThreatTypes</code>. This is just a regular global table. Its keys are the constants' names and the pairs the corresponding values.

<br/>Below are the values found in this enumeration.
<code>
{|
|-
!align="left" |Key
!
!align="left" |Value 
|-
|align="left" |"NO_THREAT_VALUE"
|
|align="right" |-1
|-
|align="left" |"THREAT_NONE"
|
|align="right" |0
|-
|align="left" |"THREAT_MINOR"
|
|align="right" |1
|-
|align="left" |"THREAT_MAJOR"
|
|align="right" |2
|-
|align="left" |"THREAT_SEVERE"
|
|align="right" |3
|-
|align="left" |"THREAT_CRITICAL"
|
|align="right" |4
|-
|align="left" |"NUM_THREAT_VALUES"
|
|align="right" |5
|}</code>


= Examples =
Here is how to use the LUA enumeration to retrieve the ''ID'' from the ''type''. Those examples will return and assign the integer value 0.
<syntaxhighlight lang="lua" class="civ5-example">
local id = ThreatTypes.THREAT_NONE
local id = ThreatTypes["THREAT_NONE"]
</syntaxhighlight>


=Used by=
{|cellspacing="4" cellpadding="0" width="100%" style="background-color:#F0F0F0"
<!-- 
GETWARMONGERTHREAT
-->
|-
|align="right" width="200" |<code>{{Type5|ThreatType}}</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|GetWarmongerThreat}}<b>(</b>{{Type5|PlayerID}} activePlayer<b>)</b></code>
|}




{{Civ5 API Footer}}
[[Category:Civ5 Types|ThreatType]]