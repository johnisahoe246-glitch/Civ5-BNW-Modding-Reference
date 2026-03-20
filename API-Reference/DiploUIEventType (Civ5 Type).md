{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|ID.png|The <code>DiploUIEventType</code> pseudo-type is actually a regular '''integer'''. Pseudo-types do not exist in Lua, they only serve a documentation purpose on the wiki!
* {{Lua}} Integers labeled as <code>DiploUIEventType</code> corresponds to the constants defined in the '''FromUIDiploEventTypes''' Lua enumeration.
}}


= Lua: the FromUIDiploEventTypes enumeration =
Firaxis provides a Lua enumeration named <code>FromUIDiploEventTypes</code>. This is just a regular global table. Its keys are the constants' names and the pairs the corresponding values.

<br/>Below are the values found in this enumeration.
<code>
{|
|-
!align="left" |Key
!
!align="left" |Value 
|-
|align="left" |"NO_FROM_UI_DIPLO_EVENT"
|
|align="right" |-1
|-
|align="left" |"FROM_UI_DIPLO_EVENT_HUMAN_DECLARES_WAR"
|
|align="right" |0
|-
|align="left" |"FROM_UI_DIPLO_EVENT_HUMAN_NEGOTIATE_PEACE"
|
|align="right" |1
|-
|align="left" |"FROM_UI_DIPLO_EVENT_HUMAN_WANTS_DISCUSSION"
|
|align="right" |2
|-
|align="left" |"FROM_UI_DIPLO_EVENT_HUMAN_DISCUSSION_DONT_SETTLE"
|
|align="right" |3
|-
|align="left" |"FROM_UI_DIPLO_EVENT_HUMAN_DISCUSSION_WORK_WITH_US"
|
|align="right" |4
|-
|align="left" |"FROM_UI_DIPLO_EVENT_HUMAN_DISCUSSION_END_WORK_WITH_US"
|
|align="right" |5
|-
|align="left" |"FROM_UI_DIPLO_EVENT_DEMAND_HUMAN_REFUSAL"
|
|align="right" |6
|-
|align="left" |"FROM_UI_DIPLO_EVENT_REQUEST_HUMAN_REFUSAL"
|
|align="right" |7
|-
|align="left" |"FROM_UI_DIPLO_EVENT_AGGRESSIVE_MILITARY_WARNING_RESPONSE"
|
|align="right" |8
|-
|align="left" |"FROM_UI_DIPLO_EVENT_I_ATTACKED_YOUR_MINOR_CIV_RESPONSE"
|
|align="right" |9
|-
|align="left" |"FROM_UI_DIPLO_EVENT_I_BULLIED_YOUR_MINOR_CIV_RESPONSE"
|
|align="right" |10
|-
|align="left" |"FROM_UI_DIPLO_EVENT_ATTACKED_MINOR_RESPONSE"
|
|align="right" |11
|-
|align="left" |"FROM_UI_DIPLO_EVENT_KILLED_MINOR_RESPONSE"
|
|align="right" |12
|-
|align="left" |"FROM_UI_DIPLO_EVENT_BULLIED_MINOR_RESPONSE"
|
|align="right" |13
|-
|align="left" |"FROM_UI_DIPLO_EVENT_EXPANSION_SERIOUS_WARNING_RESPONSE"
|
|align="right" |14
|-
|align="left" |"FROM_UI_DIPLO_EVENT_EXPANSION_WARNING_RESPONSE"
|
|align="right" |15
|-
|align="left" |"FROM_UI_DIPLO_EVENT_PLOT_BUYING_SERIOUS_WARNING_RESPONSE"
|
|align="right" |16
|-
|align="left" |"FROM_UI_DIPLO_EVENT_PLOT_BUYING_WARNING_RESPONSE"
|
|align="right" |17
|-
|align="left" |"FROM_UI_DIPLO_EVENT_WORK_WITH_US_RESPONSE"
|
|align="right" |18
|-
|align="left" |"FROM_UI_DIPLO_EVENT_WORK_AGAINST_SOMEONE_RESPONSE"
|
|align="right" |19
|-
|align="left" |"FROM_UI_DIPLO_EVENT_DENOUNCE"
|
|align="right" |20
|-
|align="left" |"FROM_UI_DIPLO_EVENT_COOP_WAR_OFFER"
|
|align="right" |21
|-
|align="left" |"FROM_UI_DIPLO_EVENT_COOP_WAR_RESPONSE"
|
|align="right" |22
|-
|align="left" |"FROM_UI_DIPLO_EVENT_COOP_WAR_NOW_RESPONSE"
|
|align="right" |23
|-
|align="left" |"FROM_UI_DIPLO_EVENT_HUMAN_DEMAND"
|
|align="right" |24
|-
|align="left" |"FROM_UI_DIPLO_EVENT_PLAN_RA_RESPONSE"
|
|align="right" |25
|-
|align="left" |"FROM_UI_DIPLO_EVENT_AI_REQUEST_DENOUNCE_RESPONSE"
|
|align="right" |26
|-
|align="left" |"FROM_UI_DIPLO_EVENT_CAUGHT_YOUR_SPY_RESPONSE"
|
|align="right" |27
|-
|align="left" |"FROM_UI_DIPLO_EVENT_KILLED_MY_SPY_RESPONSE"
|
|align="right" |28
|-
|align="left" |"FROM_UI_DIPLO_EVENT_HUMAN_DISCUSSION_STOP_SPYING"
|
|align="right" |29
|-
|align="left" |"FROM_UI_DIPLO_EVENT_HUMAN_DISCUSSION_SHARE_INTRIGUE"
|
|align="right" |30
|-
|align="left" |"FROM_UI_DIPLO_EVENT_STOP_CONVERSIONS"
|
|align="right" |31
|-
|align="left" |"NUM_FROM_UI_DIPLO_EVENTS"
|
|align="right" |32
|}</code>


= Examples =
Here is how to use the LUA enumeration to retrieve the ''ID'' from the ''type''. Those examples will return and assign the integer value 0.
<syntaxhighlight lang="lua" class="civ5-example">
local id = FromUIDiploEventTypes.FROM_UI_DIPLO_EVENT_HUMAN_DECLARES_WAR
local id = FromUIDiploEventTypes["FROM_UI_DIPLO_EVENT_HUMAN_DECLARES_WAR"]
</syntaxhighlight>


=Used by=
{|cellspacing="4" cellpadding="0" width="100%" style="background-color:#F0F0F0"
<!-- 
DOFROMUIDIPLOEVENT
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Game}}.{{Func5|Game|DoFromUIDiploEvent}}<b>(</b>{{Type5|DiploUIEventType}} event, {{Type5|PlayerID}} aIPlayer, {{Type5|SpecialistType}} button, '''int''' againstPlayer, '''int''' arg3<b>)</b></code>
|}




{{Civ5 API Footer}}
[[Category:Civ5 Types|DiploUIEventType]]