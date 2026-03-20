{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|ID.png|The <code>NotificationType</code> pseudo-type is actually a regular '''integer'''. Pseudo-types do not exist in Lua, they only serve a documentation purpose on the wiki!
* {{DB}} Integers labeled as <code>NotificationType</code> corresponds to the ''ID'' column of the {{Table5|Notifications|Notifications}} XML table.
* {{Lua}} The standard (unmodded) values in the ''ID'' and ''Type'' columns are also stored in the '''NotificationTypes''' Lua enumeration.
}}


= Lua: the NotificationTypes enumeration =
Firaxis provides a Lua enumeration named <code>NotificationTypes</code>. This is just a regular global table. Its keys are the constants' names and the pairs the corresponding values.
* This specific enumeration contains data from the {{Table5|Notifications|Notifications}} data table.<br/>
* They are stored as key/value pairs: the keys are the strings from the ''Type'' column and the values are the integers from the ''ID'' column.<br/>
{{Warning}} Be careful: this enumeration do '''not''' reflect the changes, additions and deletions made by mods. As a result it is advised to rely on {{Type5|GameInfo}} instead.<br/>

<br/>Below are the values found in this enumeration.
<code>
{|
|-
!align="left" |Key
!
!align="left" |Value 
|-
|align="left" |"NOTIFICATION_GENERIC"
|
|align="right" |0
|-
|align="left" |"NOTIFICATION_TECH"
|
|align="right" |1
|-
|align="left" |"NOTIFICATION_FREE_TECH"
|
|align="right" |2
|-
|align="left" |"NOTIFICATION_POLICY"
|
|align="right" |3
|-
|align="left" |"NOTIFICATION_PRODUCTION"
|
|align="right" |4
|-
|align="left" |"NOTIFICATION_MET_MINOR"
|
|align="right" |5
|-
|align="left" |"NOTIFICATION_MINOR"
|
|align="right" |6
|-
|align="left" |"NOTIFICATION_MINOR_QUEST"
|
|align="right" |7
|-
|align="left" |"NOTIFICATION_ENEMY_IN_TERRITORY"
|
|align="right" |8
|-
|align="left" |"NOTIFICATION_CITY_RANGE_ATTACK"
|
|align="right" |9
|-
|align="left" |"NOTIFICATION_BARBARIAN"
|
|align="right" |10
|-
|align="left" |"NOTIFICATION_GOODY"
|
|align="right" |11
|-
|align="left" |"NOTIFICATION_BUY_TILE"
|
|align="right" |12
|-
|align="left" |"NOTIFICATION_CITY_GROWTH"
|
|align="right" |13
|-
|align="left" |"NOTIFICATION_CITY_TILE"
|
|align="right" |14
|-
|align="left" |"NOTIFICATION_DEMAND_RESOURCE"
|
|align="right" |15
|-
|align="left" |"NOTIFICATION_UNIT_PROMOTION"
|
|align="right" |16
|-
|align="left" |"NOTIFICATION_WONDER_COMPLETED_ACTIVE_PLAYER"
|
|align="right" |17
|-
|align="left" |"NOTIFICATION_WONDER_COMPLETED"
|
|align="right" |18
|-
|align="left" |"NOTIFICATION_WONDER_BEATEN"
|
|align="right" |19
|-
|align="left" |"NOTIFICATION_GOLDEN_AGE_BEGUN_ACTIVE_PLAYER"
|
|align="right" |20
|-
|align="left" |"NOTIFICATION_GOLDEN_AGE_ENDED_ACTIVE_PLAYER"
|
|align="right" |21
|-
|align="left" |"NOTIFICATION_GREAT_PERSON_ACTIVE_PLAYER"
|
|align="right" |22
|-
|align="left" |"NOTIFICATION_STARVING"
|
|align="right" |23
|-
|align="left" |"NOTIFICATION_WAR_ACTIVE_PLAYER"
|
|align="right" |24
|-
|align="left" |"NOTIFICATION_WAR"
|
|align="right" |25
|-
|align="left" |"NOTIFICATION_PEACE_ACTIVE_PLAYER"
|
|align="right" |26
|-
|align="left" |"NOTIFICATION_PEACE"
|
|align="right" |27
|-
|align="left" |"NOTIFICATION_VICTORY"
|
|align="right" |28
|-
|align="left" |"NOTIFICATION_UNIT_DIED"
|
|align="right" |29
|-
|align="left" |"NOTIFICATION_CITY_LOST"
|
|align="right" |30
|-
|align="left" |"NOTIFICATION_CAPITAL_LOST_ACTIVE_PLAYER"
|
|align="right" |31
|-
|align="left" |"NOTIFICATION_CAPITAL_LOST"
|
|align="right" |32
|-
|align="left" |"NOTIFICATION_CAPITAL_RECOVERED"
|
|align="right" |33
|-
|align="left" |"NOTIFICATION_PLAYER_KILLED"
|
|align="right" |34
|-
|align="left" |"NOTIFICATION_DISCOVERED_LUXURY_RESOURCE"
|
|align="right" |35
|-
|align="left" |"NOTIFICATION_DISCOVERED_STRATEGIC_RESOURCE"
|
|align="right" |36
|-
|align="left" |"NOTIFICATION_DISCOVERED_BONUS_RESOURCE"
|
|align="right" |37
|-
|align="left" |"NOTIFICATION_DIPLO_VOTE"
|
|align="right" |38
|-
|align="left" |"NOTIFICATION_RELIGION_RACE"
|
|align="right" |39
|-
|align="left" |"NOTIFICATION_EXPLORATION_RACE"
|
|align="right" |40
|-
|align="left" |"NOTIFICATION_DIPLOMACY_DECLARATION"
|
|align="right" |41
|-
|align="left" |"NOTIFICATION_DEAL_EXPIRED_GPT"
|
|align="right" |42
|-
|align="left" |"NOTIFICATION_DEAL_EXPIRED_RESOURCE"
|
|align="right" |43
|-
|align="left" |"NOTIFICATION_DEAL_EXPIRED_OPEN_BORDERS"
|
|align="right" |44
|-
|align="left" |"NOTIFICATION_DEAL_EXPIRED_DEFENSIVE_PACT"
|
|align="right" |45
|-
|align="left" |"NOTIFICATION_DEAL_EXPIRED_RESEARCH_AGREEMENT"
|
|align="right" |46
|-
|align="left" |"NOTIFICATION_DEAL_EXPIRED_TRADE_AGREEMENT"
|
|align="right" |47
|-
|align="left" |"NOTIFICATION_TECH_AWARD"
|
|align="right" |48
|-
|align="left" |"NOTIFICATION_PLAYER_DEAL"
|
|align="right" |49
|-
|align="left" |"NOTIFICATION_PLAYER_DEAL_RECEIVED"
|
|align="right" |50
|-
|align="left" |"NOTIFICATION_PLAYER_DEAL_RESOLVED"
|
|align="right" |51
|-
|align="left" |"NOTIFICATION_PROJECT_COMPLETED"
|
|align="right" |52
|-
|align="left" |"NOTIFICATION_REBELS"
|
|align="right" |53
|-
|align="left" |"NOTIFICATION_FREE_POLICY"
|
|align="right" |54
|-
|align="left" |"NOTIFICATION_FREE_GREAT_PERSON"
|
|align="right" |55
|-
|align="left" |"NOTIFICATION_DENUNCIATION_EXPIRED"
|
|align="right" |56
|-
|align="left" |"NOTIFICATION_FRIENDSHIP_EXPIRED"
|
|align="right" |57
|-
|align="left" |"NOTIFICATION_RELIGION_FOUNDED_ACTIVE_PLAYER"
|
|align="right" |58
|-
|align="left" |"NOTIFICATION_RELIGION_FOUNDED"
|
|align="right" |59
|-
|align="left" |"NOTIFICATION_PANTHEON_FOUNDED_ACTIVE_PLAYER"
|
|align="right" |60
|-
|align="left" |"NOTIFICATION_PANTHEON_FOUNDED"
|
|align="right" |61
|-
|align="left" |"NOTIFICATION_FOUND_PANTHEON"
|
|align="right" |62
|-
|align="left" |"NOTIFICATION_FOUND_RELIGION"
|
|align="right" |63
|-
|align="left" |"NOTIFICATION_ENHANCE_RELIGION"
|
|align="right" |64
|-
|align="left" |"NOTIFICATION_RELIGION_ENHANCED_ACTIVE_PLAYER"
|
|align="right" |65
|-
|align="left" |"NOTIFICATION_RELIGION_ENHANCED"
|
|align="right" |66
|-
|align="left" |"NOTIFICATION_SPY_CREATED_ACTIVE_PLAYER"
|
|align="right" |67
|-
|align="left" |"NOTIFICATION_SPY_STOLE_TECH"
|
|align="right" |68
|-
|align="left" |"NOTIFICATION_SPY_CANT_STEAL_TECH"
|
|align="right" |69
|-
|align="left" |"NOTIFICATION_CAN_BUILD_MISSIONARY"
|
|align="right" |70
|-
|align="left" |"NOTIFICATION_OTHER_PLAYER_NEW_ERA"
|
|align="right" |71
|-
|align="left" |"NOTIFICATION_SPY_EVICTED"
|
|align="right" |72
|-
|align="left" |"NOTIFICATION_RELIGION_SPREAD"
|
|align="right" |73
|-
|align="left" |"NOTIFICATION_TECH_STOLEN_SPY_DETECTED"
|
|align="right" |74
|-
|align="left" |"NOTIFICATION_TECH_STOLEN_SPY_IDENTIFIED"
|
|align="right" |75
|-
|align="left" |"NOTIFICATION_SPY_WAS_KILLED"
|
|align="right" |76
|-
|align="left" |"NOTIFICATION_SPY_KILLED_A_SPY"
|
|align="right" |77
|-
|align="left" |"NOTIFICATION_SPY_REPLACEMENT"
|
|align="right" |78
|-
|align="left" |"NOTIFICATION_MAYA_LONG_COUNT"
|
|align="right" |79
|-
|align="left" |"NOTIFICATION_FAITH_GREAT_PERSON"
|
|align="right" |80
|-
|align="left" |"NOTIFICATION_SPY_PROMOTION"
|
|align="right" |81
|-
|align="left" |"NOTIFICATION_INTRIGUE_DECEPTION"
|
|align="right" |82
|-
|align="left" |"NOTIFICATION_SPY_RIG_ELECTION_SUCCESS"
|
|align="right" |83
|-
|align="left" |"NOTIFICATION_SPY_RIG_ELECTION_FAILURE"
|
|align="right" |84
|-
|align="left" |"NOTIFICATION_SPY_RIG_ELECTION_ALERT"
|
|align="right" |85
|-
|align="left" |"NOTIFICATION_SPY_YOU_STAGE_COUP_SUCCESS"
|
|align="right" |86
|-
|align="left" |"NOTIFICATION_SPY_YOU_STAGE_COUP_FAILURE"
|
|align="right" |87
|-
|align="left" |"NOTIFICATION_SPY_STAGE_COUP_SUCCESS"
|
|align="right" |88
|-
|align="left" |"NOTIFICATION_SPY_STAGE_COUP_FAILURE"
|
|align="right" |89
|-
|align="left" |"NOTIFICATION_INTRIGUE_BUILDING_SNEAK_ATTACK_ARMY"
|
|align="right" |90
|-
|align="left" |"NOTIFICATION_INTRIGUE_BUILDING_SNEAK_ATTACK_AMPHIBIOUS"
|
|align="right" |91
|-
|align="left" |"NOTIFICATION_INTRIGUE_SNEAK_ATTACK_ARMY_AGAINST_KNOWN_CITY_UNKNOWN"
|
|align="right" |92
|-
|align="left" |"NOTIFICATION_INTRIGUE_SNEAK_ATTACK_ARMY_AGAINST_KNOWN_CITY_KNOWN"
|
|align="right" |93
|-
|align="left" |"NOTIFICATION_INTRIGUE_SNEAK_ATTACK_ARMY_AGAINST_YOU_CITY_UNKNOWN"
|
|align="right" |94
|-
|align="left" |"NOTIFICATION_INTRIGUE_SNEAK_ATTACK_ARMY_AGAINST_YOU_CITY_KNOWN"
|
|align="right" |95
|-
|align="left" |"NOTIFICATION_INTRIGUE_SNEAK_ATTACK_ARMY_AGAINST_UNKNOWN"
|
|align="right" |96
|-
|align="left" |"NOTIFICATION_INTRIGUE_SNEAK_ATTACK_AMPHIB_AGAINST_KNOWN_CITY_UNKNOWN"
|
|align="right" |97
|-
|align="left" |"NOTIFICATION_INTRIGUE_SNEAK_ATTACK_AMPHIB_AGAINST_KNOWN_CITY_KNOWN"
|
|align="right" |98
|-
|align="left" |"NOTIFICATION_INTRIGUE_SNEAK_ATTACK_AMPHIB_AGAINST_YOU_CITY_UNKNOWN"
|
|align="right" |99
|-
|align="left" |"NOTIFICATION_INTRIGUE_SNEAK_ATTACK_AMPHIB_AGAINST_YOU_CITY_KNOWN"
|
|align="right" |100
|-
|align="left" |"NOTIFICATION_INTRIGUE_SNEAK_ATTACK_AMPHIB_AGAINST_UNKNOWN"
|
|align="right" |101
|-
|align="left" |"NOTIFICATION_RELIGION_ERROR"
|
|align="right" |102
|-
|align="left" |"NOTIFICATION_AUTOMATIC_FAITH_PURCHASE_STOPPED"
|
|align="right" |103
|-
|align="left" |"NOTIFICATION_EXPANSION_PROMISE_EXPIRED"
|
|align="right" |104
|-
|align="left" |"NOTIFICATION_BORDER_PROMISE_EXPIRED"
|
|align="right" |105
|-
|align="left" |"NOTIFICATION_TRADE_ROUTE"
|
|align="right" |106
|-
|align="left" |"NOTIFICATION_TRADE_ROUTE_BROKEN"
|
|align="right" |107
|-
|align="left" |"NOTIFICATION_RELIGION_SPREAD_NATURAL"
|
|align="right" |108
|-
|align="left" |"NOTIFICATION_INTRIGUE_CONSTRUCTING_WONDER"
|
|align="right" |109
|-
|align="left" |"NOTIFICATION_MINOR_BUYOUT"
|
|align="right" |110
|-
|align="left" |"NUM_NOTIFICATION_TYPES"
|
|align="right" |111
|}</code>


= Examples =
Here is how to use the LUA enumeration to retrieve the ''ID'' from the ''type''. Those examples will return and assign the integer value 0.
<syntaxhighlight lang="lua" class="civ5-example">
local id = NotificationTypes.NOTIFICATION_GENERIC
local id = NotificationTypes["NOTIFICATION_GENERIC"]
</syntaxhighlight>


=Used by=
{|cellspacing="4" cellpadding="0" width="100%" style="background-color:#F0F0F0"
<!-- 
NOTIFICATIONADDED
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Events}}.{{Func5|Events|NotificationAdded}}<b>(</b>{{Type5|CityAIFocusType}} notification, {{Type5|NotificationType}} notificationType, '''string''' toolTip, '''string''' summary, '''int''' gameValue, {{Type5|TechType}} extraGameData<b>)</b></code>
<!-- 
ADDNOTIFICATION
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|AddNotification}}<b>(</b>{{Type5|NotificationType}} notificationType, '''string''' description, '''string''' title, '''int''' x = -1, '''int''' y = -1, {{Type5|PlayerID}} extra1 = -1, '''int''' extra2 = -1<b>)</b></code>
|}




{{Civ5 API Footer}}
[[Category:Civ5 Types|NotificationType]]