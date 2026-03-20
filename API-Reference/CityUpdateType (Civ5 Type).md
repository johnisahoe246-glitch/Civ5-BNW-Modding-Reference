{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|ID.png|The <code>CityUpdateType</code> pseudo-type is actually a regular '''integer'''. Pseudo-types do not exist in Lua, they only serve a documentation purpose on the wiki!
* {{Lua}} Integers labeled as <code>CityUpdateType</code> corresponds to the constants defined in the '''CityUpdateTypes''' Lua enumeration.
}}


= Lua: the CityUpdateTypes enumeration =
Firaxis provides a Lua enumeration named <code>CityUpdateTypes</code>. This is just a regular global table. Its keys are the constants' names and the pairs the corresponding values.

<br/>Below are the values found in this enumeration.
<code>
{|
|-
!align="left" |Key
!
!align="left" |Value 
|-
|align="left" |"NO_CITY_UPDATE_TYPE"
|
|align="right" |-1
|-
|align="left" |"CITY_UPDATE_TYPE_BANNER"
|
|align="right" |0
|-
|align="left" |"CITY_UPDATE_TYPE_SPECIALISTS"
|
|align="right" |1
|-
|align="left" |"CITY_UPDATE_TYPE_PRODUCTION"
|
|align="right" |2
|-
|align="left" |"CITY_UPDATE_TYPE_ENEMY_IN_RANGE"
|
|align="right" |3
|-
|align="left" |"NUM_CITY_UPDATE_TYPES"
|
|align="right" |4
|}</code>


= Examples =
Here is how to use the LUA enumeration to retrieve the ''ID'' from the ''type''. Those examples will return and assign the integer value 0.
<syntaxhighlight lang="lua" class="civ5-example">
local id = CityUpdateTypes.CITY_UPDATE_TYPE_BANNER
local id = CityUpdateTypes["CITY_UPDATE_TYPE_BANNER"]
</syntaxhighlight>


=Used by=
{|cellspacing="4" cellpadding="0" width="100%" style="background-color:#F0F0F0"
<!-- 
SPECIFICCITYINFODIRTY
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Events}}.{{Func5|Events|SpecificCityInfoDirty}}<b>(</b>{{Type5|PlayerID}} player, {{Type5|CityID}} cityID, {{Type5|CityUpdateType}} updateType<b>)</b></code>
|}




{{Civ5 API Footer}}
[[Category:Civ5 Types|CityUpdateType]]