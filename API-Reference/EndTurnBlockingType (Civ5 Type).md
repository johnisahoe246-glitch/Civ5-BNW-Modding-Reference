{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|ID.png|The <code>EndTurnBlockingType</code> pseudo-type is actually a regular '''integer'''. Pseudo-types do not exist in Lua, they only serve a documentation purpose on the wiki!
* {{Lua}} Integers labeled as <code>EndTurnBlockingType</code> corresponds to the constants defined in the '''EndTurnBlockingTypes''' Lua enumeration.
}}


= Lua: the EndTurnBlockingTypes enumeration =
Firaxis provides a Lua enumeration named <code>EndTurnBlockingTypes</code>. This is just a regular global table. Its keys are the constants' names and the pairs the corresponding values.

<br/>Below are the values found in this enumeration.
<code>
{|
|-
!align="left" |Key
!
!align="left" |Value 
|-
|align="left" |"NO_ENDTURN_BLOCKING_TYPE"
|
|align="right" |-1
|-
|align="left" |"ENDTURN_BLOCKING_POLICY"
|
|align="right" |0
|-
|align="left" |"ENDTURN_BLOCKING_RESEARCH"
|
|align="right" |1
|-
|align="left" |"ENDTURN_BLOCKING_PRODUCTION"
|
|align="right" |2
|-
|align="left" |"ENDTURN_BLOCKING_UNITS"
|
|align="right" |3
|-
|align="left" |"ENDTURN_BLOCKING_DIPLO_VOTE"
|
|align="right" |4
|-
|align="left" |"ENDTURN_BLOCKING_MINOR_QUEST"
|
|align="right" |5
|-
|align="left" |"ENDTURN_BLOCKING_FREE_TECH"
|
|align="right" |6
|-
|align="left" |"ENDTURN_BLOCKING_STACKED_UNITS"
|
|align="right" |7
|-
|align="left" |"ENDTURN_BLOCKING_UNIT_NEEDS_ORDERS"
|
|align="right" |8
|-
|align="left" |"ENDTURN_BLOCKING_UNIT_PROMOTION"
|
|align="right" |9
|-
|align="left" |"ENDTURN_BLOCKING_CITY_RANGE_ATTACK"
|
|align="right" |10
|-
|align="left" |"ENDTURN_BLOCKING_FREE_POLICY"
|
|align="right" |11
|-
|align="left" |"ENDTURN_BLOCKING_FREE_ITEMS"
|
|align="right" |12
|-
|align="left" |"ENDTURN_BLOCKING_FOUND_PANTHEON"
|
|align="right" |13
|-
|align="left" |"ENDTURN_BLOCKING_FOUND_RELIGION"
|
|align="right" |14
|-
|align="left" |"ENDTURN_BLOCKING_ENHANCE_RELIGION"
|
|align="right" |15
|-
|align="left" |"ENDTURN_BLOCKING_STEAL_TECH"
|
|align="right" |16
|-
|align="left" |"ENDTURN_BLOCKING_MAYA_LONG_COUNT"
|
|align="right" |17
|-
|align="left" |"ENDTURN_BLOCKING_FAITH_GREAT_PERSON"
|
|align="right" |18
|-
|align="left" |"NUM_ENDTURN_BLOCKING_TYPES"
|
|align="right" |19
|}</code>


= Examples =
Here is how to use the LUA enumeration to retrieve the ''ID'' from the ''type''. Those examples will return and assign the integer value 0.
<syntaxhighlight lang="lua" class="civ5-example">
local id = EndTurnBlockingTypes.ENDTURN_BLOCKING_POLICY
local id = EndTurnBlockingTypes["ENDTURN_BLOCKING_POLICY"]
</syntaxhighlight>


=Used by=
{|cellspacing="4" cellpadding="0" width="100%" style="background-color:#F0F0F0"
<!-- 
ENDTURNBLOCKINGCHANGED
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Events}}.{{Func5|Events|EndTurnBlockingChanged}}<b>(</b>{{Type5|EndTurnBlockingType}} prevEndTurnBlockingType, {{Type5|EndTurnBlockingType}} newEndTurnBlockingType<b>)</b></code>
<!-- 
REGISTERCALLBACK
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Image}}:{{Func5|UIElement|RegisterCallback}}<b>(</b>{{Type5|MouseType}} arg0, ('''void''' func<b>(</b>{{Type5|EndTurnBlockingType}} Id<b>)</b>) OnEditNameClick<b>)</b></code>
<!-- 
GETENDTURNBLOCKINGNOTIFICATIONINDEX
-->
|-
|align="right" width="200" |<code>{{Type5|EndTurnBlockingType}}</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|GetEndTurnBlockingNotificationIndex}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETENDTURNBLOCKINGTYPE
-->
|-
|align="right" width="200" |<code>{{Type5|EndTurnBlockingType}}</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|GetEndTurnBlockingType}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETNOTIFICATIONINDEX
-->
|-
|align="right" width="200" |<code>{{Type5|EndTurnBlockingType}}</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|GetNotificationIndex}}<b>(</b>'''int''' i<b>)</b></code>
<!-- 
REGISTERCALLBACK
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Stack}}:{{Func5|UIElement|RegisterCallback}}<b>(</b>{{Type5|MouseType}} arg0, ('''void''' func<b>(</b>{{Type5|EndTurnBlockingType}} Id<b>)</b>) GenericLeftClick<b>)</b></code>
<!-- 
REMOVENOTIFICATION
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|UI}}.{{Func5|UI|RemoveNotification}}<b>(</b>{{Type5|EndTurnBlockingType}} blockingNotificationIndex<b>)</b></code>
|}




{{Civ5 API Footer}}
[[Category:Civ5 Types|EndTurnBlockingType]]