{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|ID.png|The <code>ContentType</code> pseudo-type is actually a regular '''integer'''. Pseudo-types do not exist in Lua, they only serve a documentation purpose on the wiki!
* {{Lua}} Integers labeled as <code>ContentType</code> corresponds to the constants defined in the '''ContentType''' Lua enumeration.
}}


= Lua: the ContentType enumeration =
Firaxis provides a Lua enumeration named <code>ContentType</code>. This is just a regular global table. Its keys are the constants' names and the pairs the corresponding values.

<br/>Below are the values found in this enumeration.
<code>
{|
|-
!align="left" |Key
!
!align="left" |Value 
|-
|align="left" |"COMMON"
|
|align="right" |0
|-
|align="left" |"GAMEPLAY"
|
|align="right" |1
|-
|align="left" |"UISKIN"
|
|align="right" |2
|}</code>


= Examples =
Here is how to use the LUA enumeration to retrieve the ''ID'' from the ''type''. Those examples will return and assign the integer value 0.
<syntaxhighlight lang="lua" class="civ5-example">
local id = ContentType.COMMON
local id = ContentType["COMMON"]
</syntaxhighlight>


=Used by=
{|cellspacing="4" cellpadding="0" width="100%" style="background-color:#F0F0F0"
<!-- 
ISACTIVE
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|ContentManager}}.{{Func5|ContentManager|IsActive}}<b>(</b>'''string''' v, {{Type5|ContentType}} arg1<b>)</b></code>
|}




{{Civ5 API Footer}}
[[Category:Civ5 Types|ContentType]]