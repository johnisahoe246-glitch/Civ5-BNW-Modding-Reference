{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|ID.png|The <code>DiploUIStateType</code> pseudo-type is actually a regular '''integer'''. Pseudo-types do not exist in Lua, they only serve a documentation purpose on the wiki!
* {{Lua}} Integers labeled as <code>DiploUIStateType</code> corresponds to the constants defined in the '''DiploUIStateTypes''' Lua enumeration.
}}


= Lua: the DiploUIStateTypes enumeration =
Firaxis provides a Lua enumeration named <code>DiploUIStateTypes</code>. This is just a regular global table. Its keys are the constants' names and the pairs the corresponding values.

<br/>Below are the values found in this enumeration.
<code>
{|
|-
!align="left" |Key
!
!align="left" |Value 
|-
|align="left" |"NO_DIPLO_UI_STATE"
|
|align="right" |-1
|-
|align="left" |"DIPLO_UI_STATE_DEFAULT_ROOT"
|
|align="right" |0
|-
|align="left" |"DIPLO_UI_STATE_WAR_DECLARED_BY_HUMAN"
|
|align="right" |1
|-
|align="left" |"DIPLO_UI_STATE_PEACE_MADE_BY_HUMAN"
|
|align="right" |2
|-
|align="left" |"DIPLO_UI_STATE_TRADE"
|
|align="right" |3
|-
|align="left" |"DIPLO_UI_STATE_TRADE_AI_MAKES_OFFER"
|
|align="right" |4
|-
|align="left" |"DIPLO_UI_STATE_TRADE_AI_ACCEPTS_OFFER"
|
|align="right" |5
|-
|align="left" |"DIPLO_UI_STATE_TRADE_AI_REJECTS_OFFER"
|
|align="right" |6
|-
|align="left" |"DIPLO_UI_STATE_TRADE_AI_MAKES_DEMAND"
|
|align="right" |7
|-
|align="left" |"DIPLO_UI_STATE_TRADE_AI_MAKES_REQUEST"
|
|align="right" |8
|-
|align="left" |"DIPLO_UI_STATE_TRADE_HUMAN_OFFERS_CONCESSIONS"
|
|align="right" |9
|-
|align="left" |"DIPLO_UI_STATE_HUMAN_DEMAND"
|
|align="right" |10
|-
|align="left" |"DIPLO_UI_STATE_BLANK_DISCUSSION_RETURN_TO_ROOT"
|
|align="right" |11
|-
|align="left" |"DIPLO_UI_STATE_BLANK_DISCUSSION"
|
|align="right" |12
|-
|align="left" |"DIPLO_UI_STATE_BLANK_DISCUSSION_MEAN_HUMAN"
|
|align="right" |13
|-
|align="left" |"DIPLO_UI_STATE_BLANK_DISCUSSION_MEAN_AI"
|
|align="right" |14
|-
|align="left" |"DIPLO_UI_STATE_AI_DECLARED_WAR"
|
|align="right" |15
|-
|align="left" |"DIPLO_UI_STATE_DISCUSS_HUMAN_INVOKED"
|
|align="right" |16
|-
|align="left" |"DIPLO_UI_STATE_DISCUSS_AGGRESSIVE_MILITARY_WARNING"
|
|align="right" |17
|-
|align="left" |"DIPLO_UI_STATE_DISCUSS_I_ATTACKED_YOUR_MINOR_CIV"
|
|align="right" |18
|-
|align="left" |"DIPLO_UI_STATE_DISCUSS_I_BULLIED_YOUR_MINOR_CIV"
|
|align="right" |19
|-
|align="left" |"DIPLO_UI_STATE_DISCUSS_YOU_ATTACKED_MINOR_CIV"
|
|align="right" |20
|-
|align="left" |"DIPLO_UI_STATE_DISCUSS_YOU_KILLED_MINOR_CIV"
|
|align="right" |21
|-
|align="left" |"DIPLO_UI_STATE_DISCUSS_YOU_BULLIED_MINOR_CIV"
|
|align="right" |22
|-
|align="left" |"DIPLO_UI_STATE_DISCUSS_PROTECT_MINOR_CIV"
|
|align="right" |23
|-
|align="left" |"DIPLO_UI_STATE_DISCUSS_YOU_EXPANSION_SERIOUS_WARNING"
|
|align="right" |24
|-
|align="left" |"DIPLO_UI_STATE_DISCUSS_YOU_EXPANSION_WARNING"
|
|align="right" |25
|-
|align="left" |"DIPLO_UI_STATE_DISCUSS_YOU_PLOT_BUYING_SERIOUS_WARNING"
|
|align="right" |26
|-
|align="left" |"DIPLO_UI_STATE_DISCUSS_YOU_PLOT_BUYING_WARNING"
|
|align="right" |27
|-
|align="left" |"DIPLO_UI_STATE_DISCUSS_WORK_WITH_US"
|
|align="right" |28
|-
|align="left" |"DIPLO_UI_STATE_DISCUSS_WORK_AGAINST_SOMEONE"
|
|align="right" |29
|-
|align="left" |"DIPLO_UI_STATE_DISCUSS_COOP_WAR"
|
|align="right" |30
|-
|align="left" |"DIPLO_UI_STATE_DISCUSS_COOP_WAR_TIME"
|
|align="right" |31
|-
|align="left" |"DIPLO_UI_STATE_DISCUSS_PLAN_RESEARCH_AGREEMENT"
|
|align="right" |32
|-
|align="left" |"DIPLO_UI_STATE_DISCUSS_AI_REQUEST_DENOUNCE"
|
|align="right" |33
|-
|align="left" |"DIPLO_UI_STATE_CAUGHT_YOUR_SPY"
|
|align="right" |34
|-
|align="left" |"DIPLO_UI_STATE_KILLED_YOUR_SPY"
|
|align="right" |35
|-
|align="left" |"DIPLO_UI_STATE_KILLED_MY_SPY"
|
|align="right" |36
|-
|align="left" |"DIPLO_UI_STATE_CONFRONT_YOU_KILLED_MY_SPY"
|
|align="right" |37
|-
|align="left" |"DIPLO_UI_STATE_STOP_CONVERSIONS"
|
|align="right" |38
|-
|align="left" |"NUM_DIPLO_UI_STATES"
|
|align="right" |39
|}</code>


= Examples =
Here is how to use the LUA enumeration to retrieve the ''ID'' from the ''type''. Those examples will return and assign the integer value 0.
<syntaxhighlight lang="lua" class="civ5-example">
local id = DiploUIStateTypes.DIPLO_UI_STATE_DEFAULT_ROOT
local id = DiploUIStateTypes["DIPLO_UI_STATE_DEFAULT_ROOT"]
</syntaxhighlight>


=Used by=
{|cellspacing="4" cellpadding="0" width="100%" style="background-color:#F0F0F0"
<!-- 
AILEADERMESSAGE
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Events}}.{{Func5|Events|AILeaderMessage}}<b>(</b>{{Type5|PlayerID}} player, {{Type5|DiploUIStateType}} diploUIState, '''string''' leaderMessage, '''int''' animationAction, '''int''' data1<b>)</b></code>
|}




{{Civ5 API Footer}}
[[Category:Civ5 Types|DiploUIStateType]]