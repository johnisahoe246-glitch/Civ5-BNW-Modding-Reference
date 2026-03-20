{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|ID.png|The <code>OrderType</code> pseudo-type is actually a regular '''integer'''. Pseudo-types do not exist in Lua, they only serve a documentation purpose on the wiki!
* {{Lua}} Integers labeled as <code>OrderType</code> corresponds to the constants defined in the '''OrderTypes''' Lua enumeration.
}}


= Lua: the OrderTypes enumeration =
Firaxis provides a Lua enumeration named <code>OrderTypes</code>. This is just a regular global table. Its keys are the constants' names and the pairs the corresponding values.

<br/>Below are the values found in this enumeration.
<code>
{|
|-
!align="left" |Key
!
!align="left" |Value 
|-
|align="left" |"NO_ORDER"
|
|align="right" |-1
|-
|align="left" |"ORDER_TRAIN"
|
|align="right" |0
|-
|align="left" |"ORDER_CONSTRUCT"
|
|align="right" |1
|-
|align="left" |"ORDER_CREATE"
|
|align="right" |2
|-
|align="left" |"ORDER_PREPARE"
|
|align="right" |3
|-
|align="left" |"ORDER_MAINTAIN"
|
|align="right" |4
|-
|align="left" |"NUM_ORDER_TYPES"
|
|align="right" |5
|}</code>


= Examples =
Here is how to use the LUA enumeration to retrieve the ''ID'' from the ''type''. Those examples will return and assign the integer value 0.
<syntaxhighlight lang="lua" class="civ5-example">
local id = OrderTypes.ORDER_TRAIN
local id = OrderTypes["ORDER_TRAIN"]
</syntaxhighlight>


=Used by=
{|cellspacing="4" cellpadding="0" width="100%" style="background-color:#F0F0F0"
<!-- 
CANCONTINUEPRODUCTION
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|City}}:{{Func5|City|CanContinueProduction}}<b>(</b>{{Type5|OrderType}} orderType, '''int''' data1, '''int''' data2, '''bool''' save<b>)</b></code>
<!-- 
GETORDERFROMQUEUE
-->
|-
|align="right" width="200" |<code>{{Type5|OrderType}}, '''int''', '''unknown''', '''unknown''', '''unknown'''</code>
|style="padding-left:6px" |<code>{{Type5|City}}:{{Func5|City|GetOrderFromQueue}}<b>(</b>'''int''' arg0<b>)</b></code>
<!-- 
PUSHORDER
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|City}}:{{Func5|City|PushOrder}}<b>(</b>{{Type5|OrderType}} order, '''int''' data1, '''int''' data2, '''bool''' save, '''bool''' pop, '''bool''' append, '''bool''' force<b>)</b></code>
<!-- 
CITYPUSHORDER
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Game}}.{{Func5|Game|CityPushOrder}}<b>(</b>{{Type5|City}} city, {{Type5|OrderType}} order, {{Type5|UnitType}} data, '''bool''' alt, '''bool''' shift, '''bool''' ctrl<b>)</b></code>
<!-- 
SETVOID1
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|TextButton}}:{{Func5|UIElement|SetVoid1}}<b>(</b>{{Type5|OrderType}} MAINTAIN_GOLD<b>)</b></code>
|}




{{Civ5 API Footer}}
[[Category:Civ5 Types|OrderType]]