{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|ID.png|The <code>GameMessageType</code> pseudo-type is actually a regular '''integer'''. Pseudo-types do not exist in Lua, they only serve a documentation purpose on the wiki!
* {{Lua}} Integers labeled as <code>GameMessageType</code> corresponds to the constants defined in the '''GameMessageTypes''' Lua enumeration.
}}


= Lua: the GameMessageTypes enumeration =
Firaxis provides a Lua enumeration named <code>GameMessageTypes</code>. This is just a regular global table. Its keys are the constants' names and the pairs the corresponding values.

<br/>Below are the values found in this enumeration.
<code>
{|
|-
!align="left" |Key
!
!align="left" |Value 
|-
|align="left" |"GAMEMESSAGE_NETWORK_READY"
|
|align="right" |0
|-
|align="left" |"GAMEMESSAGE_VERIFY_VERSION"
|
|align="right" |1
|-
|align="left" |"GAMEMESSAGE_VERSION_NACK"
|
|align="right" |2
|-
|align="left" |"GAMEMESSAGE_VERSION_WARNING"
|
|align="right" |3
|-
|align="left" |"GAMEMESSAGE_GAME_TYPE"
|
|align="right" |4
|-
|align="left" |"GAMEMESSAGE_ID_ASSIGNMENT"
|
|align="right" |5
|-
|align="left" |"GAMEMESSAGE_FILE_INFO"
|
|align="right" |6
|-
|align="left" |"GAMEMESSAGE_PICK_YOUR_CIV"
|
|align="right" |7
|-
|align="left" |"GAMEMESSAGE_CIV_CHOICE"
|
|align="right" |8
|-
|align="left" |"GAMEMESSAGE_CONFIRM_CIV_CLAIM"
|
|align="right" |9
|-
|align="left" |"GAMEMESSAGE_CLAIM_INFO"
|
|align="right" |10
|-
|align="left" |"GAMEMESSAGE_CIV_CHOICE_ACK"
|
|align="right" |11
|-
|align="left" |"GAMEMESSAGE_CIV_CHOICE_NACK"
|
|align="right" |12
|-
|align="left" |"GAMEMESSAGE_CIV_CHOSEN"
|
|align="right" |13
|-
|align="left" |"GAMEMESSAGE_INTERIM_NOTICE"
|
|align="right" |14
|-
|align="left" |"GAMEMESSAGE_INIT_INFO"
|
|align="right" |15
|-
|align="left" |"GAMEMESSAGE_MAPSCRIPT_CHECK"
|
|align="right" |16
|-
|align="left" |"GAMEMESSAGE_MAPSCRIPT_ACK"
|
|align="right" |17
|-
|align="left" |"GAMEMESSAGE_LOAD_GAME"
|
|align="right" |18
|-
|align="left" |"GAMEMESSAGE_PLAYER_ID"
|
|align="right" |19
|-
|align="left" |"GAMEMESSAGE_SLOT_REASSIGNMENT"
|
|align="right" |20
|-
|align="left" |"GAMEMESSAGE_PLAYER_INFO"
|
|align="right" |21
|-
|align="left" |"GAMEMESSAGE_GAME_INFO"
|
|align="right" |22
|-
|align="left" |"GAMEMESSAGE_REASSIGN_PLAYER"
|
|align="right" |23
|-
|align="left" |"GAMEMESSAGE_PITBOSS_INFO"
|
|align="right" |24
|-
|align="left" |"GAMEMESSAGE_LAUNCHING_INFO"
|
|align="right" |25
|-
|align="left" |"GAMEMESSAGE_INIT_GAME"
|
|align="right" |26
|-
|align="left" |"GAMEMESSAGE_INIT_PLAYERS"
|
|align="right" |27
|-
|align="left" |"GAMEMESSAGE_AUTH_REQUEST"
|
|align="right" |28
|-
|align="left" |"GAMEMESSAGE_AUTH_RESPONSE"
|
|align="right" |29
|-
|align="left" |"GAMEMESSAGE_SYNCH_START"
|
|align="right" |30
|-
|align="left" |"GAMEMESSAGE_PLAYER_OPTION"
|
|align="right" |31
|-
|align="left" |"GAMEMESSAGE_EXTENDED_GAME"
|
|align="right" |32
|-
|align="left" |"GAMEMESSAGE_AUTO_MOVES"
|
|align="right" |33
|-
|align="left" |"GAMEMESSAGE_TURN_COMPLETE"
|
|align="right" |34
|-
|align="left" |"GAMEMESSAGE_PUSH_MISSION"
|
|align="right" |35
|-
|align="left" |"GAMEMESSAGE_AUTO_MISSION"
|
|align="right" |36
|-
|align="left" |"GAMEMESSAGE_DO_COMMAND"
|
|align="right" |37
|-
|align="left" |"GAMEMESSAGE_PUSH_ORDER"
|
|align="right" |38
|-
|align="left" |"GAMEMESSAGE_POP_ORDER"
|
|align="right" |39
|-
|align="left" |"GAMEMESSAGE_DO_TASK"
|
|align="right" |41
|-
|align="left" |"GAMEMESSAGE_RESEARCH"
|
|align="right" |42
|-
|align="left" |"GAMEMESSAGE_CONVERT"
|
|align="right" |43
|-
|align="left" |"GAMEMESSAGE_CHAT"
|
|align="right" |44
|-
|align="left" |"GAMEMESSAGE_PING"
|
|align="right" |45
|-
|align="left" |"GAMEMESSAGE_SIGN"
|
|align="right" |46
|-
|align="left" |"GAMEMESSAGE_LINE_ENTITY"
|
|align="right" |47
|-
|align="left" |"GAMEMESSAGE_SIGN_DELETE"
|
|align="right" |48
|-
|align="left" |"GAMEMESSAGE_LINE_ENTITY_DELETE"
|
|align="right" |49
|-
|align="left" |"GAMEMESSAGE_LINE_GROUP_DELETE"
|
|align="right" |50
|-
|align="left" |"GAMEMESSAGE_PAUSE"
|
|align="right" |51
|-
|align="left" |"GAMEMESSAGE_MP_KICK"
|
|align="right" |52
|-
|align="left" |"GAMEMESSAGE_MP_RETIRE"
|
|align="right" |53
|-
|align="left" |"GAMEMESSAGE_CLOSE_CONNECTION"
|
|align="right" |54
|-
|align="left" |"GAMEMESSAGE_NEVER_JOINED"
|
|align="right" |55
|-
|align="left" |"GAMEMESSAGE_MP_DROP_INIT"
|
|align="right" |56
|-
|align="left" |"GAMEMESSAGE_MP_DROP_VOTE"
|
|align="right" |57
|-
|align="left" |"GAMEMESSAGE_MP_DROP_UPDATE"
|
|align="right" |58
|-
|align="left" |"GAMEMESSAGE_MP_DROP_RESULT"
|
|align="right" |59
|-
|align="left" |"GAMEMESSAGE_MP_DROP_SAVE"
|
|align="right" |60
|-
|align="left" |"GAMEMESSAGE_TOGGLE_TRADE"
|
|align="right" |61
|-
|align="left" |"GAMEMESSAGE_IMPLEMENT_OFFER"
|
|align="right" |62
|-
|align="left" |"GAMEMESSAGE_CHANGE_WAR"
|
|align="right" |63
|-
|align="left" |"GAMEMESSAGE_LIBERATE_PLAYER"
|
|align="right" |66
|-
|align="left" |"GAMEMESSAGE_CHOOSE_ELECTION"
|
|align="right" |67
|-
|align="left" |"GAMEMESSAGE_DIPLO_VOTE"
|
|align="right" |68
|-
|align="left" |"GAMEMESSAGE_APPLY_EVENT"
|
|align="right" |69
|-
|align="left" |"GAMEMESSAGE_CONTACT_CIV"
|
|align="right" |70
|-
|align="left" |"GAMEMESSAGE_DIPLO_CHAT"
|
|align="right" |71
|-
|align="left" |"GAMEMESSAGE_SEND_OFFER"
|
|align="right" |72
|-
|align="left" |"GAMEMESSAGE_RENEGOTIATE"
|
|align="right" |73
|-
|align="left" |"GAMEMESSAGE_RENEGOTIATE_ITEM"
|
|align="right" |74
|-
|align="left" |"GAMEMESSAGE_EXIT_TRADE"
|
|align="right" |75
|-
|align="left" |"GAMEMESSAGE_KILL_DEAL"
|
|align="right" |76
|-
|align="left" |"GAMEMESSAGE_UPDATE_POLICIES"
|
|align="right" |77
|-
|align="left" |"GAMEMESSAGE_CLEAR_TABLE"
|
|align="right" |78
|-
|align="left" |"GAMEMESSAGE_POPUP_PROCESSED"
|
|align="right" |79
|-
|align="left" |"GAMEMESSAGE_DIPLOMACY_FROM_UI"
|
|align="right" |80
|-
|align="left" |"GAMEMESSAGE_HOT_JOIN_NOTICE"
|
|align="right" |81
|-
|align="left" |"GAMEMESSAGE_HOT_DROP_NOTICE"
|
|align="right" |82
|-
|align="left" |"GAMEMESSAGE_POPUP"
|
|align="right" |83
|-
|align="left" |"GAMEMESSAGE_EVENT_TRIGGERED"
|
|align="right" |84
|-
|align="left" |"GAMEMESSAGE_LAUNCH_SPACESHIP"
|
|align="right" |85
|-
|align="left" |"GAMEMESSAGE_ADVANCED_START_ACTION"
|
|align="right" |86
|-
|align="left" |"GAMEMESSAGE_MINOR_CIV_QUEST_NO_INTEREST"
|
|align="right" |87
|-
|align="left" |"GAMEMESSAGE_MINOR_CIV_QUEST_COMPLETED"
|
|align="right" |88
|-
|align="left" |"GAMEMESSAGE_MINOR_CIV_INTRUSION"
|
|align="right" |89
|-
|align="left" |"GAMEMESSAGE_MINOR_CIV_ENTER_TERRITORY"
|
|align="right" |90
|-
|align="left" |"GAMEMESSAGE_BARBARIAN_RANSOM"
|
|align="right" |91
|-
|align="left" |"GAMEMESSAGE_PLAYER_HURRY"
|
|align="right" |96
|-
|align="left" |"GAMEMESSAGE_MOD_NET_MESSAGE"
|
|align="right" |97
|-
|align="left" |"GAMEMESSAGE_SWAP_UNITS"
|
|align="right" |98
|-
|align="left" |"GAMEMESSAGE_SWAP_ORDER"
|
|align="right" |124
|-
|align="left" |"GAMEMESSAGE_AVOID_GROWTH"
|
|align="right" |127
|}</code>


