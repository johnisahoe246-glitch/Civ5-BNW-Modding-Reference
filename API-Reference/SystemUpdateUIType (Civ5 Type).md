{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|ID.png|The <code>SystemUpdateUIType</code> pseudo-type is actually a regular '''integer'''. Pseudo-types do not exist in Lua, they only serve a documentation purpose on the wiki!
* {{Lua}} Integers labeled as <code>SystemUpdateUIType</code> corresponds to the constants defined in the '''SystemUpdateUIType''' Lua enumeration.
}}


= Lua: the SystemUpdateUIType enumeration =
Firaxis provides a Lua enumeration named <code>SystemUpdateUIType</code>. This is just a regular global table. Its keys are the constants' names and the pairs the corresponding values.

<br/>Below are the values found in this enumeration.
<code>
{|
|-
!align="left" |Key
!
!align="left" |Value 
|-
|align="left" |"ScreenResize"
|
|align="right" |0
|-
|align="left" |"ReloadUI"
|
|align="right" |1
|-
|align="left" |"ReprocessAnchoring"
|
|align="right" |2
|-
|align="left" |"BulkHideUI"
|
|align="right" |3
|-
|align="left" |"BulkShowUI"
|
|align="right" |4
|}</code>


= Examples =
Here is how to use the LUA enumeration to retrieve the ''ID'' from the ''type''. Those examples will return and assign the integer value 0.
<syntaxhighlight lang="lua" class="civ5-example">
local id = SystemUpdateUIType.ScreenResize
local id = SystemUpdateUIType["ScreenResize"]
</syntaxhighlight>


=Used by=
{|cellspacing="4" cellpadding="0" width="100%" style="background-color:#F0F0F0"
<!-- 
SYSTEMUPDATEUI
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Events}}.{{Func5|Events|SystemUpdateUI}}<b>(</b>{{Type5|SystemUpdateUIType}} type<b>)</b></code>
|}




{{Civ5 API Footer}}
[[Category:Civ5 Types|SystemUpdateUIType]]