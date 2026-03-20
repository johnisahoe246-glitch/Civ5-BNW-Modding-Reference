{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|ID.png|The <code>MouseEventType</code> pseudo-type is actually a regular '''integer'''. Pseudo-types do not exist in Lua, they only serve a documentation purpose on the wiki!
* {{Lua}} Integers labeled as <code>MouseEventType</code> corresponds to the constants defined in the '''MouseEvents''' Lua enumeration.
}}


= Lua: the MouseEvents enumeration =
Firaxis provides a Lua enumeration named <code>MouseEvents</code>. This is just a regular global table. Its keys are the constants' names and the pairs the corresponding values.

<br/>Below are the values found in this enumeration.
<code>
{|
|-
!align="left" |Key
!
!align="left" |Value 
|-
|align="left" |"MouseMove"
|
|align="right" |512
|-
|align="left" |"MouseFirst"
|
|align="right" |512
|-
|align="left" |"LButtonDown"
|
|align="right" |513
|-
|align="left" |"LButtonUp"
|
|align="right" |514
|-
|align="left" |"LButtonDoubleClick"
|
|align="right" |515
|-
|align="left" |"RButtonDown"
|
|align="right" |516
|-
|align="left" |"RButtonUp"
|
|align="right" |517
|-
|align="left" |"RButtonDoubleClick"
|
|align="right" |518
|-
|align="left" |"MButtonDown"
|
|align="right" |519
|-
|align="left" |"MButtonUp"
|
|align="right" |520
|-
|align="left" |"MButtonDoubleClick"
|
|align="right" |521
|-
|align="left" |"MouseWheel"
|
|align="right" |522
|-
|align="left" |"XButtonDown"
|
|align="right" |523
|-
|align="left" |"XButtonUp"
|
|align="right" |524
|-
|align="left" |"MouseLast"
|
|align="right" |525
|-
|align="left" |"XButtonDoubleClick"
|
|align="right" |525
|}</code>


= Examples =
Here is how to use the LUA enumeration to retrieve the ''ID'' from the ''type''. Those examples will return and assign the integer value 512.
<syntaxhighlight lang="lua" class="civ5-example">
local id = MouseEvents.MouseMove
local id = MouseEvents["MouseMove"]
</syntaxhighlight>


=Used by=
{|cellspacing="4" cellpadding="0" width="100%" style="background-color:#F0F0F0"
<!-- 
SETINPUTHANDLER
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Context}}:{{Func5|UIElement|SetInputHandler}}<b>(</b>('''void''' func<b>(</b>{{Type5|MouseEventType}} uiMsg, {{Type5|KeyType}} wParam, '''unknown''' lParam<b>)</b>) InputHandler<b>)</b></code>
|}




{{Civ5 API Footer}}
[[Category:Civ5 Types|MouseEventType]]