{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|ID.png|The <code>YieldDisplayType</code> pseudo-type is actually a regular '''integer'''. Pseudo-types do not exist in Lua, they only serve a documentation purpose on the wiki!
* {{Lua}} Integers labeled as <code>YieldDisplayType</code> corresponds to the constants defined in the '''YieldDisplayTypes''' Lua enumeration.
}}


= Lua: the YieldDisplayTypes enumeration =
Firaxis provides a Lua enumeration named <code>YieldDisplayTypes</code>. This is just a regular global table. Its keys are the constants' names and the pairs the corresponding values.

<br/>Below are the values found in this enumeration.
<code>
{|
|-
!align="left" |Key
!
!align="left" |Value 
|-
|align="left" |"USER_ALL_ON"
|
|align="right" |0
|-
|align="left" |"USER_ALL_OFF"
|
|align="right" |1
|-
|align="left" |"USER_ALL_RESOURCE_ON"
|
|align="right" |2
|-
|align="left" |"USER_ALL_RESOURCE_OFF"
|
|align="right" |3
|-
|align="left" |"EMPIRE"
|
|align="right" |4
|-
|align="left" |"CITY_OWNED"
|
|align="right" |5
|-
|align="left" |"CITY_WORKED"
|
|align="right" |6
|-
|align="left" |"CITY_PURCHASABLE"
|
|align="right" |7
|-
|align="left" |"AREA"
|
|align="right" |8
|}</code>


= Examples =
Here is how to use the LUA enumeration to retrieve the ''ID'' from the ''type''. Those examples will return and assign the integer value 0.
<syntaxhighlight lang="lua" class="civ5-example">
local id = YieldDisplayTypes.USER_ALL_ON
local id = YieldDisplayTypes["USER_ALL_ON"]
</syntaxhighlight>


=Used by=
{|cellspacing="4" cellpadding="0" width="100%" style="background-color:#F0F0F0"
<!-- 
REQUESTYIELDDISPLAY
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Events}}.{{Func5|Events|RequestYieldDisplay}}<b>(</b>{{Type5|YieldDisplayType}} type, {{Type5|ResourceType}} arg1 = nil, {{Type5|ResourceType}} gridX = nil, '''int''' gridY = nil<b>)</b></code>
|}




{{Civ5 API Footer}}
[[Category:Civ5 Types|YieldDisplayType]]