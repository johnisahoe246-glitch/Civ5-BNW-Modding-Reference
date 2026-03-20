{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|ID.png|The <code>TaskType</code> pseudo-type is actually a regular '''integer'''. Pseudo-types do not exist in Lua, they only serve a documentation purpose on the wiki!
* {{Lua}} Integers labeled as <code>TaskType</code> corresponds to the constants defined in the '''TaskTypes''' Lua enumeration.
}}


= Lua: the TaskTypes enumeration =
Firaxis provides a Lua enumeration named <code>TaskTypes</code>. This is just a regular global table. Its keys are the constants' names and the pairs the corresponding values.

<br/>Below are the values found in this enumeration.
<code>
{|
|-
!align="left" |Key
!
!align="left" |Value 
|-
|align="left" |"TASK_RAZE"
|
|align="right" |0
|-
|align="left" |"TASK_UNRAZE"
|
|align="right" |1
|-
|align="left" |"TASK_DISBAND"
|
|align="right" |2
|-
|align="left" |"TASK_GIFT"
|
|align="right" |3
|-
|align="left" |"TASK_SET_AUTOMATED_CITIZENS"
|
|align="right" |4
|-
|align="left" |"TASK_SET_AUTOMATED_PRODUCTION"
|
|align="right" |5
|-
|align="left" |"TASK_SET_EMPHASIZE"
|
|align="right" |6
|-
|align="left" |"TASK_NO_AUTO_ASSIGN_SPECIALISTS"
|
|align="right" |7
|-
|align="left" |"TASK_ADD_SPECIALIST"
|
|align="right" |8
|-
|align="left" |"TASK_REMOVE_SPECIALIST"
|
|align="right" |9
|-
|align="left" |"TASK_CHANGE_WORKING_PLOT"
|
|align="right" |10
|-
|align="left" |"TASK_CLEAR_WORKING_OVERRIDE"
|
|align="right" |11
|-
|align="left" |"TASK_HURRY"
|
|align="right" |12
|-
|align="left" |"TASK_CONSCRIPT"
|
|align="right" |13
|-
|align="left" |"TASK_CLEAR_ORDERS"
|
|align="right" |14
|-
|align="left" |"TASK_RALLY_PLOT"
|
|align="right" |15
|-
|align="left" |"TASK_CLEAR_RALLY_PLOT"
|
|align="right" |16
|-
|align="left" |"TASK_RANGED_ATTACK"
|
|align="right" |17
|-
|align="left" |"TASK_CREATE_PUPPET"
|
|align="right" |18
|-
|align="left" |"TASK_ANNEX_PUPPET"
|
|align="right" |19
|-
|align="left" |"NUM_TASK_TYPES"
|
|align="right" |20
|}</code>


= Examples =
Here is how to use the LUA enumeration to retrieve the ''ID'' from the ''type''. Those examples will return and assign the integer value 0.
<syntaxhighlight lang="lua" class="civ5-example">
local id = TaskTypes.TASK_RAZE
local id = TaskTypes["TASK_RAZE"]
</syntaxhighlight>


=Used by=
{|cellspacing="4" cellpadding="0" width="100%" style="background-color:#F0F0F0"
<!-- 
DOTASK
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|City}}:{{Func5|City|DoTask}}<b>(</b>{{Type5|TaskType}} task, '''int''' data1, '''int''' data2, '''bool''' option<b>)</b></code>
<!-- 
DOMINORGIFTTILEIMPROVEMENT
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Game}}.{{Func5|Game|DoMinorGiftTileImprovement}}<b>(</b>{{Type5|PlayerID}} fromPlayer, {{Type5|TaskType}} toPlayer, '''int''' plotX, '''int''' plotY<b>)</b></code>
<!-- 
SELECTEDCITIESGAMENETMESSAGE
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Game}}.{{Func5|Game|SelectedCitiesGameNetMessage}}<b>(</b>{{Type5|GameMessageType}} message, {{Type5|TaskType}} data2, '''int''' data3, {{Type5|BuildingType}} data4, '''bool''' option, '''bool''' alt, '''bool''' shift, '''bool''' ctrl<b>)</b></code>
<!-- 
SENDDOTASK
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Network}}.{{Func5|Network|SendDoTask}}<b>(</b>{{Type5|CityID}} cityID, {{Type5|TaskType}} task, '''int''' plotIndex, '''int''' arg3, '''bool''' arg4, '''bool''' alt, '''bool''' shift, '''bool''' ctrl<b>)</b></code>
<!-- 
SENDSETCITYAIFOCUS
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Network}}.{{Func5|Network|SendSetCityAIFocus}}<b>(</b>{{Type5|CityID}} arg0, {{Type5|TaskType}} focus<b>)</b></code>
<!-- 
GETINTERFACEMODEVALUE
-->
|-
|align="right" width="200" |<code>{{Type5|TaskType}}</code>
|style="padding-left:6px" |<code>{{Type5|UI}}.{{Func5|UI|GetInterfaceModeValue}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
CANDISTANCEGIFT
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|Unit}}:{{Func5|Unit|CanDistanceGift}}<b>(</b>{{Type5|TaskType}} toPlayer<b>)</b></code>
|}




{{Civ5 API Footer}}
[[Category:Civ5 Types|TaskType]]