{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|ID.png|The <code>ButtonState</code> pseudo-type is actually a regular '''integer'''. Pseudo-types do not exist in Lua, they only serve a documentation purpose on the wiki!
* {{Lua}} Integers labeled as <code>ButtonState</code> corresponds to the constants defined in the '''ButtonStates''' Lua enumeration.
}}


= Lua: the ButtonStates enumeration =
Firaxis provides a Lua enumeration named <code>ButtonStates</code>. This is just a regular global table. Its keys are the constants' names and the pairs the corresponding values.

<br/>Below are the values found in this enumeration.
<code>
{|
|-
!align="left" |Key
!
!align="left" |Value 
|-
|align="left" |"eNormal"
|
|align="right" |0
|-
|align="left" |"eMouseOver"
|
|align="right" |1
|-
|align="left" |"eMouseDown"
|
|align="right" |2
|-
|align="left" |"eDisabled"
|
|align="right" |3
|}</code>


= Examples =
Here is how to use the LUA enumeration to retrieve the ''ID'' from the ''type''. Those examples will return and assign the integer value 0.
<syntaxhighlight lang="lua" class="civ5-example">
local id = ButtonStates.eNormal
local id = ButtonStates["eNormal"]
</syntaxhighlight>




{{Civ5 API Footer}}
[[Category:Civ5 Types|ButtonState]]