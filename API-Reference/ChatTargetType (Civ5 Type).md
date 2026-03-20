{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|ID.png|The <code>ChatTargetType</code> pseudo-type is actually a regular '''integer'''. Pseudo-types do not exist in Lua, they only serve a documentation purpose on the wiki!
* {{Lua}} Integers labeled as <code>ChatTargetType</code> corresponds to the constants defined in the '''ChatTargetTypes''' Lua enumeration.
}}


= Lua: the ChatTargetTypes enumeration =
Firaxis provides a Lua enumeration named <code>ChatTargetTypes</code>. This is just a regular global table. Its keys are the constants' names and the pairs the corresponding values.

<br/>Below are the values found in this enumeration.
<code>
{|
|-
!align="left" |Key
!
!align="left" |Value 
|-
|align="left" |"CHATTARGET_PLAYER"
|
|align="right" |-4
|-
|align="left" |"CHATTARGET_TEAM"
|
|align="right" |-3
|-
|align="left" |"CHATTARGET_ALL"
|
|align="right" |-2
|-
|align="left" |"NO_CHATTARGET"
|
|align="right" |-1
|}</code>


= Examples =
Here is how to use the LUA enumeration to retrieve the ''ID'' from the ''type''. Those examples will return and assign the integer value -4.
<syntaxhighlight lang="lua" class="civ5-example">
local id = ChatTargetTypes.CHATTARGET_PLAYER
local id = ChatTargetTypes["CHATTARGET_PLAYER"]
</syntaxhighlight>


=Used by=
{|cellspacing="4" cellpadding="0" width="100%" style="background-color:#F0F0F0"
<!-- 
GAMEMESSAGECHAT
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Events}}.{{Func5|Events|GameMessageChat}}<b>(</b>{{Type5|PlayerID}} fromPlayer, {{Type5|PlayerID}} toPlayer, '''string''' text, {{Type5|ChatTargetType}} targetType<b>)</b></code>
|}




{{Civ5 API Footer}}
[[Category:Civ5 Types|ChatTargetType]]