= Examples =
Here is how to use the LUA enumeration to retrieve the ''ID'' from the ''type''. Those examples will return and assign the integer value 0.
<syntaxhighlight lang="lua" class="civ5-example">
local id = GameMessageTypes.GAMEMESSAGE_NETWORK_READY
local id = GameMessageTypes["GAMEMESSAGE_NETWORK_READY"]
</syntaxhighlight>


=Used by=
{|cellspacing="4" cellpadding="0" width="100%" style="background-color:#F0F0F0"
<!-- 
SELECTEDCITIESGAMENETMESSAGE
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Game}}.{{Func5|Game|SelectedCitiesGameNetMessage}}<b>(</b>{{Type5|GameMessageType}} message, {{Type5|TaskType}} data2, '''int''' data3, {{Type5|BuildingType}} data4, '''bool''' option, '''bool''' alt, '''bool''' shift, '''bool''' ctrl<b>)</b></code>
<!-- 
SELECTIONLISTGAMENETMESSAGE
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Game}}.{{Func5|Game|SelectionListGameNetMessage}}<b>(</b>{{Type5|GameMessageType}} message, '''int''' data2 = -1, {{Type5|BuildActionType}} data3 = -1, {{Type5|UnitID}} data4 = -1, '''int''' flags = 0, '''bool''' alt = false, '''bool''' shift = false<b>)</b></code>
|}




{{Civ5 API Footer}}
[[Category:Civ5 Types|GameMessageType]]