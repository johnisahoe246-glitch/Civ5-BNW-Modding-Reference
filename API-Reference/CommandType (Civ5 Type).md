{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|ID.png|The <code>CommandType</code> pseudo-type is actually a regular '''integer'''. Pseudo-types do not exist in Lua, they only serve a documentation purpose on the wiki!
* {{Lua}} Integers labeled as <code>CommandType</code> corresponds to the constants defined in the '''CommandTypes''' Lua enumeration.
}}


= Lua: the CommandTypes enumeration =
Firaxis provides a Lua enumeration named <code>CommandTypes</code>. This is just a regular global table. Its keys are the constants' names and the pairs the corresponding values.

<br/>Below are the values found in this enumeration.
<code>
{|
|-
!align="left" |Key
!
!align="left" |Value 
|-
|align="left" |"COMMAND_PROMOTION"
|
|align="right" |0
|-
|align="left" |"COMMAND_UPGRADE"
|
|align="right" |1
|-
|align="left" |"COMMAND_AUTOMATE"
|
|align="right" |2
|-
|align="left" |"COMMAND_WAKE"
|
|align="right" |3
|-
|align="left" |"COMMAND_CANCEL"
|
|align="right" |4
|-
|align="left" |"COMMAND_CANCEL_ALL"
|
|align="right" |5
|-
|align="left" |"COMMAND_STOP_AUTOMATION"
|
|align="right" |6
|-
|align="left" |"COMMAND_DELETE"
|
|align="right" |7
|-
|align="left" |"COMMAND_GIFT"
|
|align="right" |8
|-
|align="left" |"COMMAND_HOTKEY"
|
|align="right" |9
|-
|align="left" |"NUM_COMMAND_TYPES"
|
|align="right" |10
|}</code>


= Examples =
Here is how to use the LUA enumeration to retrieve the ''ID'' from the ''type''. Those examples will return and assign the integer value 0.
<syntaxhighlight lang="lua" class="civ5-example">
local id = CommandTypes.COMMAND_PROMOTION
local id = CommandTypes["COMMAND_PROMOTION"]
</syntaxhighlight>


=Used by=
{|cellspacing="4" cellpadding="0" width="100%" style="background-color:#F0F0F0"
<!-- 
CANDOCOMMAND
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|Unit}}:{{Func5|Unit|CanDoCommand}}<b>(</b>{{Type5|CommandType}} command, '''int''' data1, '''int''' data2, '''bool''' testVisible = false, '''bool''' testBusy = true<b>)</b></code>
<!-- 
DOCOMMAND
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Unit}}:{{Func5|Unit|DoCommand}}<b>(</b>{{Type5|CommandType}} command, '''int''' data1, '''int''' data2<b>)</b></code>
|}




{{Civ5 API Footer}}
[[Category:Civ5 Types|CommandType]]