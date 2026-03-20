{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|ID.png|The <code>KeyEventType</code> pseudo-type is actually a regular '''integer'''. Pseudo-types do not exist in Lua, they only serve a documentation purpose on the wiki!
* {{Lua}} Integers labeled as <code>KeyEventType</code> corresponds to the constants defined in the '''KeyEvents''' Lua enumeration.
}}


= Lua: the KeyEvents enumeration =
Firaxis provides a Lua enumeration named <code>KeyEvents</code>. This is just a regular global table. Its keys are the constants' names and the pairs the corresponding values.

<br/>Below are the values found in this enumeration.
<code>
{|
|-
!align="left" |Key
!
!align="left" |Value 
|-
|align="left" |"KeyDown"
|
|align="right" |256
|-
|align="left" |"WM_KEYDOWN"
|
|align="right" |256
|-
|align="left" |"WM_KEYUP"
|
|align="right" |257
|-
|align="left" |"KeyUp"
|
|align="right" |257
|}</code>


= Examples =
Here is how to use the LUA enumeration to retrieve the ''ID'' from the ''type''. Those examples will return and assign the integer value 256.
<syntaxhighlight lang="lua" class="civ5-example">
local id = KeyEvents.KeyDown
local id = KeyEvents["KeyDown"]
</syntaxhighlight>


=Used by=
{|cellspacing="4" cellpadding="0" width="100%" style="background-color:#F0F0F0"
<!-- 
DEBUGKEYHANDLER
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|UI}}.{{Func5|UI|DebugKeyHandler}}<b>(</b>{{Type5|KeyEventType}} uiMsg, {{Type5|KeyType}} wParam, '''unknown''' lParam<b>)</b></code>
|}




{{Civ5 API Footer}}
[[Category:Civ5 Types|KeyEventType]]