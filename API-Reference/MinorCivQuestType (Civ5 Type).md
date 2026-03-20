{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|ID.png|The <code>MinorCivQuestType</code> pseudo-type is actually a regular '''integer'''. Pseudo-types do not exist in Lua, they only serve a documentation purpose on the wiki!
* {{Lua}} Integers labeled as <code>MinorCivQuestType</code> corresponds to the constants defined in the '''MinorCivQuestTypes''' Lua enumeration.
}}


= Lua: the MinorCivQuestTypes enumeration =
Firaxis provides a Lua enumeration named <code>MinorCivQuestTypes</code>. This is just a regular global table. Its keys are the constants' names and the pairs the corresponding values.

<br/>Below are the values found in this enumeration.
<code>
{|
|-
!align="left" |Key
!
!align="left" |Value 
|-
|align="left" |"NO_MINOR_CIV_QUEST_TYPE"
|
|align="right" |-1
|-
|align="left" |"MINOR_CIV_QUEST_ROUTE"
|
|align="right" |0
|-
|align="left" |"MINOR_CIV_QUEST_KILL_CAMP"
|
|align="right" |1
|-
|align="left" |"MINOR_CIV_QUEST_CONNECT_RESOURCE"
|
|align="right" |2
|-
|align="left" |"MINOR_CIV_QUEST_CONSTRUCT_WONDER"
|
|align="right" |3
|-
|align="left" |"MINOR_CIV_QUEST_GREAT_PERSON"
|
|align="right" |4
|-
|align="left" |"MINOR_CIV_QUEST_KILL_CITY_STATE"
|
|align="right" |5
|-
|align="left" |"MINOR_CIV_QUEST_FIND_PLAYER"
|
|align="right" |6
|-
|align="left" |"MINOR_CIV_QUEST_FIND_NATURAL_WONDER"
|
|align="right" |7
|-
|align="left" |"MINOR_CIV_QUEST_GIVE_GOLD"
|
|align="right" |8
|-
|align="left" |"MINOR_CIV_QUEST_PLEDGE_TO_PROTECT"
|
|align="right" |9
|-
|align="left" |"MINOR_CIV_QUEST_CONTEST_CULTURE"
|
|align="right" |10
|-
|align="left" |"MINOR_CIV_QUEST_CONTEST_FAITH"
|
|align="right" |11
|-
|align="left" |"MINOR_CIV_QUEST_CONTEST_TECHS"
|
|align="right" |12
|-
|align="left" |"MINOR_CIV_QUEST_INVEST"
|
|align="right" |13
|-
|align="left" |"MINOR_CIV_QUEST_BULLY_CITY_STATE"
|
|align="right" |14
|-
|align="left" |"MINOR_CIV_QUEST_DENOUNCE_MAJOR"
|
|align="right" |15
|-
|align="left" |"MINOR_CIV_QUEST_SPREAD_RELIGION"
|
|align="right" |16
|-
|align="left" |"NUM_MINOR_CIV_QUEST_TYPES"
|
|align="right" |17
|}</code>


= Examples =
Here is how to use the LUA enumeration to retrieve the ''ID'' from the ''type''. Those examples will return and assign the integer value 0.
<syntaxhighlight lang="lua" class="civ5-example">
local id = MinorCivQuestTypes.MINOR_CIV_QUEST_ROUTE
local id = MinorCivQuestTypes["MINOR_CIV_QUEST_ROUTE"]
</syntaxhighlight>


=Used by=
{|cellspacing="4" cellpadding="0" width="100%" style="background-color:#F0F0F0"
<!-- 
GETACTIVEQUESTFORPLAYER
-->
|-
|align="right" width="200" |<code>{{Type5|MinorCivQuestType}}</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|GetActiveQuestForPlayer}}<b>(</b>{{Type5|PlayerID}} player<b>)</b></code>
<!-- 
GETMINORCIVCONTESTVALUEFORLEADER
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|GetMinorCivContestValueForLeader}}<b>(</b>{{Type5|MinorCivQuestType}} arg0<b>)</b></code>
<!-- 
GETMINORCIVCONTESTVALUEFORPLAYER
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|GetMinorCivContestValueForPlayer}}<b>(</b>{{Type5|PlayerID}} major, {{Type5|MinorCivQuestType}} arg1<b>)</b></code>
<!-- 
GETQUESTDATA1
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|GetQuestData1}}<b>(</b>{{Type5|PlayerID}} major, {{Type5|MinorCivQuestType}} type = nil<b>)</b></code>
<!-- 
GETQUESTDATA2
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|GetQuestData2}}<b>(</b>{{Type5|PlayerID}} major, {{Type5|MinorCivQuestType}} type = nil<b>)</b></code>
<!-- 
GETQUESTTURNSREMAINING
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|GetQuestTurnsRemaining}}<b>(</b>{{Type5|PlayerID}} major, {{Type5|MinorCivQuestType}} type, {{Type5|PlayerID}} arg2<b>)</b></code>
<!-- 
ISMINORCIVACTIVEQUESTFORPLAYER
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|IsMinorCivActiveQuestForPlayer}}<b>(</b>{{Type5|PlayerID}} major, {{Type5|MinorCivQuestType}} type<b>)</b></code>
<!-- 
ISMINORCIVCONTESTLEADER
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|IsMinorCivContestLeader}}<b>(</b>{{Type5|PlayerID}} major, {{Type5|MinorCivQuestType}} arg1<b>)</b></code>
|}




{{Civ5 API Footer}}
[[Category:Civ5 Types|MinorCivQuestType]]