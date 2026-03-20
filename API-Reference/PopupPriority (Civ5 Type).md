{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|ID.png|The <code>PopupPriority</code> pseudo-type is actually a regular '''integer'''. Pseudo-types do not exist in Lua, they only serve a documentation purpose on the wiki!
* {{Lua}} Integers labeled as <code>PopupPriority</code> corresponds to the constants defined in the '''PopupPriority''' Lua enumeration.
}}


= Lua: the PopupPriority enumeration =
Firaxis provides a Lua enumeration named <code>PopupPriority</code>. This is just a regular global table. Its keys are the constants' names and the pairs the corresponding values.

<br/>Below are the values found in this enumeration.
<code>
{|
|-
!align="left" |Key
!
!align="left" |Value 
|-
|align="left" |"MainMenu"
|
|align="right" |0
|-
|align="left" |"LegalScreen"
|
|align="right" |1
|-
|align="left" |"SinglePlayerScreen"
|
|align="right" |2
|-
|align="left" |"MultiplayerSelectScreen"
|
|align="right" |3
|-
|align="left" |"ModsEULAScreen"
|
|align="right" |4
|-
|align="left" |"OtherMenu"
|
|align="right" |5
|-
|align="left" |"Credits"
|
|align="right" |6
|-
|align="left" |"GameSetupScreen"
|
|align="right" |7
|-
|align="left" |"LoadTutorial"
|
|align="right" |8
|-
|align="left" |"ModsBrowserScreen"
|
|align="right" |9
|-
|align="left" |"ModsMenuScreen"
|
|align="right" |10
|-
|align="left" |"ModdingScenarioSetupScreen"
|
|align="right" |11
|-
|align="left" |"ModdingSinglePlayer"
|
|align="right" |12
|-
|align="left" |"ModMultiplayerSelectScreen"
|
|align="right" |13
|-
|align="left" |"ModdingGameSetupScreen"
|
|align="right" |14
|-
|align="left" |"ModsCustom"
|
|align="right" |15
|-
|align="left" |"LoadGameScreen"
|
|align="right" |16
|-
|align="left" |"AdvancedSetup"
|
|align="right" |17
|-
|align="left" |"SelectCivilization"
|
|align="right" |18
|-
|align="left" |"CustomMod"
|
|align="right" |19
|-
|align="left" |"LobbyScreen"
|
|align="right" |20
|-
|align="left" |"MPGameSetupScreen"
|
|align="right" |21
|-
|align="left" |"MPLoadGameScreen"
|
|align="right" |22
|-
|align="left" |"JoiningScreen"
|
|align="right" |23
|-
|align="left" |"StagingScreen"
|
|align="right" |24
|-
|align="left" |"SocialPolicy"
|
|align="right" |25
|-
|align="left" |"DiploOverview"
|
|align="right" |26
|-
|align="left" |"CityStateDiplo"
|
|align="right" |27
|-
|align="left" |"GenericPopup"
|
|align="right" |28
|-
|align="left" |"TextPopup"
|
|align="right" |29
|-
|align="left" |"AdvisorCounsel"
|
|align="right" |30
|-
|align="left" |"AdvisorInfo"
|
|align="right" |31
|-
|align="left" |"AdvisorModal"
|
|align="right" |32
|-
|align="left" |"BarbarianCamp"
|
|align="right" |33
|-
|align="left" |"CityStateGreeting"
|
|align="right" |34
|-
|align="left" |"GoldenAge"
|
|align="right" |35
|-
|align="left" |"GreatPersonReward"
|
|align="right" |36
|-
|align="left" |"CityStateList"
|
|align="right" |37
|-
|align="left" |"NaturalWonderPopup"
|
|align="right" |38
|-
|align="left" |"NotificationLog"
|
|align="right" |39
|-
|align="left" |"NewEraPopup"
|
|align="right" |40
|-
|align="left" |"TechAward"
|
|align="right" |41
|-
|align="left" |"WhosWinning"
|
|align="right" |42
|-
|align="left" |"GoodyHut"
|
|align="right" |43
|-
|align="left" |"WonderPopup"
|
|align="right" |44
|-
|align="left" |"MilitaryOverview"
|
|align="right" |45
|-
|align="left" |"EconOverview"
|
|align="right" |46
|-
|align="left" |"ProductionPopup"
|
|align="right" |47
|-
|align="left" |"DiploVote"
|
|align="right" |48
|-
|align="left" |"TechTree"
|
|align="right" |49
|-
|align="left" |"EndGameMenu"
|
|align="right" |50
|-
|align="left" |"VictoryProgress"
|
|align="right" |51
|-
|align="left" |"Demographics"
|
|align="right" |52
|-
|align="left" |"VoteResults"
|
|align="right" |53
|-
|align="left" |"InGameMenu"
|
|align="right" |54
|-
|align="left" |"OptionsMenu"
|
|align="right" |55
|-
|align="left" |"SaveMenu"
|
|align="right" |56
|-
|align="left" |"LoadMenu"
|
|align="right" |57
|-
|align="left" |"SaveMapMenu"
|
|align="right" |58
|-
|align="left" |"HallOfFame"
|
|align="right" |59
|-
|align="left" |"Civilopedia"
|
|align="right" |60
|-
|align="left" |"LeaderHead"
|
|align="right" |61
|-
|align="left" |"LeaderDiscuss"
|
|align="right" |62
|-
|align="left" |"LeaderTrade"
|
|align="right" |63
|-
|align="left" |"PlayerChange"
|
|align="right" |64
|-
|align="left" |"eUtmost"
|
|align="right" |65
|}</code>


= Examples =
Here is how to use the LUA enumeration to retrieve the ''ID'' from the ''type''. Those examples will return and assign the integer value 0.
<syntaxhighlight lang="lua" class="civ5-example">
local id = PopupPriority.MainMenu
local id = PopupPriority["MainMenu"]
</syntaxhighlight>


=Used by=
{|cellspacing="4" cellpadding="0" width="100%" style="background-color:#F0F0F0"
<!-- 
QUEUEPOPUP
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|UIManager}}.{{Func5|UIManager|QueuePopup}}<b>(</b>{{Type5|Context}} ContextPtr, {{Type5|PopupPriority}} arg1<b>)</b></code>
|}




{{Civ5 API Footer}}
[[Category:Civ5 Types|PopupPriority]]