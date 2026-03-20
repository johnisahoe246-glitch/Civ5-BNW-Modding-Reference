{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|ID.png|The <code>CityAIFocusType</code> pseudo-type is actually a regular '''integer'''. Pseudo-types do not exist in Lua, they only serve a documentation purpose on the wiki!
* {{Lua}} Integers labeled as <code>CityAIFocusType</code> corresponds to the constants defined in the '''CityAIFocusTypes''' Lua enumeration.
}}


= Lua: the CityAIFocusTypes enumeration =
Firaxis provides a Lua enumeration named <code>CityAIFocusTypes</code>. This is just a regular global table. Its keys are the constants' names and the pairs the corresponding values.

<br/>Below are the values found in this enumeration.
<code>
{|
|-
!align="left" |Key
!
!align="left" |Value 
|-
|align="left" |"NO_CITY_AI_FOCUS_TYPE"
|
|align="right" |-1
|-
|align="left" |"CITY_AI_FOCUS_TYPE_FOOD"
|
|align="right" |0
|-
|align="left" |"CITY_AI_FOCUS_TYPE_PRODUCTION"
|
|align="right" |1
|-
|align="left" |"CITY_AI_FOCUS_TYPE_GOLD"
|
|align="right" |2
|-
|align="left" |"CITY_AI_FOCUS_TYPE_GREAT_PEOPLE"
|
|align="right" |3
|-
|align="left" |"CITY_AI_FOCUS_TYPE_SCIENCE"
|
|align="right" |4
|-
|align="left" |"CITY_AI_FOCUS_TYPE_CULTURE"
|
|align="right" |5
|-
|align="left" |"CITY_AI_FOCUS_TYPE_PROD_GROWTH"
|
|align="right" |6
|-
|align="left" |"CITY_AI_FOCUS_TYPE_GOLD_GROWTH"
|
|align="right" |7
|-
|align="left" |"CITY_AI_FOCUS_TYPE_FAITH"
|
|align="right" |8
|-
|align="left" |"NUM_CITY_AI_FOCUS_TYPES"
|
|align="right" |9
|}</code>


= Examples =
Here is how to use the LUA enumeration to retrieve the ''ID'' from the ''type''. Those examples will return and assign the integer value 0.
<syntaxhighlight lang="lua" class="civ5-example">
local id = CityAIFocusTypes.CITY_AI_FOCUS_TYPE_FOOD
local id = CityAIFocusTypes["CITY_AI_FOCUS_TYPE_FOOD"]
</syntaxhighlight>


=Used by=
{|cellspacing="4" cellpadding="0" width="100%" style="background-color:#F0F0F0"
<!-- 
GETFOCUSTYPE
-->
|-
|align="right" width="200" |<code>{{Type5|CityAIFocusType}}</code>
|style="padding-left:6px" |<code>{{Type5|City}}:{{Func5|City|GetFocusType}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
NOTIFICATIONADDED
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Events}}.{{Func5|Events|NotificationAdded}}<b>(</b>{{Type5|CityAIFocusType}} notification, {{Type5|NotificationType}} notificationType, '''string''' toolTip, '''string''' summary, '''int''' gameValue, {{Type5|TechType}} extraGameData<b>)</b></code>
<!-- 
NOTIFICATIONREMOVED
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Events}}.{{Func5|Events|NotificationRemoved}}<b>(</b>{{Type5|CityAIFocusType}} <b>)</b></code>
<!-- 
SETVOID1
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Image}}:{{Func5|UIElement|SetVoid1}}<b>(</b>{{Type5|CityAIFocusType}} <b>)</b></code>
|}




{{Civ5 API Footer}}
[[Category:Civ5 Types|CityAIFocusType]]