{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|ID.png|The <code>ActionSubType</code> pseudo-type is actually a regular '''integer'''. Pseudo-types do not exist in Lua, they only serve a documentation purpose on the wiki!
* {{Lua}} Integers labeled as <code>ActionSubType</code> corresponds to the constants defined in the '''ActionSubTypes''' Lua enumeration.
}}


= Lua: the ActionSubTypes enumeration =
Firaxis provides a Lua enumeration named <code>ActionSubTypes</code>. This is just a regular global table. Its keys are the constants' names and the pairs the corresponding values.

<br/>Below are the values found in this enumeration.
<code>
{|
|-
!align="left" |Key
!
!align="left" |Value 
|-
|align="left" |"ACTIONSUBTYPE_INTERFACEMODE"
|
|align="right" |0
|-
|align="left" |"ACTIONSUBTYPE_COMMAND"
|
|align="right" |1
|-
|align="left" |"ACTIONSUBTYPE_BUILD"
|
|align="right" |2
|-
|align="left" |"ACTIONSUBTYPE_PROMOTION"
|
|align="right" |3
|-
|align="left" |"ACTIONSUBTYPE_SPECIALIST"
|
|align="right" |4
|-
|align="left" |"ACTIONSUBTYPE_CONTROL"
|
|align="right" |5
|-
|align="left" |"ACTIONSUBTYPE_AUTOMATE"
|
|align="right" |6
|-
|align="left" |"ACTIONSUBTYPE_MISSION"
|
|align="right" |7
|-
|align="left" |"NUM_ACTIONSUBTYPES"
|
|align="right" |8
|}</code>


= Examples =
Here is how to use the LUA enumeration to retrieve the ''ID'' from the ''type''. Those examples will return and assign the integer value 0.
<syntaxhighlight lang="lua" class="civ5-example">
local id = ActionSubTypes.ACTIONSUBTYPE_INTERFACEMODE
local id = ActionSubTypes["ACTIONSUBTYPE_INTERFACEMODE"]
</syntaxhighlight>




{{Civ5 API Footer}}
[[Category:Civ5 Types|ActionSubType]]