{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|ID.png|The <code>ButtonPopupType</code> pseudo-type is actually a regular '''integer'''. Pseudo-types do not exist in Lua, they only serve a documentation purpose on the wiki!
* {{Lua}} Integers labeled as <code>ButtonPopupType</code> corresponds to the constants defined in the '''ButtonPopupTypes''' Lua enumeration.
}}


= Lua: the ButtonPopupTypes enumeration =
Firaxis provides a Lua enumeration named <code>ButtonPopupTypes</code>. This is just a regular global table. Its keys are the constants' names and the pairs the corresponding values.

<br/>Below are the values found in this enumeration.
<code>
{|
|-
!align="left" |Key
!
!align="left" |Value 
|-
|align="left" |"BUTTONPOPUP_TEXT"
|
|align="right" |0
|-
|align="left" |"BUTTONPOPUP_MAIN_MENU"
|
|align="right" |1
|-
|align="left" |"BUTTONPOPUP_CONFIRM_MENU"
|
|align="right" |2
|-
|align="left" |"BUTTONPOPUP_DECLAREWARMOVE"
|
|align="right" |3
|-
|align="left" |"BUTTONPOPUP_DECLAREWARRANGESTRIKE"
|
|align="right" |4
|-
|align="left" |"BUTTONPOPUP_CONFIRMCOMMAND"
|
|align="right" |5
|-
|align="left" |"BUTTONPOPUP_CONFIRM_CITY_TASK"
|
|align="right" |6
|-
|align="left" |"BUTTONPOPUP_CONFIRM_IMPROVEMENT_REBUILD"
|
|align="right" |7
|-
|align="left" |"BUTTONPOPUP_GREAT_PERSON"
|
|align="right" |8
|-
|align="left" |"BUTTONPOPUP_LOADUNIT"
|
|align="right" |9
|-
|align="left" |"BUTTONPOPUP_LEADUNIT"
|
|align="right" |10
|-
|align="left" |"BUTTONPOPUP_CHOOSETECH"
|
|align="right" |11
|-
|align="left" |"BUTTONPOPUP_CITY_CAPTURED"
|
|align="right" |12
|-
|align="left" |"BUTTONPOPUP_ANNEX_CITY"
|
|align="right" |13
|-
|align="left" |"BUTTONPOPUP_LIBERATE_MINOR"
|
|align="right" |14
|-
|align="left" |"BUTTONPOPUP_DISBANDCITY"
|
|align="right" |15
|-
|align="left" |"BUTTONPOPUP_CHOOSEPRODUCTION"
|
|align="right" |16
|-
|align="left" |"BUTTONPOPUP_CHOOSEPOLICY"
|
|align="right" |17
|-
|align="left" |"BUTTONPOPUP_CHOOSECITYPURCHASE"
|
|align="right" |18
|-
|align="left" |"BUTTONPOPUP_CHOOSEELECTION"
|
|align="right" |19
|-
|align="left" |"BUTTONPOPUP_DIPLOVOTE"
|
|align="right" |20
|-
|align="left" |"BUTTONPOPUP_ALARM"
|
|align="right" |21
|-
|align="left" |"BUTTONPOPUP_DEAL_CANCELED"
|
|align="right" |22
|-
|align="left" |"BUTTONPOPUP_PYTHON"
|
|align="right" |23
|-
|align="left" |"BUTTONPOPUP_PYTHON_SCREEN"
|
|align="right" |24
|-
|align="left" |"BUTTONPOPUP_DETAILS"
|
|align="right" |25
|-
|align="left" |"BUTTONPOPUP_ADMIN"
|
|align="right" |26
|-
|align="left" |"BUTTONPOPUP_ADMIN_PASSWORD"
|
|align="right" |27
|-
|align="left" |"BUTTONPOPUP_EXTENDED_GAME"
|
|align="right" |28
|-
|align="left" |"BUTTONPOPUP_DIPLOMACY"
|
|align="right" |29
|-
|align="left" |"BUTTONPOPUP_ADDBUDDY"
|
|align="right" |30
|-
|align="left" |"BUTTONPOPUP_FORCED_DISCONNECT"
|
|align="right" |31
|-
|align="left" |"BUTTONPOPUP_PITBOSS_DISCONNECT"
|
|align="right" |32
|-
|align="left" |"BUTTONPOPUP_KICKED"
|
|align="right" |33
|-
|align="left" |"BUTTONPOPUP_FREE_COLONY"
|
|align="right" |34
|-
|align="left" |"BUTTONPOPUP_LAUNCH"
|
|align="right" |35
|-
|align="left" |"BUTTONPOPUP_MINOR_GOLD"
|
|align="right" |36
|-
|align="left" |"BUTTONPOPUP_MINOR_CIV_QUEST"
|
|align="right" |37
|-
|align="left" |"BUTTONPOPUP_MINOR_CIV_QUEST_COMPLETED"
|
|align="right" |38
|-
|align="left" |"BUTTONPOPUP_MINOR_CIV_INTRUSION"
|
|align="right" |39
|-
|align="left" |"BUTTONPOPUP_MINOR_CIV_GREETING_AND_WAR"
|
|align="right" |40
|-
|align="left" |"BUTTONPOPUP_BARBARIAN_RANSOM"
|
|align="right" |41
|-
|align="left" |"BUTTONPOPUP_MINOR_CIV_ENTER_TERRITORY"
|
|align="right" |42
|-
|align="left" |"BUTTONPOPUP_TEMP_SPECIALISTS"
|
|align="right" |43
|-
|align="left" |"BUTTONPOPUP_NOTIFICATION_LOG"
|
|align="right" |44
|-
|align="left" |"BUTTONPOPUP_ECONOMIC_OVERVIEW"
|
|align="right" |45
|-
|align="left" |"BUTTONPOPUP_MILITARY_OVERVIEW"
|
|align="right" |46
|-
|align="left" |"BUTTONPOPUP_DIPLOMATIC_OVERVIEW"
|
|align="right" |47
|-
|align="left" |"BUTTONPOPUP_DEMOGRAPHICS"
|
|align="right" |48
|-
|align="left" |"BUTTONPOPUP_VICTORY_INFO"
|
|align="right" |49
|-
|align="left" |"BUTTONPOPUP_MINOR_CIVS_LIST"
|
|align="right" |50
|-
|align="left" |"BUTTONPOPUP_GIFT_CONFIRM"
|
|align="right" |51
|-
|align="left" |"BUTTONPOPUP_RETURN_CIVILIAN"
|
|align="right" |52
|-
|align="left" |"BUTTONPOPUP_CONFIRM_POLICY_BRANCH_SWITCH"
|
|align="right" |53
|-
|align="left" |"BUTTONPOPUP_WHOS_WINNING"
|
|align="right" |54
|-
|align="left" |"BUTTONPOPUP_NEW_ERA"
|
|align="right" |55
|-
|align="left" |"BUTTONPOPUP_NATURAL_WONDER_REWARD"
|
|align="right" |56
|-
|align="left" |"BUTTONPOPUP_GOODY_HUT_REWARD"
|
|align="right" |57
|-
|align="left" |"BUTTONPOPUP_BARBARIAN_CAMP_REWARD"
|
|align="right" |58
|-
|align="left" |"BUTTONPOPUP_GOLDEN_AGE_REWARD"
|
|align="right" |59
|-
|align="left" |"BUTTONPOPUP_GREAT_PERSON_REWARD"
|
|align="right" |60
|-
|align="left" |"BUTTONPOPUP_CITY_STATE_GREETING"
|
|align="right" |61
|-
|align="left" |"BUTTONPOPUP_CITY_STATE_MESSAGE"
|
|align="right" |62
|-
|align="left" |"BUTTONPOPUP_CITY_STATE_DIPLO"
|
|align="right" |63
|-
|align="left" |"BUTTONPOPUP_CITY_PLOT_MANAGEMENT"
|
|align="right" |64
|-
|align="left" |"BUTTONPOPUP_DIPLO_VOTE"
|
|align="right" |65
|-
|align="left" |"BUTTONPOPUP_VOTE_RESULTS"
|
|align="right" |66
|-
|align="left" |"BUTTONPOPUP_TECH_TREE"
|
|align="right" |67
|-
|align="left" |"BUTTONPOPUP_TECH_AWARD"
|
|align="right" |68
|-
|align="left" |"BUTTONPOPUP_WONDER_COMPLETED_ACTIVE_PLAYER"
|
|align="right" |69
|-
|align="left" |"BUTTONPOPUP_ADVISOR_INFO"
|
|align="right" |70
|-
|align="left" |"BUTTONPOPUP_ADVISOR_COUNSEL"
|
|align="right" |71
|-
|align="left" |"BUTTONPOPUP_ADVISOR_MODAL"
|
|align="right" |72
|-
|align="left" |"BUTTONPOPUP_RENAME_CITY"
|
|align="right" |73
|-
|align="left" |"BUTTONPOPUP_RENAME_UNIT"
|
|align="right" |74
|-
|align="left" |"BUTTONPOPUP_CHOOSE_FREE_GREAT_PERSON"
|
|align="right" |75
|-
|align="left" |"BUTTONPOPUP_FOUND_PANTHEON"
|
|align="right" |76
|-
|align="left" |"BUTTONPOPUP_FOUND_RELIGION"
|
|align="right" |77
|-
|align="left" |"BUTTONPOPUP_ESPIONAGE_OVERVIEW"
|
|align="right" |78
|-
|align="left" |"BUTTONPOPUP_RELIGION_OVERVIEW"
|
|align="right" |79
|-
|align="left" |"BUTTONPOPUP_CHOOSE_TECH_TO_STEAL"
|
|align="right" |80
|-
|align="left" |"BUTTONPOPUP_CHOOSE_MAYA_BONUS"
|
|align="right" |81
|-
|align="left" |"BUTTONPOPUP_CHOOSE_FAITH_GREAT_PERSON"
|
|align="right" |82
|-
|align="left" |"BUTTONPOPUP_MODDER_0"
|
|align="right" |83
|-
|align="left" |"BUTTONPOPUP_MODDER_1"
|
|align="right" |84
|-
|align="left" |"BUTTONPOPUP_MODDER_2"
|
|align="right" |85
|-
|align="left" |"BUTTONPOPUP_MODDER_3"
|
|align="right" |86
|-
|align="left" |"BUTTONPOPUP_MODDER_4"
|
|align="right" |87
|-
|align="left" |"BUTTONPOPUP_MODDER_5"
|
|align="right" |88
|-
|align="left" |"BUTTONPOPUP_MODDER_6"
|
|align="right" |89
|-
|align="left" |"BUTTONPOPUP_MODDER_7"
|
|align="right" |90
|-
|align="left" |"BUTTONPOPUP_MODDER_8"
|
|align="right" |91
|-
|align="left" |"BUTTONPOPUP_MODDER_9"
|
|align="right" |92
|-
|align="left" |"BUTTONPOPUP_MODDER_10"
|
|align="right" |93
|-
|align="left" |"BUTTONPOPUP_MODDER_11"
|
|align="right" |94
|-
|align="left" |"NUM_BUTTONPOPUP_TYPES"
|
|align="right" |95
|}</code>


= Examples =
Here is how to use the LUA enumeration to retrieve the ''ID'' from the ''type''. Those examples will return and assign the integer value 0.
<syntaxhighlight lang="lua" class="civ5-example">
local id = ButtonPopupTypes.BUTTONPOPUP_TEXT
local id = ButtonPopupTypes["BUTTONPOPUP_TEXT"]
</syntaxhighlight>


=Used by=
{|cellspacing="4" cellpadding="0" width="100%" style="background-color:#F0F0F0"
<!-- 
SERIALEVENTGAMEMESSAGEPOPUPPROCESSED
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Events}}.{{Func5|Events|SerialEventGameMessagePopupProcessed}}<b>(</b>{{Type5|ButtonPopupType}} mostRecentPopup, '''int''' arg1<b>)</b></code>
<!-- 
ADDPOPUP
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|UI}}.{{Func5|UI|AddPopup}}<b>(</b>'''table''' popupInfo<b>)</b></code>
|}




{{Civ5 API Footer}}
[[Category:Civ5 Types|ButtonPopupType]]